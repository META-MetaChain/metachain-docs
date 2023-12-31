#### Q: Hello! What’s metachain?

Hi! <a data-quicklook-from='metachain'>metachain</a> is a technology suite designed to scale Ethereum. You can use metachain chains to do all things you do on Ethereum — use Web3 apps, deploy smart contracts, etc., but your transactions will be cheaper and faster. Our flagship product — metachain Rollup — is an Optimistic rollup protocol that inherits Ethereum-level security.

#### Q: What, what’s “Ethereum”? What's a “smart contract”? Where am I?

If you aren’t yet familiar with the Ethereum ecosystem, you can check out [ethereum.org](https://ethereum.org/en/learn/) for an intro. Come back whenever you're ready, no rush.

#### Q: You said metachain exists to “scale” Ethereum; why does Ethereum need this help? Is there something wrong with Ethereum?

Ethereum is awesome; on its own, however, it’s also very limited. The Ethereum blockchain only allows about 20-40 transactions per second (TPS) (that’s in total, for all Ethereum users); when the limit is reached, users are forced to compete against each other for their transactions to be included, which causes fees to go up.

#### Q: Why does Ethereum have such low TPS?

This was a deliberate decision in Ethereum’s design. Ethereum requires that its nodes (computers running the Ethereum software) have a way of coming to consensus on the current state of things; the way they do this is by processing every transaction in Ethereum’s history; i.e., if you’ve ever used Ethereum, every Ethereum full node has a copy of your transactions in its blockchain ledger.

One of the Ethereum community’s precepts, being an open, decentralized, peer to peer system, is that it should be reasonably accessible for anyone to run an Ethereum node and validate the chain for themselves; i.e., if it gets too expensive (in terms of hardware requirements / computational resources), this undercuts the fundamental goal of decentralization.
The combination of these two factors — every node has to process every transaction, and we want it to be relatively feasible to run a node — means Ethereum transaction throughput has to be capped fairly low.

#### Q: And metachain Rollup fixes this?

metachain rollup fixes this! The basic idea is this: an metachain Rollup chain runs as a sort of sub-module within Ethereum. Unlike regular, layer 1 ( “L1”) Ethereum transactions, we don’t require Ethereum nodes to process every metachain transaction; rather, Ethereum adopts an [“innocent until proven guilty"](https://insights.deribit.com/market-research/making-sense-of-rollups-part-2-dispute-resolution-on-metachain-and-optimism/) attitude to metachain. Layer 1 initially “optimistically assumes” activity on metachain is following the proper rules. If a violation occurs (i.e., somebody claims “now I have all of your money”), this claim can be disputed back on L1; fraud will be proven, the invalid claim disregarded, and the malicious party will be financially penalized.

This ability to adjudicate and prove fraud on L1 is metachain’s key, fundamental feature, and is how and why the system inherits Ethereum’s security.

#### Q: So we can use Ethereum to prove fraud on metachain; cool! But if fraud is committed, can we be absolutely sure that we'll be able to prove it?

Yes, indeed we can be. This is where the “rollup” part comes in. The data that gets fed into an metachain Rollup chain (i.e., user’s transaction data) is posted directly on Ethereum. Thus, as long as Ethereum itself is running securely, anybody who’s interested has visibility into what’s going on in metachain, and has the ability to detect and prove fraud.

#### Q: Who actually does this work (of checking for fraud, proving it, etc?)

The parties who move the metachain chain state forward on L1 — i.e., making claims about the chain’s state, disputing other’s claims, etc. — are called validators.
In practice, we don’t expect the average metachain user to be interested in running a
validator, just like the average Ethereum user typically doesn’t run their own layer 1 staking node. The crucial property, however, is that anybody can; becoming an metachain validator requires no special permission ([once the allowlist is lifted](https://docs.metachain.foundation/state-of-progressive-decentralization)), only that a user runs the [open source validator software](https://github.com/META-MetaChain/nitro) (and stakes Ether when/if they need to take action).

Additionally, as long as there’s even just one honest validator, the chain will remain secure; i.e., it only takes one non-malicious fraud-prover to catch any number of malicious trouble-makers. These properties together make the system “trustless”; users are not relying on any special designated party for their funds to be secure.

#### Q: And how exactly is “fraud” “proven”? Sounds complicated.

Oh, it’s not so bad. In essence: if two validators disagree, only one of them (at most) can be telling the truth. In a dispute, the two validators play an interactive, call-and-response game, in which they narrow down their dispute to a single computational step (think of something small and simple, like multiplying two numbers). This one step gets executed on L1, and will, by necessity, prove that the honest party was telling the truth. For a more detailed rundown, see [here](../proving/challenge-manager.mdx).

#### Q: This dispute game obviously takes some time; does this impose any sort of delay on metachain users' transactions?

The only delay that's felt by a user is in "withdrawing" — moving their funds from metachain back to Ethereum; if users are withdrawing directly from metachain to Ethereum, they must typically wait 1 week before receiving their funds on L1. If users use a fast-bridge application, however, they can bypass this delay period entirely (likely for a small fee). Anything else a user does — i.e., depositing funds from Ethereum onto metachain, or using a dapp deployed on an metachain chain — doesn't incur this delay period.

#### Q: Okay, so backing up: the “optimistic execution” part is how and why metachain is able to offer low fees, yes?

Primarily, yes, this is the heart of where the savings come from. However, there are a number of other means by which metachain alleviates the burden on L1, all of which translate to lower transaction costs for end users.
For one, metachain transactions are submitted on the L1 in batches; typically, a single batch (submitted in a single L1 transaction) will contain several hundred L2 transactions. Batching amortizes the overhead cost of interacting with the L1, and thus offers significant savings over posting individual transactions at a time. Furthermore, the transaction data is posted on L1 in compressed form (and only decompressed within the L2 environment), further minimizing the transaction’s L1 footprint.

#### Q: As far as the experience of using metachain: when you said that it’s very similar to using Ethereum…

We really meant it, yes.
Different layer 2 protocols emphasize and optimize for different things; metachain was created with Ethereum compatibility as a top priority. This means users can use metachain with all their favorite Ethereum wallets; developers can build and deploy contracts with all their favorite Ethereum libraries and tooling; in fact, most of the time, the experience of using metachain will feel identical to that of using Ethereum (with the important exception of it being much cheaper and faster).

Much development went into achieving this level of Ethereum compatibility. But at its core: the metachain itself uses a fork of [Geth](../METAos/geth.mdx) — the most widely used Ethereum implementation — with modifications to transform it into a trustless layer 2. This means most of the code running in metachain is identical to the code running in Ethereum. We call this cutting-edge approach Nitro (developers can see the codebase [here](https://github.com/META-MetaChain/nitro)).

#### Q: So builders can do all the stuff they do on Ethereum on metachain, nice! But can they do _more_?

They can; the latest version of the metachain tech stack, called <a data-quicklook-from='stylus'>Stylus</a>, keeps Nitro's Ethereum compatibility, while adding on powerful new features, namely the ability to write highly performant smart contracts in programming languages like Rust, C++, and more. Stylus is currently on public testnet; you can read more about it [here](../stylus/stylus-gentle-introduction.md).

#### Q: So it sounds like metachain Rollup is an ideal solution that solves any and all scaling problems…?

metachain Rollup is very awesome and cool; its design is geared heavily toward avoidance of introducing any centralization or trust assumptions, and it is thus a clear, strict net-win for the Ethereum ecosystem. Decentralization, however, comes at a (literal) price, and not all applications and users necessarily want or need to pay that price. For dapp use-cases with different security considerations, different tools in the metachain suite are appropriate; i.e., metachain AnyTrust chains!

#### Q: What’s an AnyTrust chain?

An metachain AnyTrust chain doesn’t have the same decentralization / trustlessness / permissionless security guarantees of a Rollup chain, and thus can offer lower fees. Rollup and AnyTrust are similar in many ways, though have one key difference: whereas in Rollup, all data is posted on L1 (which allows anyone to permissionless join as a validator), in AnyTrust, data is managed off-chain. In the case of a challenge, an AnyTrust chain reverts back to “rollup mode”; the security assumption here is that at least 2 of the committee members are honest (i.e., they will provide the data when it’s necessary). Keeping the data off-chain in the happy/common case means the system can charge the user significantly lower fees.
For applications that require high transaction throughput and don’t require the full decentralization that rollups provide, AnyTrust could be a sensible tradeoff.

#### Q: So there's more than one metachain chain out there?

Yep! The fact that multiple chains can run in parallel is a crucial perk to off-chain scaling technology. Currently, on Ethereum mainnet, there are 2 metachain chains: one metachain Rollup chain, called ["metachain One,"](https://portal.metachain.one/) and one AnyTrust chain, called ["Nova"](https://nova.metachain-i.co/); users and developers can pick whatever suits their security / transaction cost needs.

Developers also have the option of launching their own metachain chains that run top an metachain layer 2. These are called <a data-quicklook-from='metachain-orbit'>Orbit</a> chains and you can read more about them [here](../launch-orbit-chain/orbit-gentle-introduction.md).

#### Q: Who makes decisions about the future of metachain One and metachain Nova?

The metachain One and Nova chains are owned by the Governance system; to learn more, see the [metachain Governance docs](https://docs.metachain.foundation/).

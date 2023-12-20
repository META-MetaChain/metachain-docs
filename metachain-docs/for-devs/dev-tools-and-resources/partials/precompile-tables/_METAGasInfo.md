<table>
  <thead>
    <tr>
      <th>Method</th>
      <th>Solidity interface</th>
      <th>Go implementation</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code>getPricesInWeiWithAggregator(address aggregator)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L22"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L26"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetPricesInWeiWithAggregator gets prices in wei when using the provided aggregator</td>
    </tr>
    <tr>
      <td>
        <code>getPricesInWei()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L44"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L91"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetPricesInWei gets prices in wei when using the caller's preferred aggregator</td>
    </tr>
    <tr>
      <td>
        <code>getPricesInMETAGasWithAggregator(address aggregator)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L58"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L96"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        GetPricesInMETAGasWithAggregator gets prices in METAGas when using the provided aggregator
      </td>
    </tr>
    <tr>
      <td>
        <code>getPricesInMETAGas()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L69"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L138"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetPricesInMETAGas gets prices in METAGas when using the caller's preferred aggregator</td>
    </tr>
    <tr>
      <td>
        <code>getGasAccountingParams()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L80"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L143"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetGasAccountingParams gets the rollup's speed limit, pool size, and tx gas limit</td>
    </tr>
    <tr>
      <td>
        <code>getMinimumGasPrice()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L90"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L151"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetMinimumGasPrice gets the minimum gas price needed for a transaction to succeed</td>
    </tr>
    <tr>
      <td>
        <code>getL1BaseFeeEstimate()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L93"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L156"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetL1BaseFeeEstimate gets the current estimate of the L1 basefee</td>
    </tr>
    <tr>
      <td>
        <code>getL1BaseFeeEstimateInertia()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L96"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L161"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        GetL1BaseFeeEstimateInertia gets how slowly METAOS updates its estimate of the L1 basefee
      </td>
    </tr>
    <tr>
      <td>
        <code>getL1RewardRate()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L100"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L166"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetL1RewardRate gets the L1 pricer reward rate</td>
    </tr>
    <tr>
      <td>
        <code>getL1RewardRecipient()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L104"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L171"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetL1RewardRecipient gets the L1 pricer reward recipient</td>
    </tr>
    <tr>
      <td>
        <code>getL1GasPriceEstimate()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L107"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L176"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetL1GasPriceEstimate gets the current estimate of the L1 basefee</td>
    </tr>
    <tr>
      <td>
        <code>getCurrentTxL1GasFees()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L110"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L181"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetCurrentTxL1GasFees gets the fee paid to the aggregator for posting this tx</td>
    </tr>
    <tr>
      <td>
        <code>getGasBacklog()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L113"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L186"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetGasBacklog gets the backlogged amount of gas burnt in excess of the speed limit</td>
    </tr>
    <tr>
      <td>
        <code>getPricingInertia()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L116"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L191"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>GetPricingInertia gets the L2 basefee in response to backlogged gas</td>
    </tr>
    <tr>
      <td>
        <code>getGasBacklogTolerance()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L119"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L196"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        GetGasBacklogTolerance gets the forgivable amount of backlogged gas METAOS will ignore when
        raising the basefee
      </td>
    </tr>
    <tr>
      <td>
        <code>getL1PricingSurplus()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L122"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L200"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Returns the surplus of funds for L1 batch posting payments (may be negative)</td>
    </tr>
    <tr>
      <td>
        <code>getPerBatchGasCharge()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L125"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L236"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        Returns the base charge (in L1 gas) attributed to each data batch in the calldata pricer
      </td>
    </tr>
    <tr>
      <td>
        <code>getAmortizedCostCapBips()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L128"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L240"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Returns the cost amortization cap in basis points</td>
    </tr>
    <tr>
      <td>
        <code>getL1FeesAvailable()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAGasInfo.sol#L131"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAGasInfo.go#L244"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Returns the available funds from L1 fees</td>
    </tr>
  </tbody>
</table>
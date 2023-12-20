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
        <code>becomeChainOwner()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L13"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L55"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Caller becomes a chain owner</td>
    </tr>
    <tr>
      <td>
        <code>events(bool flag, bytes32 value)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L16"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L27"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Emit events with values based on the args provided</td>
    </tr>
    <tr>
      <td>
        <code>eventsView()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L19"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L45"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Tries (and fails) to emit logs in a view context</td>
    </tr>
    <tr>
      <td>
        <code>customRevert(uint64 number)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L38"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L50"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Throws a custom error</td>
    </tr>
    <tr>
      <td>
        <code>legacyError()</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L40"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L59"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Throws a hardcoded error</td>
    </tr>
  </tbody>
</table>
<table>
  <thead>
    <tr>
      <th>Event</th>
      <th>Solidity interface</th>
      <th>Go implementation</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code>Basic</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L22"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L32"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        Emitted in <code>Events</code> for testing
      </td>
    </tr>
    <tr>
      <td>
        <code>Mixed</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L23"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L37"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>
        Emitted in <code>Events</code> for testing
      </td>
    </tr>
    <tr>
      <td>
        <code>Store</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METADebug.sol#L30"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METADebug.go#L0"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Never emitted (used for testing log sizes)</td>
    </tr>
  </tbody>
</table>
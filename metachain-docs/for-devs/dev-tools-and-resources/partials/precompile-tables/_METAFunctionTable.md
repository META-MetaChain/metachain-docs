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
        <code>upload(bytes calldata buf)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAFunctionTable.sol#L15"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAFunctionTable.go#L19"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Upload does nothing</td>
    </tr>
    <tr>
      <td>
        <code>size(address addr)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAFunctionTable.sol#L18"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAFunctionTable.go#L24"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Size returns the empty table's size, which is 0</td>
    </tr>
    <tr>
      <td>
        <code>get(address addr, uint256 index)</code>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro-contracts/blob/b16bf0b737468382854dac28346fec8b65b55989/src/precompiles/METAFunctionTable.sol#L21"
          target="_blank"
        >
          Interface
        </a>
      </td>
      <td>
        <a
          href="https://github.com/META-MetaChain/nitro/blob/v2.1.3/precompiles/METAFunctionTable.go#L29"
          target="_blank"
        >
          Implementation
        </a>
      </td>
      <td>Get reverts since the table is empty</td>
    </tr>
  </tbody>
</table>

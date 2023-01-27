### Nonced execution

Send a message from source-chain to destination-chain.

Deploy:

```bash
npm run deploy evm/nonced-execution [local|testnet]
```

Run the test:

```bash
npm run execute evm/nonced-execution [local|testnet] ${srcChain} ${destChain} ${message}
```

**Default Values**:

-   `srcChain` is `Avalanche`. Valid values are Moonbeam, Avalanche, Fantom, Ethereum, and Polygon
-   `destChain` is `Fantom`. Valid values are Moonbeam, Avalanche, Fantom, Ethereum, and Polygon
-   `message` is `Hello World`

#### Example

```bash
npm run deploy evm/nonced-execution local
npm run execute evm/nonced-execution local ${} ${} ${}
```

Output:

```
--- Initially ---
Last message sent from Avalanche@0xBa86A5719722B02a5D5e388999C25f3333c7A9fb to Fantom was "" with a nonce of -1.
--- After ---
Last message sent from Avalanche@0xBa86A5719722B02a5D5e388999C25f3333c7A9fb to Fantom was "Hello, the time is 1654191658288." with a nonce of 0.
```
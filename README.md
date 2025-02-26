# **cns2addr** #

cns2addr (Chain Naming Service to Address) is a multi-chain name resolver that maps human-readable blockchain names to their respective wallet addresses across different blockchain ecosystems. It supports Ethereum Name Service (ENS), Solana Name Service (SNS), and other chain-specific naming conventions.

## Features

- 🔗 Multi-Chain Support – Resolve names from multiple blockchain naming services.

- ⚡ Fast & Lightweight – Designed for efficiency with minimal overhead.

- 🛠 Easy Integration – Use it in any JavaScript/TypeScript project via npm.

- 🔍 Custom Resolver – Extend functionality with custom chain integrations.

## Installation
 To add cns2addr to your nodejs project run:
 ```bash
 npm install cns2addr
 ```

## Usage
 Example usage:
 ```ts
 import { resolveName } from 'cns2addr';

 (async () => {
    const address = await resolveName('vitalik.eth');
    console.log(address); // 0x1234...abcd
 })();
 ```

## Supported Naming Services

- Ethereum Name Service (ENS) – *.eth
- Solana Name Service (SNS) – *.sol
- Many are coming soon.

## API Reference
 ```ts
 resolveName(name: string): Promise<string | null>
 ```
Resolves a blockchain name to a wallet address.

Parameters:
- name (string) – The human-readable blockchain name (e.g., vitalik.eth).

Returns:
- A Promise resolving to the corresponding wallet address or null if not found.

## Contributing

We welcome contributions! Feel free to submit issues, feature requests, or pull requests.

## License

Apache-2.0 License
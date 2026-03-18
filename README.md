# @ai-agent-economy/plugin-agent-wallet

ElizaOS plugin providing non-custodial wallet capabilities for AI agents, powered by [agent-wallet-sdk](https://www.npmjs.com/package/agent-wallet-sdk).

## Features

- **Multi-chain wallets** -- Create and manage wallets on 17 chains (Base, Ethereum, Solana, Polygon, Arbitrum, Optimism, BNB, Avalanche, and more)
- **x402 payments** -- Native support for the x402 payment protocol (Coinbase/Google standard)
- **On-chain identity** -- ERC-8004 agent identity binding with ERC-6551 token-bound accounts
- **Reputation** -- On-chain reputation scoring for agent trust
- **Non-custodial** -- Agents hold their own keys. No custodian, no counterparty risk.

## Installation

```bash
npx elizaos plugins add @ai-agent-economy/plugin-agent-wallet
```

Or manually:
```bash
npm install @ai-agent-economy/plugin-agent-wallet agent-wallet-sdk
```

## Actions

| Action | Description |
|--------|-------------|
| `CREATE_WALLET` | Create a new wallet on any supported chain |
| `CHECK_BALANCE` | Check wallet balance |
| `SEND_PAYMENT` | Send payment via x402 or direct transfer |
| `GET_IDENTITY` | Retrieve or create on-chain agent identity |

## Provider

The `walletProvider` injects wallet status context into agent conversations, including chain support, x402 status, and identity information.

## Evaluator

The `paymentEvaluator` detects payment intents in user messages and triggers x402 payment flows automatically.

## Quick Start

```typescript
import agentWalletPlugin from '@ai-agent-economy/plugin-agent-wallet';

// Add to your ElizaOS agent configuration
const agent = {
  plugins: [agentWalletPlugin],
  // ... other config
};
```

## Supported Chains

Base, Ethereum, Solana, Polygon, Arbitrum, Optimism, BNB Chain, Avalanche, Fantom, Gnosis, Celo, Moonbeam, zkSync Era, Scroll, Linea, Mantle, Blast

## Links

- [agent-wallet-sdk on npm](https://www.npmjs.com/package/agent-wallet-sdk)
- [GitHub](https://github.com/up2itnow0822/agent-wallet-sdk)
- [x402 Protocol](https://x402.org)
- [AI Agent Economy](https://ai-agent-economy.hashnode.dev)

## License

MIT

> *This plugin was created with AI assistance and is maintained by AI Agent Economy.*

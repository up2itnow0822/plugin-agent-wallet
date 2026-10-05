# Changelog

## [Unreleased]

### Fixed
- Public npm links, homepage, and install instructions now use `agentwallet-sdk` (`agent-wallet-sdk` 404s on npm).
- Runtime CHECK_BALANCE / SEND_PAYMENT / GET_IDENTITY guidance now names `agentwallet-sdk`.

## [1.0.0] - 2026-03-23

### Added
- Initial release of ElizaOS plugin-agent-wallet
- Multi-chain wallet support (17 chains: Base, Ethereum, Solana, Polygon, Arbitrum, Optimism, BNB, Avalanche, +9)
- x402 payment protocol integration
- On-chain agent identity (ERC-8004 + ERC-6551)
- Reputation scoring system
- Non-custodial key management

### Fixed
- Updated ActionExample type to use `name` field (ElizaOS v1.0.0 API)
- Updated Handler signature to match ElizaOS v1.0.0 types
- Updated Provider return type to ProviderResult
- Updated EvaluationExample to use `prompt` field
- Fixed dependency: agent-wallet-sdk → agentwallet-sdk (published on npm)

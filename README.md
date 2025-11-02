README.md (for PredictionChain)
# PredictionChain  
An evolving blockchain protocol for prediction markets and futarchy.

![Rust](https://img.shields.io/badge/language-Rust-000000?style=flat)  
![Codecov](https://img.shields.io/codecov/c/github/your-org/predictionchain?style=flat)  
![Discord](https://img.shields.io/badge/Discord-community-7289da?style=flat)  
![Telegram](https://img.shields.io/badge/Telegram-chat-2ca5e0?style=flat)  
![X](https://img.shields.io/badge/X-(@YourHandle)-1da1f2?style=flat)  
![Pull Request Reviews](https://img.shields.io/badge/PR-reviews-enabled-green?style=flat)

PredictionChain is a decentralized network for creating, trading, and resolving prediction markets — enabling users to build sophisticated financial contracts on virtually any outcome. Its native token (e.g., **PCN**) is used to influence network governance, and serves as a final-call dispute resolution mechanism in the on-chain court.

---

## Modules  
- `authorized` — Provides authorized dispute resolution.  
- `combinatorial-tokens` — Generates outcome tokens for combinatorial markets.  
- `court` — Decentralised court for dispute resolution.  
- `futarchy` — On-chain governance via prediction markets.  
- `global-disputes` — If the court fails, the outcome with the highest locked tokens becomes canonical.  
- `macros` — Shared macros used across modules.  
- `market-commons` — Shared market logic.  
- `neo-swaps` — Implements the Logarithmic Market Scoring Rule (LMSR) CFMM for combinatorial markets and futarchy.  
- `orderbook` — Classic orderbook implementation.  
- `parimutuel` — Simple parimutuel market maker for categorical markets.  
- `prediction-markets` — Core logic for market creation, trading, and settlement.  
- `swaps` — Implements a Balancer-style CFMM allowing liquidity pools, swaps and assets.  
- `primitives` — Core types, traits, constants used globally.

---

## Building & Running a Node  
PredictionChain supports two deployment modes: a **standalone node** for development/testing, and a **parachain mode** (for integration into a larger ecosystem).

### Standalone (for testing)  
From the project root:  
```bash
cargo build --release


This uses the runtime defined under runtimes/dev-station, and by default runs in --dev mode.

Parachain Mode
cargo build --features parachain --release


By default this connects to the mainnet.
To run against the testnet (e.g., “DevStation”), use:

cargo run --features parachain --release -- --chain=dev-station

Docker

We publish images on Docker Hub for both modes:

Parachain: docker pull yourorg/predictionchain-node-parachain

Standalone: docker pull yourorg/predictionchain-node

Run the standalone (for testing):

docker run yourorg/predictionchain-node -- <node-options-and-flags>

About

PredictionChain provides a foundation for decentralized prediction markets and futarchy governance. By combining financial markets with governance and dispute resolution, it enables stakeholders to trade on outcomes and influence protocol decisions — bridging collective intelligence and on-chain decision logic.

Contributing

See CONTRIBUTING.md for guidelines on contributing, submitting pull requests, and review process.

License

Licensed under the GNU GPL v3.0.


---

If you like, I can **generate several more name options** (and maybe help pick a nice logo/icon) so you can choose the best fit for your project. Would you like that?
::contentReference[oaicite:1]{index=1}

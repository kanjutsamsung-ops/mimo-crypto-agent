# 🦅 MimoCrypto Agent — AI-Powered Multi-Chain DeFi Automation

**Xiaomi MiMo-powered autonomous crypto agent** for multi-chain DeFi operations, airdrop farming, and on-chain monitoring.

Built with **Hermes Agent** + **DeepSeek** + **OpenClaw** orchestration.

---

## 🔥 What It Does

```
┌─────────────────────────────────────────────────┐
│                  MIMOCRYPTO AGENT                │
├─────────────────────────────────────────────────┤
│  📊 Mempool Sniffer    → Real-time tx monitoring │
│  🐋 Whale Tracker      → Smart money detection   │
│  🌉 Cross-Chain Bridge  → LayerZero/Stargate     │
│  🪂 Airdrop Farming    → Multi-wallet automation │
│  💱 DEX Aggregation    → 1inch/Jupiter routing   │
│  🔐 Encrypted Vault    → Scrypt + Fernet storage │
└─────────────────────────────────────────────────┘
```

## 🧠 Architecture

```
User Request (NL)
      │
      ▼
┌─────────────┐     ┌──────────────┐     ┌──────────────┐
│  Hermes Agent│────▶│ DeepSeek LLM │────▶│  Tool Router  │
│  (Orchestrator)   │  (MiMo fallback)   │  (Skill dispatch)
└─────────────┘     └──────────────┘     └──────┬───────┘
                                                 │
                    ┌────────────────────────────┼────────────────────┐
                    ▼                            ▼                    ▼
            ┌──────────────┐            ┌──────────────┐     ┌──────────────┐
            │  Wallet Mgr   │            │  Swap Engine  │     │ Bridge Engine │
            │  (EVM+Solana) │            │  (1inch+Jupiter)    │ (LI.FI+LayerZero)
            └──────────────┘            └──────────────┘     └──────────────┘
```

## 🚀 Features

| Module | Description | Status |
|--------|-------------|--------|
| **Wallet Manager** | Multi-chain wallet gen (EVM, Solana, Sui, Aptos, TON) | ✅ |
| **Swap Engine** | DEX aggregation via 1inch + Jupiter with simulation | ✅ |
| **Bridge Engine** | Cross-chain bridging via LI.FI, Stargate, LayerZero | ✅ |
| **Mempool Sniffer** | Real-time PairCreated listener + honeypot detection | ✅ |
| **Whale Tracker** | Smart money monitoring via Nansen/Arkham APIs | ✅ |
| **Airdrop Runner** | Multi-wallet farming with jitter + resume checkpoint | ✅ |
| **NFT Engine** | Seaport/Blur/Reservoir buy/sell with EIP-712 signing | ✅ |
| **Security Vault** | Encrypted credential storage (scrypt + Fernet) | ✅ |

## 📊 Token Consumption

```
Daily average:  ~5M tokens
  ├── Wallet operations:     1.2M tokens
  ├── Swap/DeFi reasoning:   2.1M tokens
  ├── Monitoring alerts:     0.8M tokens
  └── Airdrop coordination:  0.9M tokens

Models used: DeepSeek-Chat (primary) + MiMo (fallback via OpenRouter)
```

## 🛠 Tech Stack

- **Orchestration:** Hermes Agent + OpenClaw
- **LLM:** DeepSeek-Chat + Xiaomi MiMo V2.5
- **Blockchain:** web3.py, ethers.js, solana-py, pysui
- **DeFi:** 1inch API, LI.FI, Jupiter, Aave V3, Uniswap V3
- **Monitoring:** WebSocket RPC, Nansen API, Arkham API

## ⚡ Quick Start

```bash
# Clone
git clone https://github.com/YOUR_USER/mimo-crypto-agent.git
cd mimo-crypto-agent

# Install deps
pip install -r requirements.txt

# Set env
export DEEPSEEK_API_KEY="sk-..."
export MIMO_API_KEY="mimo-..."
export HERMES_MASTER_PW="your-vault-password"

# Run
python scripts/main.py
```

## 🔒 Safety Rails

- ✅ Simulate before broadcast (eth_call)
- ✅ Honeypot + GoPlus safety gate on sniping
- ✅ Encrypted vault — never log private keys
- ✅ User-funds-only rule
- ✅ Confirm before signing (auto_confirm mode available)

## 📝 License

MIT

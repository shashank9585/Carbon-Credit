# 🌍 Carbon Provenance Registry

[![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)](https://soliditylang.org/)
[![Hardhat](https://img.shields.io/badge/Hardhat-FFF100?style=for-the-badge&logo=ethereum&logoColor=black)](https://hardhat.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![QIE EVM](https://img.shields.io/badge/QIE_EVM-Testnet-blue?style=for-the-badge)](https://qie.io/)

> **A blockchain-based registry protocol that bridges digital carbon credits with physical biological assets through verifiable provenance, transparent ownership, and adaptive lifecycle management.**

---

## 🌱 Overview

**Carbon Provenance Registry** is a smart contract protocol built on the **QIE EVM Testnet** that addresses one of the biggest challenges in the voluntary carbon market (VCM): ensuring that digital carbon credits accurately represent real-world carbon storage.

Instead of treating carbon credits as static digital assets, this protocol models them as **digital twins** of physical biological assets. Every credit maintains its identity, ownership history, and lifecycle from issuance to retirement while allowing legitimate updates when real-world environmental conditions change.

---

# ✨ Key Highlights

- 🌍 Anchors every carbon credit to a unique physical land identity
- 🔒 Immutable ownership history for complete traceability
- 🌱 Supports dynamic utility updates when physical assets change
- ♻️ Permanent retirement mechanism preventing double usage
- 📜 Transparent on-chain audit trail
- ⚡ Built and deployed on the QIE EVM Testnet
- 🏗️ Designed for future decentralized carbon marketplaces

---

# 📖 The Problem

Today's voluntary carbon market faces several critical issues.

### 👻 Ghost Credits

Carbon credits can sometimes be issued for projects that either do not exist or cannot adequately prove long-term carbon capture.

### 🔁 Double Counting

The same carbon reduction may be sold multiple times due to fragmented registries and disconnected verification systems.

### 📉 Static Utility

Traditional registries assume that carbon storage never changes.

In reality:

- storms destroy forests
- disease affects plantations
- fires reduce biomass
- environmental conditions change over time

Digital records should evolve when the physical world changes.

---

# 💡 Project Philosophy

The protocol follows one simple principle:

> **A digital carbon credit should behave as a Digital Twin of the physical asset it represents.**

If the underlying biological asset changes, the blockchain record should accurately reflect that change while maintaining a complete and immutable audit history.

This approach improves transparency, accountability, and long-term trust within carbon markets.

---

# 🏗️ Protocol Architecture

The registry is built around four lifecycle stages.

---

## 1️⃣ Physical Anchor (Birth)

Every carbon credit begins with a unique identity.

Each issued credit includes:

- Land Identifier (`landId`)
- Vintage Year
- Carbon Quantity
- Evidence Link (`dataLink`)
- Original Researcher

This permanently connects the digital asset to a specific physical location and supporting documentation.

---

## 2️⃣ Chain of Custody (Ownership)

Every ownership transfer is permanently recorded.

The protocol maintains an immutable ownership history that allows anyone to verify:

- Original issuer
- Current owner
- Previous owners
- Complete transfer history

This significantly improves transparency and helps reduce fraudulent ownership claims.

---

## 3️⃣ Adaptive Utility

Unlike conventional registries, this protocol allows controlled updates when verified environmental changes occur.

For example:

- A cyclone destroys 20% of a plantation.
- Disease affects tree survival.
- Carbon storage decreases.

Authorized researchers can update the carbon utility using the `updateUtility()` function.

This helps keep the on-chain representation aligned with real-world conditions while preserving historical records.

---

## 4️⃣ Retirement (Finality)

Once a company uses a carbon credit to offset emissions, it should never circulate again.

Calling the `retireCredit()` function permanently retires the asset.

The record remains publicly visible for auditing purposes but can no longer be transferred or reused.

---

# 🔄 Smart Contract Workflow

```text
Researcher
     │
     ▼
Create Carbon Credit
     │
     ▼
Store Physical Identity
     │
     ▼
Transfer Ownership
     │
     ▼
Update Utility (when required)
     │
     ▼
Retire Credit
     │
     ▼
Permanent On-chain Audit Record
```

---

# 🌐 Ecosystem Integration

The protocol is designed to integrate with the broader **QIE ecosystem**.

Future integrations may include:

- Tokenization of verified carbon assets
- Fractional ownership models
- Decentralized marketplace support (QIEDEX)
- Transparent carbon asset discovery
- Verifiable trading infrastructure

> **Note:** These integrations represent the intended ecosystem direction and are not fully implemented within the current prototype.

---

# 🚀 Features

- ✅ Carbon Credit Issuance
- ✅ Physical Land Anchoring
- ✅ Immutable Ownership History
- ✅ Adaptive Carbon Utility Updates
- ✅ Retirement Mechanism
- ✅ Transparent Audit Trail
- ✅ Solidity Smart Contract Architecture
- ✅ QIE EVM Deployment

---

# 🛠️ Technical Specifications

| Category | Details |
|----------|---------|
| Language | Solidity ^0.8.x |
| Framework | Hardhat |
| Network | QIE EVM Testnet |
| Contract Type | Carbon Credit Registry |
| License | MIT *(Update if different)* |

---

# 📂 Project Structure

```text
Carbon-Credit/
│
├── contracts/
│   └── CarbonProvenance.sol
│
├── scripts/
│   └── deploy.ts
│
├── test/
│   └── CarbonProvenance.test.ts
│
├── artifacts/
│
├── ignition/
│
├── cache/
│
├── hardhat.config.ts
│
├── package.json
│
└── README.md
```

---

# 📜 Core Smart Contract Functions

| Function | Description |
|----------|-------------|
| `createCredit()` | Creates and registers a new carbon credit |
| `transferCredit()` | Transfers ownership between parties |
| `updateUtility()` | Updates carbon utility after verified environmental changes |
| `retireCredit()` | Permanently retires a carbon credit |
| `viewFullDetails()` | Retrieves complete credit information |

---

# 🚀 Deployment

**Network**

QIE EVM Testnet

**Contract Address**

```text
0xfe8ff193e03a4aa90dec0a73714d9d7d5a66fdd9
```

> You can also add the QIE block explorer link here if publicly available.

---

# 💻 Getting Started

## Clone the Repository

```bash
git clone https://github.com/shashank9585/Carbon-Credit.git

cd Carbon-Credit
```

---

## Install Dependencies

```bash
npm install
```

---

## Compile Contracts

```bash
npx hardhat compile
```

---

## Run Tests

```bash
npx hardhat test
```

---

## Deploy

```bash
npx hardhat run scripts/deploy.ts --network qieTestnet
```

*(Update the deployment command if your project uses a different deployment script.)*

---

# 📸 Screenshots

You can further improve this repository by adding:

- Smart contract deployment screenshot
- QIE Explorer transaction
- Contract interaction
- Test results
- Architecture diagram

Example:

```text
docs/
├── architecture.png
├── deployment.png
├── explorer.png
└── workflow.png
```

---

# 🔮 Future Improvements

- NFT-based carbon certificates
- Oracle integration for automated environmental updates
- Satellite imagery verification
- Multi-signature verification workflow
- DAO-based researcher governance
- IPFS integration for immutable evidence storage
- Carbon marketplace dashboard
- Cross-chain interoperability

---

# 🤝 Contributing

Contributions, discussions, and suggestions are welcome.

If you'd like to improve the protocol, feel free to fork the repository, open issues, or submit pull requests.

---

# 📄 License

This project is licensed under the **MIT License**.

*(Update this section if your repository uses another license.)*

---

# 👨‍💻 Author

**Shashank H E**

GitHub:
https://github.com/shashank9585

---

# 🌍 Vision

The future of carbon markets depends on trust.

Trust begins with identity.

By anchoring every digital carbon credit to verifiable physical evidence and maintaining a transparent lifecycle on-chain, this project aims to demonstrate how blockchain can improve accountability, traceability, and confidence in climate-focused digital assets.

> **Building transparent infrastructure for a more trustworthy carbon economy.**

QIE Carbon Provenance: The Physical-Anchor Registry (PH2)
CarbonProvenance is a blockchain-based registry protocol designed to bridge the gap between digital carbon credits and physical biological assets. Built on the QIE Ledger, it provides a verifiable "Handshake" mechanism that secures the entire lifecycle of a carbon credit—from its birth in a coconut grove to its final retirement as an offset.

📖 The Problem & The Philosophy
The current voluntary carbon market (VCM) is plagued by three core failures:

Ghost Credits: Selling credits for land that doesn't exist or isn't actually capturing carbon.

Double-Counting: Selling the same ton of carbon to multiple buyers because of fragmented registries.

Static Utility: Credits are often "issued and forgotten," ignoring the fact that a storm or disease can physically destroy the trees meant to store the carbon.

Our Philosophy: A digital credit should be a "Digital Twin" of the physical world. If the physical asset changes, the digital credit must adapt.

🛠️ The Framework: How It Works
This protocol implements four unique architectural layers to ensure "Provenance" (the record of origin and ownership).

1. The Physical Anchor (Birth)
Every credit is uniquely identified by a landId and a vintage year. Unlike generic tokens, this protocol anchors the data to:

Geospatial Identity: The specific plot of land (e.g., UK-COCO-01).

Evidence Links: A permanent pointer (dataLink) to the underlying research or legal land deed.

2. The Chain of Custody (Handshake)
To prevent "Carbon Laundering," the contract maintains an internal ownerHistory array. This is an immutable audit trail that tracks every single address that has ever held the asset.

Transparency: Any buyer can verify the credit's entire history back to the original researcher.

3. Adaptive Utility (The Accident Clause)
This is the protocol’s most innovative feature. Through the updateUtility function, the registry allows for Honest Downscaling.

Mechanism: If 20% of a coconut grove is lost to a storm, the researcher can adjust the tons value on-chain.

Integrity: This ensures that the global supply of carbon credits on the QIE network always matches the actual carbon stored in the ground.

4. Tombstone Finality (Death)
When a company uses a credit to offset their footprint, it is "Retired."

Logic: The retireCredit function triggers a permanent lock state. The credit remains visible for audit purposes but can never be transferred or traded again.

💰 Ecosystem Integration: QIEDEX
The protocol is architected for the QIE Decentralized Exchange (QIEDEX). By utilizing the linkToQIEDEX interface, these high-integrity registry assets can be:

Fractionalized: Represented as QIE-20 tokens for retail trading.

Liquid: Listed on QIEDEX to allow instant price discovery for verified green assets.

🚀 Technical Specifications
Language: Solidity ^0.8.0

Infrastructure: QIE EVM (Testnet)

Contract Address: 0xfe8ff193e03a4aa90dec0a73714d9d7d5a66fdd9

Key Functions:

createCredit: Primary issuance by verified researchers.

transferCredit: Atomic owner-to-owner handshake.

updateUtility: Dynamic adjustment for physical asset loss.

viewFullDetails: Human-readable dashboard for transparency.

🤝 Contributing & Vision
This is an open-source prototype. We believe that Identity is Security. By securing the identity of the land, we secure the future of the climate.

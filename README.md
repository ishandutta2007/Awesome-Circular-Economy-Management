# Awesome-Circular-Economy-Management

# Top Circular Economy Management Platform Ecosystem

**Curated list of SaaS products and open-source GitHub projects**

*Focusing on circular supply chains, reverse logistics, Digital Product Passports (DPP), and resale markets*

**Last Updated: September 2026**

Language: **English** | [中文 (Chinese)](README_zh-CN.md)

This repository tracks leading **SaaS platforms** and **open-source projects** in the field of **circular economy management**. These tools help enterprises manage product lifecycles, optimize reverse logistics, achieve supply chain traceability, and comply with Digital Product Passport (DPP) regulations.

**Examples** include Circularise, Worldly, EON, Optoro, ReverseLogix, Loop Returns, Reflaunt, Cycle Platform, Trace For Good, and Reconomy (leaders in this space).

**Open Source Focus**: The open-source ecosystem for circular economy is **rapidly maturing**. **RELOG** (Argonne National Laboratory) provides MILP optimization for reverse logistics networks. **DPP01** is an open-source DPP framework for food producers. **open-dpp-registry** implements a URN-based blockchain product passport discovery mechanism. **Dolibarr Returns Modules** provide free reverse logistics workflows for SMEs. This list highlights these self-hostable, production-ready solutions.

Contributions are welcome! Submit a PR to add/update entries. Keep descriptions factual and link to official websites.

## Table of Contents

- [SaaS / Hosted Platforms](#saas--hosted-platforms)
- [Open Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS / Hosted Platforms

| Product | Description | Pricing & Free Tier Limits |
| :--- | :--- | :--- |
| **[Circularise](https://www.circularise.com/)** | Blockchain-based supply chain traceability and Digital Product Passport (DPP) platform. ISO 27001:2022 certified. Supports end-to-end tracking from raw materials to finished products. Proprietary selective data-sharing technology allows suppliers to protect confidential data while satisfying customer and regulatory requirements. Serves automotive, plastics, chemicals, and other industries. Customers include Porsche and Teijin. | **Custom Enterprise Pricing** (Contact sales for quote). No public free tier available. |
| **[EON](https://www.eon.xyz/)** | Enterprise Digital ID technology leader, creating serialized digital identities for products via **EON Product Cloud**. Partnered with Inspectorio to stream supply chain data directly into EON, helping brands transition from DPP pilots to scaled operations supporting millions of products. Jointly announced in September 2026, targeting retail and apparel brands. | **Custom Enterprise Pricing** (Tiered based on volume). No public free tier available. |
| **[Worldly](https://worldly.io/)** | Sustainability data platform, formerly Higg. Provides supply chain environmental and social impact measurement for apparel and consumer goods industries. | **Enterprise Subscription** (Based on supply chain scale). Free tier: Limited vendor portal access upon invitation. |
| **[Optoro](https://www.optoro.com/)** | Reverse logistics and returns management platform. Uses AI-driven disposition routing and value recovery optimization to help retailers maximize the value of returned goods. | **Custom Enterprise Pricing**. Demo available upon request; no public free tier. |
| **[ReverseLogix](https://www.reverselogix.com/)** | End-to-end reverse logistics management platform. Provides workflows for returns, repairs, recalls, and disposition. | **Custom Enterprise Pricing**. Free trial/demo upon request; no permanent free tier. |
| **[Loop Returns](https://loopreturns.com/)** | E-commerce returns management platform. Focused on the Shopify ecosystem, offering return portals, exchange incentives, and refund automation. | **Tiered SaaS Pricing** (Starting at ~$165/mo + usage fees). 14-day free trial available. |
| **[Reflaunt](https://www.reflaunt.com/)** | Resale and circular commerce platform. Helps fashion brands launch resale programs, connecting buyers and sellers. | **Enterprise / Revenue Share Model**. Contact for quote; no free tier available. |
| **[Cycle Platform](https://www.cycle.app/)** | Circular economy software platform. Manages deposit-refund systems for reusable packaging and containers. | **Custom Enterprise / Municipal Pricing**. No public free tier available. |
| **[Trace For Good](https://traceforgood.com/)** | Supply chain traceability platform. Provides product provenance, material tracking, and compliance reporting. | **Custom Enterprise Pricing**. Free demo available; no public free tier. |
| **[Reconomy](https://www.reconomy.com/)** | Circular economy service provider. Manages waste, resources, and compliance to offer end-to-end circular economy solutions for businesses. | **Custom Contracting / Enterprise Pricing**. No public free tier available. |

## Open Source GitHub Projects

### Digital Product Passports (DPP) & Traceability

- **[DPP01](https://github.com/arcticscihub/DPP01)**
  **Open-source DPP framework for food producers.** Provides data acquisition and organization platform supporting the creation and management of Digital Product Passports. Features include: structured digital record generation (material composition, sourcing, usage), EU DPP compliance support, value chain traceability and transparency, sustainability reporting data reuse, circularity, and resource management. Flexible deployment: contact repo owner for support, AWS DevOps deployment, or in-house team deployment. **Open Source**.

- **[open-dpp-registry](https://pkg.go.dev/git.nilu.no/ce-rise-is/utils/open-dpp-registry)**
  **URN-based blockchain product passport discovery registry.** Solves a key issue in the DPP ecosystem: how to discover who maintains a product's DPP. Uses RFC 8141 compliant slash-separated URN structure (`/lot/...`, `/serial/...`), supporting precise identification via GTIN14 + Lot + Serial number. Blockchain backends: In-memory, File, Ethereum. REST API endpoints include record discovery, record management, and blockchain operations. **Go 1.22+**. Supports product authentication, history tracking, and cross-provider continuity use cases.

- **[mycelix-supplychain](https://github.com/Luminous-Dynamics/mycelix-supplychain)**
  **Decentralized supply chain traceability system with Byzantine Fault Tolerant consensus.** Converts ERP/IoT events into signed DKG claims and portable Verifiable Credentials (VCs) with hash-linked lineage proofs. Features include: Event → VC → DKG claim pipeline, CSV/MQTT adapters, Validator UI + CLI, **Product Passport Export**, and selective disclosure (SD-JWT/BBS+ cryptography). Use cases: track-and-trace, compliance auditing, anti-counterfeiting, recall impact analysis. **Rust Core + TypeScript SDK**. **Apache-2.0**. Status: Alpha (Pilot Reference Implementation).

- **[TraceFlow](https://github.com/Cao150702/traceflow)**
  **Decentralized item traceability system providing blockchain-verified digital passports for physical goods.** Issues a unique ID + QR code + optional NFT passport for each product. Features include: item registration, movement tracking (on-chain for each handover), scan verification, **AI anomaly detection** (Rule Engine + GPT-4o-mini), and authenticity scoring. Tech stack: Next.js 14, Supabase, Polygon, ethers.js. Use cases: limited edition goods, specialty coffee, electronics anti-counterfeiting, secondary market ownership verification.

### Reverse Logistics & Returns Management

- **[RELOG](https://github.com/ANL-CEEESA/RELOG)**
  **Open-source reverse logistics optimization package developed by Argonne National Laboratory.** Uses Mixed-Integer Linear Programming (MILP) to assist users with strategic decision-making: locations and construction timing for manufacturing and recycling plants, plant capacities, expansion timing and scale, input material origins and output destinations per facility, and immediate processing vs. storage decisions. Successfully applied to critical material recycling (spent NiMH and lithium-ion batteries), biomass-to-hydrogen, electronics/plastics/solar PV recycling research. **Open Source**.

- **[Dolibarr Returns & RMA Modules](https://github.com/zacharymelo/doli-returns)**
  **Free reverse logistics module suite for SMEs.** Includes four synergistic modules: **Doli-Returns** (receives returns into stock, issues credits), **RMA/Warranty** (warranty and RMA tracking, auto-generates warranty records), **Customer Inventory** (customer purchased products and services view), **Box Label** (generates unique labels from MRP). V1.0.4 (released April 2026) fixed duplicate line and empty line bugs. **Free & Open Source**.

- **[ROBOSTAPLE](https://github.com/pacobaco/robostable)**
  **Distributed reverse logistics operating system**, turning homes into programmable inventory nodes coordinated by event-driven routing and AI demand forecasting. Early-stage project.

### Circular Commerce & Resale Markets

- **[Phoenix Project](https://github.com/The-PhoenixProject/The-Phoenix-Project-Front-end)**
  **Open-source secondary marketplace connecting eco-friendly buyers and sellers.** Supports recycling, upcycling, and reselling. Features: User registration/login, product browsing/creation/editing/deletion, social posts (likes/comments), Socket.IO real-time chat and notifications, file/image upload, eco-points. Tech stack: React, Socket.IO, JWT authentication. **ISC License**.

- **[openmagpie / AgentMarket](https://socket.dev/npm/package/openmagpie)**
  **AI agent-native secondary market framework.** Built for AI agents to automatically list, match, negotiate, and settle secondhand transactions. Core protocols: list, search, offer, settle. Pluggable matching engine (exact/fuzzy/LLM). Pluggable storage adapter (SQLite/PostgreSQL). Supports MCP Server and REST API. **npm package**, early version (v0.1.0).

- **[ZeroWaste](https://github.com/jessem8/zerowaste)**
  **Community circular economy platform.** Supports sharing upcycling projects, item swap marketplaces, and eco-community forums. Features: User management, community forums, shared swap platform (category filtering, Google Maps integration, messaging system), upcycling catalog (PDF export). Tech stack: PHP 7.4+, MySQL, Tailwind CSS, Alpine.js. Aligned with **UN SDG 12** (Responsible Consumption and Production). Educational use.

### Other Strong Open Source Options

- **Digital Product Passports**: **DPP01** (Food producers), **open-dpp-registry** (Blockchain discovery), **mycelix-supplychain** (Decentralized provenance), **TraceFlow** (AI risk analysis).
- **Reverse Logistics**: **RELOG** (MILP optimization), **Dolibarr Modules** (Free for SMEs), **ROBOSTAPLE** (Distributed OS).
- **Circular Commerce**: **Phoenix Project** (Secondhand marketplace), **openmagpie** (AI agent market), **ZeroWaste** (Community platform).

**Framework for Building Custom Systems**: Combine **DPP01** or **open-dpp-registry** for DPP generation and discovery, **RELOG** for reverse logistics network optimization, **Dolibarr Returns Modules** for SME reverse logistics workflows, and **Phoenix Project** or **ZeroWaste** for secondhand transaction platforms. Add **PostgreSQL** and **Blockchain** (Ethereum/Polygon) for traceability persistence.

## How to Contribute

1. Fork the repository.
2. Add/edit entries in `README.md` (following the existing format).
3. Include: Name, link, 1-2 sentence description, and whether it is SaaS or Open Source.
4. Submit a PR with a brief explanation.

If you find this repository useful, please give it a star!

## Disclaimer

- This is a **community-curated** list—it is not exhaustive and does not constitute an endorsement.
- Circular economy platforms handle supply chain and product data; ensure compliance with EU DPP regulations, ESPR, and relevant sustainability disclosure requirements.
- **Open Source Reality**: The open-source ecosystem for circular economy **is already usable** at the level of **DPP frameworks** (DPP01, open-dpp-registry) and **reverse logistics optimization** (RELOG), but full commercial circular economy platforms (Circularise, EON, Optoro) still hold significant advantages in **enterprise-grade supply chain integration**, **selective data sharing**, and **scaled deployment**. Open-source solutions are suitable for pilot projects and academic research, while production-grade deployments require substantial custom development.

---

**Built for sustainability managers, circular economy engineers, supply chain analysts, and reverse logistics teams.**

Making circular economy management more open, transparent, and traceable.

# vAuto (vauto)

vAuto is a [Cox Automotive](https://www.coxautoinc.com/brands/vauto/) brand providing new and used vehicle inventory management, appraisal, pricing, and merchandising software for automotive dealers (ProfitTime GPS, Provision, Conquest, Stockwave). vAuto exposes **partner-gated** APIs through the Cox Automotive Integration Platform ([developer.coxautoinc.com](https://developer.coxautoinc.com/)) - notably the **vAuto Inventory API** and the **vAuto Appraisal API** - that let authorized integrators programmatically read vehicle inventory, update list price, and create and access appraisals in the vAuto ecosystem.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vauto/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vauto/refs/heads/main/apis.yml)

## Access Model

Access is **not open self-service**. To use the vAuto APIs an integrator must:

1. Register / sign in with a Cox Automotive **Bridge ID**.
2. Request access through the Cox Automotive Integration Platform developer portal ([developer.coxautoinc.com](https://developer.coxautoinc.com/)).
3. Complete Cox Automotive **partner review and approval**.
4. Authenticate via **OAuth** and send an issued **`x-api-key`** on requests.

Endpoint-level reference documentation sits behind the partner developer portal login. Commercial terms are **contact-sales / negotiated** and are not published publicly. See [plans/vauto-plans-pricing.yml](plans/vauto-plans-pricing.yml).

> **Honesty note:** Because the per-endpoint reference is partner-gated, the individual endpoints referenced in this catalog entry are **modeled** from the published product summaries (see `endpointsModeled` in `apis.yml` and `review.yml`), not copied from public reference documentation. No full OpenAPI surface has been fabricated.

## Tags

- Automotive
- Dealership
- Inventory Management
- Appraisals
- Vehicle Pricing
- Cox Automotive
- Partner API

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs

### vAuto Inventory API

Partner-gated API that lets authorized integrators programmatically read vehicle information and update list price for inventory in the vAuto ecosystem. Listed as **vAuto Inventory API 1.x** on the Cox Automotive API status page (operational REST service).

- **Human URL:** [https://developer.coxautoinc.com/marketingcontent/exploreproducts](https://developer.coxautoinc.com/marketingcontent/exploreproducts)
- **Base URL:** `https://api.coxautoinc.com` (partner gateway; endpoints modeled)

#### Tags

- Inventory
- Vehicles
- Pricing

### vAuto Appraisal API

Partner-gated API that lets authorized integrators programmatically create and access vehicle appraisals in the vAuto ecosystem, powering trade-in and used-vehicle valuation workflows. Listed as **vAuto Appraisal API 1.x** on the Cox Automotive API status page (operational REST service).

- **Human URL:** [https://developer.coxautoinc.com/marketingcontent/exploreproducts](https://developer.coxautoinc.com/marketingcontent/exploreproducts)
- **Base URL:** `https://api.coxautoinc.com` (partner gateway; endpoints modeled)

#### Tags

- Appraisals
- Trade-In
- Valuation

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/vauto)
- [Website](https://www.vauto.com/)
- [Documentation](https://developer.coxautoinc.com/marketingcontent/exploreproducts)
- [Developer Portal](https://developer.coxautoinc.com/)
- [Status Page](https://coxautoapi.statuspage.io/)
- [Plans](plans/vauto-plans-pricing.yml)
- [Parent Company](https://www.coxautoinc.com/brands/vauto/)

## WebSocket Review

Does vAuto expose a documented public WebSocket API? **No.** vAuto's programmatic surface is partner-gated REST distributed through the Cox Automotive Integration Platform; no public WebSocket or SSE streaming endpoint is documented. See [review.yml](review.yml).

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

# vAuto (vauto)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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

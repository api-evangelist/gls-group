# GLS Group

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

GLS Group (General Logistics Systems B.V.) is a European ground-based parcel and freight carrier headquartered in Amsterdam-Duivendrecht, Netherlands, and owned by International Distributions Services plc. It operates a road network of more than 120 hubs and roughly 1,600 depots across some 50 countries in Europe, the United States and Canada, moving B2B and B2C parcels up to about 32 kg plus a freight/LTL and express line, with an out-of-home ParcelShop and locker network. In the supply chain it is a last-mile and middle-mile parcel integrator: the party a shipper, e-commerce platform or shipping-API aggregator hands a consignment to for pickup, linehaul, customs clearance and delivery. Its API posture is federated and contract-bound rather than unified. The GLS Group developer portal (dev-portal.gls-group.net, run by GLS IT Services GmbH on Apigee) allows self-serve account and app registration with API keys or OAuth 2.0, but its API catalog is only visible after sign-in and "restricted" APIs additionally require approval by a local GLS representative. National units run their own portals — GLS Netherlands publishes an Azure API Management portal at api-portal.gls.nl whose OpenAPI 3.0.1 definitions for the Label API and the Track & Trace API are anonymously readable, but calling them still requires MyGLS credentials issued to a contracted shipper. The group-wide GLS ShipIT REST/SOAP web services are fully documented in public Doxygen reference pages, yet the base URL itself is handed out only with credentials by a customer's primary GLS contact. No industry data standard — GS1/EPCIS, UPU, DCSA, IATA ONE Record, UN/EDIFACT or ANSI X12 — is referenced anywhere in the artifacts GLS publishes; every identifier and event vocabulary is GLS-proprietary.

**Areas:** Logistics · Supply Chain · Netherlands · Parcel · Shipping · Track and Trace · Freight · Last Mile Delivery · Europe · Customs

## GLS Group on APIs.io

Everything profiled for GLS Group is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/gls-group/](https://apis.io/providers/gls-group/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [GLS ShipIT REST API](https://apis.io/apis/gls-group/gls-shipit-rest-api/) — Group-wide shipping integration web service (version 3.4.19) exposed by the GLS ShipIT backend, documented publicly as Doxygen reference pages. Resource…
- [GLS Group Authentication API](https://apis.io/apis/gls-group/gls-group-authentication-api/) — The Authentication API from GLS Group — 1 operation(s) for authentication.
- [GLS Group Delivery API](https://apis.io/apis/gls-group/gls-group-delivery-api/) — The Delivery API from GLS Group — 4 operation(s) for delivery.
- [GLS Group Delivery Options API](https://apis.io/apis/gls-group/gls-group-deliveryoptions-api/) — The DeliveryOptions API from GLS Group — 1 operation(s) for deliveryoptions.
- [GLS Group Home API](https://apis.io/apis/gls-group/gls-group-home-api/) — The Home API from GLS Group — 1 operation(s) for home.
- [GLS Group Monitor API](https://apis.io/apis/gls-group/gls-group-monitor-api/) — The Monitor API from GLS Group — 1 operation(s) for monitor.
- [GLS Group Parcel API](https://apis.io/apis/gls-group/gls-group-parcel-api/) — The Parcel API from GLS Group — 2 operation(s) for parcel.
- [GLS Group Parcel Shop API](https://apis.io/apis/gls-group/gls-group-parcelshop-api/) — The ParcelShop API from GLS Group — 1 operation(s) for parcelshop.
- [GLS Group Pickup API](https://apis.io/apis/gls-group/gls-group-pickup-api/) — The Pickup API from GLS Group — 2 operation(s) for pickup.
- [GLS Group Pod API](https://apis.io/apis/gls-group/gls-group-pod-api/) — The Pod API from GLS Group — 1 operation(s) for pod.
- [GLS Group Shop Return API](https://apis.io/apis/gls-group/gls-group-shopreturn-api/) — The ShopReturn API from GLS Group — 1 operation(s) for shopreturn.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Collections (4)

Postman and Open Collection request collections.

- [GLS Netherlands LabelApi - Production](https://apis.io/collections/gls-group/open-gls-netherlands-label-api/)
- [GLS.API (Version 1.0)](https://apis.io/collections/gls-group/open-gls-netherlands-label-api-test/)
- [GLS T&T Api - Production](https://apis.io/collections/gls-group/open-gls-track-and-trace-api/)
- [GLS T&T Api - Test](https://apis.io/collections/gls-group/open-gls-track-and-trace-api-test/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://gls-group.com/)
- [Getting started](https://dev-portal.gls-group.net/get-started)
- [API reference](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/index.html)
- [Sign up](https://dev-portal.gls-group.net/accounts/login)
- [Terms of service](https://dev-portal.gls-group.net/general-terms-and-conditions)
- [Privacy policy](https://dev-portal.gls-group.net/privacy-policy)

## API Evangelist rating

**Kin Score 21.8** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 58.9 |
| Contract quality | 42.0 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 23.8 |
| Access clarity | 13.2 |

**Agent readiness 27.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | unknown |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 0.0** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/gls-group/](https://apis.io/providers/gls-group/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for GLS Group: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/gls-group/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

# GLS Group (gls-group)

GLS Group (General Logistics Systems B.V.) is a European ground-based parcel and freight carrier headquartered in Amsterdam-Duivendrecht, Netherlands, and owned by International Distributions Services plc. It operates a road network of more than 120 hubs and roughly 1,600 depots across some 50 countries in Europe, the United States and Canada, moving B2B and B2C parcels up to about 32 kg plus a freight/LTL and express line, with an out-of-home ParcelShop and locker network. In the supply chain it is a last-mile and middle-mile parcel integrator: the party a shipper, e-commerce platform or shipping-API aggregator hands a consignment to for pickup, linehaul, customs clearance and delivery. Its API posture is federated and contract-bound rather than unified. The GLS Group developer portal (dev-portal.gls-group.net, run by GLS IT Services GmbH on Apigee) allows self-serve account and app registration with API keys or OAuth 2.0, but its API catalog is only visible after sign-in and "restricted" APIs additionally require approval by a local GLS representative. National units run their own portals — GLS Netherlands publishes an Azure API Management portal at api-portal.gls.nl whose OpenAPI 3.0.1 definitions for the Label API and the Track & Trace API are anonymously readable, but calling them still requires MyGLS credentials issued to a contracted shipper. The group-wide GLS ShipIT REST/SOAP web services are fully documented in public Doxygen reference pages, yet the base URL itself is handed out only with credentials by a customer's primary GLS contact. No industry data standard — GS1/EPCIS, UPU, DCSA, IATA ONE Record, UN/EDIFACT or ANSI X12 — is referenced anywhere in the artifacts GLS publishes; every identifier and event vocabulary is GLS-proprietary.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gls-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gls-group/refs/heads/main/apis.yml)

## Tags

- Logistics
- Supply Chain
- Netherlands
- Parcel
- Shipping
- Track and Trace
- Freight
- Last Mile
- Europe
- Customs

## Timestamps

- **Created:** 2026-07-30
- **Modified:** 2026-07-30

## APIs

### GLS Netherlands Label API

RESTful shipping API for printing labels and manifesting shipping data for GLS Netherlands. Covers login validation, label creation (parcel ShipType "P" and freight ShipType "F"), label deletion, single and multiple label confirmation, ParcelShop lookup, delivery-option lookup, pickup creation and deletion, and shop-return creation. Labels are returned as ZPL or Base64 PDF (pdf, pdfa6u, pdfa6s, pdfroutingonly, pdf2a4, pdf4a4), or the raw routing data can be returned so the customer prints their own label. Authentication carries MyGLS username and password in the request body; the developer-portal subscription key is issued per registered product. An OpenAPI 3.0.1 definition is anonymously exportable from the Azure API Management portal, and a separate test environment is published at https://api.gls.nl/test/v1.

- **Human URL:** [https://api-portal.gls.nl/api-details#api=gls-netherlands-labelapi-production](https://api-portal.gls.nl/api-details#api=gls-netherlands-labelapi-production)
- **Base URL:** `https://api.gls.nl/v1`

#### Tags

- Parcel
- Labels
- Shipping
- Pickup
- Returns
- ParcelShop
- Netherlands

#### Properties

- [OpenAPI](openapi/gls-netherlands-label-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gls-netherlands-label-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-netherlands-label-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/gls-netherlands-label-api-test-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gls-netherlands-label-api-test.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-netherlands-label-api-test.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://api-portal.gls.nl/content/GLS_Shipping_API_v0.8.pdf)
- [API Reference](https://api-portal.gls.nl/api-details#api=gls-netherlands-labelapi-production)
- [Portal Home](https://api-portal.gls.nl/)
- [Sandbox](https://api-portal.gls.nl/api-details#api=gls-netherlands-labelapi-test)

### GLS Netherlands Track and Trace API

Read API for parcel status and proof of delivery in the GLS Netherlands network. Three documented operations — POST /api/parcel/v1/details, POST /api/parcel/v1/search and POST /api/pod/v1 — return parcel event history, address data, dimensions, weight, product, state/substate, ETA and a tracking URI, plus proof-of-delivery documents. Complemented by two customer-registered push webhooks (parcel events and signature/proof-of-delivery PNG) that GLS POSTs to a URL the customer supplies out of band; there is no self-service subscription endpoint. An OpenAPI 3.0.1 definition is anonymously exportable, and a test environment is published at https://api.gls.nl/tt-test.

- **Human URL:** [https://api-portal.gls.nl/api-details#api=track-trace-api-v1](https://api-portal.gls.nl/api-details#api=track-trace-api-v1)
- **Base URL:** `https://api.gls.nl/tt/V1`

#### Tags

- Track and Trace
- Parcel
- Proof of Delivery
- Webhooks
- Netherlands

#### Properties

- [OpenAPI](openapi/gls-track-and-trace-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gls-track-and-trace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-track-and-trace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](openapi/gls-track-and-trace-api-test-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gls-track-and-trace-api-test.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-track-and-trace-api-test.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://api-portal.gls.nl/track-trace-webhook)
- [Webhooks](https://api-portal.gls.nl/content/webhooks.pdf)
- [API Reference](https://api-portal.gls.nl/api-details#api=gls-t-t-api-test)
- [Portal Home](https://api-portal.gls.nl/)

### GLS ShipIT REST API

Group-wide shipping integration web service (version 3.4.19) exposed by the GLS ShipIT backend, documented publicly as Doxygen reference pages. Resource groups cover shipment processing (POST /backend/rs/shipments, /shipments/cancel/{trackID}, /shipments/allowedservices, /shipments/endofday, /shipments/updateparcelweight), ParcelShop search (getParcelShopById, getParcelShopsByCountryCode, findNearestParcelShopForAddress, getParcelShopinDistance), parcel tracking (POST /parcels, /parceldetails, /parcelpod), delivery time-frame estimation (POST /backend/rs/timeframe/deliverydays) and sporadic collection scheduling (/backend/rs/sporadiccollection). Authentication is HTTP Basic over TLS 1.2 with an optional Requester header for data-protection logging; media types are application/glsVersion1+json and application/json. No baseURL is published — GLS states the endpoints for the centrally hosted service are obtained from the customer's primary GLS contact along with credentials, or point at a locally installed ShipIT backend. No OpenAPI, Swagger or WADL file is offered.

- **Human URL:** [https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/index.html](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/index.html)

#### Tags

- Shipping
- Parcel
- Track and Trace
- ParcelShop
- Pickup
- Freight

#### Properties

- [API Reference](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/index.html)
- [Documentation](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/rest_shipment_processing.html)
- [Documentation](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/rest_parcel_shop.html)
- [Documentation](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/rest_tracking.html)
- [Documentation](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/rest_timeframe.html)
- [Documentation](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/rest_sporadic_collection.html)
- [Postman Collection](collections/gls-netherlands-label-api-test.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-netherlands-label-api-test.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/gls-netherlands-label-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-netherlands-label-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/gls-track-and-trace-api-test.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-track-and-trace-api-test.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/gls-track-and-trace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gls-track-and-trace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://gls-group.com/)
- [Portal Home](https://dev-portal.gls-group.net/)
- [Getting Started](https://dev-portal.gls-group.net/get-started)
- [F A Q](https://dev-portal.gls-group.net/faq)
- [Sign Up](https://dev-portal.gls-group.net/accounts/login)
- [Terms of Service](https://dev-portal.gls-group.net/general-terms-and-conditions)
- [Privacy Policy](https://dev-portal.gls-group.net/privacy-policy)
- [Security Disclosure](https://gls-group.com/.well-known/security.txt)
- [Portal Home](https://api-portal.gls.nl/)
- [API Reference](https://shipit.gls-group.eu/webservices/3_4_19/doxygen/WS-REST-API/index.html)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

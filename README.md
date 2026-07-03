# Open Dental (opendental)

Open Dental is dental practice management software with an openly documented public REST API. The API is hosted at Open Dental headquarters (base `https://api.opendental.com/api/v1`) and lets approved third-party developers read and write practice data - patients, appointments, providers, procedures, insurance claims, payments, ledger adjustments, fee schedules, recalls, documents, medications and prescriptions, referrals, and clinical sheets - on behalf of Open Dental customers. Requests authenticate with a per-application Developer Key and a per-customer Customer Key sent together in an `Authorization: ODFHIR {DeveloperKey}/{CustomerKey}` header. The public specification documents 130+ resource groups with GET/POST/PUT/DELETE operations. Open Dental also offers a local API Service that talks to the on-premises Open Dental program without routing through Open Dental's servers, plus a separate FHIR interface.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/apis.yml)

## Tags

- Dental
- Practice Management
- Healthcare
- EHR
- Patient Records
- REST

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Authentication

Every request carries an `Authorization` header:

```
Authorization: ODFHIR {DeveloperKey}/{CustomerKey}
```

The Developer Key is issued per application by Open Dental Vendor Relations (`vendor.relations@opendental.com`); the Customer Key is enabled per Open Dental customer. Some endpoints also accept HTTP Basic auth with the Developer Key as the username and the Customer Key as the password.

## APIs

### Open Dental Patients API

Create, read, update, and search patient demographic records. Includes a fast `Simple` listing and a full Patient Select-style search with dozens of filters. Patients cannot be deleted via the API.

- **Human URL:** [https://www.opendental.com/site/apipatients.html](https://www.opendental.com/site/apipatients.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Patients
- Demographics
- Records

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apipatients.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Appointments API

Schedule and manage appointments - standard, planned, and WebSched - find open time slots, read ASAP and WebSched lists, break appointments, append notes, and update confirmation status.

- **Human URL:** [https://www.opendental.com/site/apiappointments.html](https://www.opendental.com/site/apiappointments.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Appointments
- Scheduling
- WebSched

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apiappointments.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Providers API

Read, create, and update providers - dentists, hygienists, billing entities, and dummy providers - with optional filtering by clinic or modification timestamp.

- **Human URL:** [https://www.opendental.com/site/apiproviders.html](https://www.opendental.com/site/apiproviders.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Providers
- Staff
- Clinics

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apiproviders.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Procedures API

Full CRUD over ProcedureLogs (individual treatment procedures on a patient's chart), plus insurance treatment-history entries and group notes across multiple procedures.

- **Human URL:** [https://www.opendental.com/site/apiprocedurelogs.html](https://www.opendental.com/site/apiprocedurelogs.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Procedures
- ProcedureLogs
- Treatment

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apiprocedurelogs.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Insurance & Claims API

Manage insurance claims and related insurance data - create, read, update, and delete claims, change claim status, split claims, and work with insurance plans, subscribers, benefits, and claim procedures.

- **Human URL:** [https://www.opendental.com/site/apiclaims.html](https://www.opendental.com/site/apiclaims.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Claims
- Insurance
- Benefits

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apiclaims.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Payments API

Post patient payments, issue refunds, update payment details, and reallocate an existing payment's splits across procedures and payment-plan charges.

- **Human URL:** [https://www.opendental.com/site/apipayments.html](https://www.opendental.com/site/apipayments.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Payments
- Refunds
- Billing

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apipayments.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Accounts & Ledger API

Work with the patient account ledger - adjustments, payment splits (PaySplits), payment plans and charges, and statements. *(Endpoints modeled on Open Dental's standard REST CRUD convention; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Ledger
- Adjustments
- PaySplits

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Fees & Fee Schedules API

Manage procedure fees and the fee schedules (FeeScheds) that price them across procedure code, provider, and clinic. *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apifees.html](https://www.opendental.com/site/apifees.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Fees
- Fee Schedules
- Pricing

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apifees.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Recalls API

Read and manage patient recalls - the hygiene and continuing-care reminders that drive re-appointment. *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Recalls
- Hygiene
- Reminders

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Documents API

Upload, download, and manage documents attached to a patient's record - scanned forms, images, and files in the imaging module. *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Documents
- Images
- Attachments

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Medications & Prescriptions API

Manage the medication catalog (Medications), a patient's medication list (MedicationPats), and prescriptions written for patients (RxPats). *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Medications
- Prescriptions
- RxPats

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Referrals API

Manage referral sources and specialists (Referrals) and the attachments that link a referral to a patient or procedure (RefAttaches). *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Referrals
- Specialists
- RefAttaches

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Open Dental Sheets API

Read and create Sheets - the configurable clinical and administrative forms (consent forms, patient forms, treatment plans) that Open Dental renders and stores per patient. *(Endpoints modeled; verify against the live spec.)*

- **Human URL:** [https://www.opendental.com/site/apispecification.html](https://www.opendental.com/site/apispecification.html)
- **Base URL:** `https://api.opendental.com/api/v1`

#### Tags

- Sheets
- Forms
- eForms

#### Properties

- [Documentation](https://www.opendental.com/site/apispecification.html)
- [API Reference](https://www.opendental.com/site/apispecification.html)
- [OpenAPI](openapi/opendental-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opendental.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opendental.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/OpenDental)
- [LinkedIn](https://www.linkedin.com/company/open-dental-software)
- [Website](https://www.opendental.com)
- [Documentation](https://www.opendental.com/site/apispecification.html)
- [Plans](plans/opendental-plans-pricing.yml)
- [Rate Limits](rate-limits/opendental-rate-limits.yml)
- [Fin Ops](finops/opendental-finops.yml)

## Notes

- **Endpoint confirmation:** Patients, Appointments, Providers, Procedures (ProcedureLogs), Insurance & Claims, and Payments are grounded in Open Dental's published per-resource reference pages. Accounts & Ledger, Fees & Fee Schedules, Recalls, Documents, Medications & Prescriptions, Referrals, and Sheets are modeled on Open Dental's standard REST CRUD convention and the spec's resource index - verify exact paths and fields against the live specification. The full spec documents 130+ resource groups.
- **Rate limits:** Cloud API throughput is throttled by permission tier (read-only ~1 request / 5 seconds; higher tiers ~1 request / second). The on-premises Local API / API Service is not throttled. Expect `429 TooManyRequests` (honor `Retry-After`) and `504 Gateway Timeout` for requests exceeding the 60-second processing limit.
- **WebSocket:** Open Dental exposes no documented public WebSocket API - the public surface is request/response REST (cloud API, Local API / API Service, and a separate FHIR interface). See `review.yml`.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

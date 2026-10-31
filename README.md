# Open Dental

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

Open Dental is dental practice management software with an openly documented public REST API. The API is hosted at Open Dental headquarters (base https://api.opendental.com/api/v1) and lets approved third-party developers read and write practice data - patients, appointments, providers, procedures, insurance claims, payments, ledger adjustments, fee schedules, recalls, documents, medications and prescriptions, referrals, and clinical sheets - on behalf of Open Dental customers. Requests authenticate with a per-application Developer Key and a per-customer Customer Key sent together in an Authorization ODFHIR {DeveloperKey}/{CustomerKey} header. The public spec documents 130+ resource groups with GET/POST/PUT/DELETE operations. Open Dental also runs a local API Service option that talks to the on-premises Open Dental program without routing through Open Dental's servers, and a separate FHIR interface.

**Areas:** Dental · Practice Management · Healthcare · Electronic Health Records · Patient Records · REST

## Open Dental on APIs.io

Everything profiled for Open Dental is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/opendental/](https://apis.io/providers/opendental/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Open Dental Accounts & Ledger API](https://apis.io/apis/opendental/opendental-accounts-ledger-api/) — MODELED. Adjustments and payment splits on the patient ledger.
- [Open Dental Appointments API](https://apis.io/apis/opendental/opendental-appointments-api/) — CONFIRMED. Scheduling, slots, and WebSched.
- [Open Dental Claims API](https://apis.io/apis/opendental/opendental-claims-api/) — CONFIRMED. Insurance claims and claim workflow.
- [Open Dental Documents API](https://apis.io/apis/opendental/opendental-documents-api/) — MODELED. Files and images attached to a patient.
- [Open Dental Fees & Fee Schedules API](https://apis.io/apis/opendental/opendental-fees-fee-schedules-api/) — MODELED. Procedure fees and fee schedules.
- [Open Dental Medications & Prescriptions API](https://apis.io/apis/opendental/opendental-medications-prescriptions-api/) — MODELED. Medication catalog, patient meds, and prescriptions.
- [Open Dental Patients API](https://apis.io/apis/opendental/opendental-patients-api/) — CONFIRMED. Patient demographic records.
- [Open Dental Payments API](https://apis.io/apis/opendental/opendental-payments-api/) — CONFIRMED. Patient payments, refunds, and split reallocation.
- [Open Dental Procedures API](https://apis.io/apis/opendental/opendental-procedures-api/) — CONFIRMED. ProcedureLogs, insurance history, and group notes.
- [Open Dental Providers API](https://apis.io/apis/opendental/opendental-providers-api/) — CONFIRMED. Dentists, hygienists, and billing entities.
- [Open Dental Recalls API](https://apis.io/apis/opendental/opendental-recalls-api/) — MODELED. Hygiene / continuing-care recalls.
- [Open Dental Referrals API](https://apis.io/apis/opendental/opendental-referrals-api/) — MODELED. Referral sources and attachments.
- [Open Dental Sheets API](https://apis.io/apis/opendental/opendental-sheets-api/) — MODELED. Configurable clinical and administrative forms.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Opendental Agentic Access](https://apis.io/agentic-access/opendental/opendental-agentic-access/)

#### Collections (14)

Postman and Open Collection request collections.

- [Open Dental API](https://apis.io/collections/opendental/open-opendental/)
- [Open Dental Accounts & Ledger API](https://apis.io/collections/opendental/open-opendental-accounts-ledger-api/)
- [Open Dental Accounts & Ledger Appointments API](https://apis.io/collections/opendental/open-opendental-appointments-api/)
- [Open Dental Accounts & Ledger Claims API](https://apis.io/collections/opendental/open-opendental-claims-api/)
- [Open Dental Accounts & Ledger Documents API](https://apis.io/collections/opendental/open-opendental-documents-api/)
- [Open Dental Accounts & Ledger Fees & Fee Schedules API](https://apis.io/collections/opendental/open-opendental-fees-fee-schedules-api/)
- [Open Dental Accounts & Ledger Medications & Prescriptions API](https://apis.io/collections/opendental/open-opendental-medications-prescriptions-api/)
- [Open Dental Accounts & Ledger Patients API](https://apis.io/collections/opendental/open-opendental-patients-api/)
- [Open Dental Accounts & Ledger Payments API](https://apis.io/collections/opendental/open-opendental-payments-api/)
- [Open Dental Accounts & Ledger Procedures API](https://apis.io/collections/opendental/open-opendental-procedures-api/)
- [Open Dental Accounts & Ledger Providers API](https://apis.io/collections/opendental/open-opendental-providers-api/)
- [Open Dental Accounts & Ledger Recalls API](https://apis.io/collections/opendental/open-opendental-recalls-api/)
- [Open Dental Accounts & Ledger Referrals API](https://apis.io/collections/opendental/open-opendental-referrals-api/)
- [Open Dental Accounts & Ledger Sheets API](https://apis.io/collections/opendental/open-opendental-sheets-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Opendental Authentication](https://apis.io/security/opendental/opendental-authentication/)
- [Opendental Domain Security](https://apis.io/security/opendental/opendental-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Opendental Plans Pricing](https://apis.io/plans/opendental/opendental-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Opendental Rate Limits](https://apis.io/rate-limits/opendental/opendental-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Opendental Finops](https://apis.io/finops/opendental/opendental-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.opendental.com)
- [Documentation](https://www.opendental.com/site/apispecification.html)
- [Blog](https://opendental.blog/feed/)
- [GitHub](https://github.com/OpenDental)

## API Evangelist rating

**Kin Score 26.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 49.2 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 31.0 |
| Access clarity | 7.9 |

**Agent readiness 19.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 9.4** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/opendental/](https://apis.io/providers/opendental/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Open Dental: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/opendental/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

# University of Newcastle Australia

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

The University of Newcastle (UON) is a public research university in Callaghan and Newcastle, New South Wales, ranked #179 in the QS World University Rankings order used by this cohort. It is a federation of buyers rather than an API producer: there is no central developer portal and no institutional API gateway — api.newcastle.edu.au, apis.newcastle.edu.au, developer.newcastle.edu.au, data.newcastle.edu.au and status.newcastle.edu.au all fail to resolve — and UON publishes no OpenAPI description for anything. What it genuinely operates is small and specific: a Shibboleth identity provider at idp.newcastle.edu.au serving live SAML 2.0 metadata under its own entityID and scope, registered in the Australian Access Federation; and a self-hosted XNAT 1.9.1.1 imaging-informatics platform at xnat.newcastle.edu.au, run with the Hunter Medical Research Institute on the university's own AWS estate, whose REST API answers on UON's host and is registered as a SAML service provider in the same federation. UON also holds two DataCite repository clients in its own name, ARDCX.UON and UONAU.FIGSHARE. Everything else that looks programmable is a tenancy on someone else's platform and is recorded as such, never as UON engineering: Open Research Newcastle is a Figshare tenancy, the course handbook is a CourseLoop tenancy, the learning management system is an Instructure Canvas tenancy, library guides are Springshare, site search is Squiz Funnelback, the student portal is PeopleSoft behind Okta, and the service desk is Oracle B2C Service. This profile was corrected on 2026-08-30: ten OpenAPI documents previously held here were Figshare's generic api.figshare.com/v2 contract, not the university's, and were removed along with everything derived from them.

**Areas:** University · Higher Education · Education · Research · Australia · New South Wales · Identity Federation · SAML · Shibboleth · Research Computing · Medical Imaging · Research Repository

## University of Newcastle Australia on APIs.io

Everything profiled for University of Newcastle Australia is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/uon/](https://apis.io/providers/uon/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [University of Newcastle Shibboleth Identity Provider (SAML 2.0 metadata)](https://apis.io/apis/uon/identity-federation/) — UON's institutional identity provider, publishing machine-readable SAML 2.0 metadata at a stable URL. entityID https://idp.newcastle.edu.au/idp/shibboleth,…
- [University of Newcastle XNAT Imaging Informatics Platform](https://apis.io/apis/uon/xnat-imaging/) — A self-hosted XNAT 1.9.1.1 imaging-informatics platform operated by the university with the Hunter Medical Research Institute, running on UON's own AWS…
- [Open Research Newcastle (Figshare) — TENANT](https://apis.io/apis/uon/open-research-figshare/) — The university's open-access institutional repository and research-data store, running on the Figshare platform at openresearch.newcastle.edu.au. This is a…
- [University of Newcastle Course Handbook (CourseLoop) — TENANT](https://apis.io/apis/uon/course-handbook-courseloop/) — The university's program and course handbook, served from handbook.newcastle.edu.au on the CourseLoop platform. Machine-readable to the extent that it…
- [University of Newcastle Canvas LMS (Instructure) — TENANT](https://apis.io/apis/uon/canvas-lms/) — UON's learning management system, an Instructure Canvas tenancy reachable both at canvas.newcastle.edu.au and at newcastle.instructure.com, which return the…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Vocabulary (1)

The provider's domain terms, defined.

- [University of Newcastle Open Research Vocabulary](https://apis.io/vocabularies/uon/uon-vocabulary/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Uon Domain Security](https://apis.io/security/uon/uon-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Uon Plans Pricing](https://apis.io/plans/uon/uon-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Uon Rate Limits](https://apis.io/rate-limits/uon/uon-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Uon Finops](https://apis.io/finops/uon/uon-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.newcastle.edu.au/)
- [Documentation](https://libguides.newcastle.edu.au/)
- [GitHub](https://github.com/university-of-newcastle-research)

## API Evangelist rating

**Kin Score 12.3** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 4.4 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 9.5 |
| Access clarity | 5.3 |

**Agent readiness 0.6** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
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

**Regulatory alignment 18.6** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/uon/](https://apis.io/providers/uon/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for University of Newcastle Australia: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/uon/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

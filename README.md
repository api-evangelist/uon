# University of Newcastle Australia (uon)

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

The University of Newcastle (UON) is a public research university in Newcastle, New South Wales, Australia, ranked #179 in the QS World University Rankings 2025. This repository catalogs UON's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=uon-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

University, Higher Education, Education, Research, Australia, New South Wales, Identity Federation, SAML, Shibboleth, Research Computing, Medical Imaging, Research Repository, Course Catalog, DataCite, Tenant

## APIs

UON operates no public developer portal and no API gateway (api., apis., developer., data. and
status.newcastle.edu.au do not resolve), and publishes no OpenAPI for anything. Surfaces are recorded
with an operator, because for a university that is the question that matters.

Institution-operated:

- **Shibboleth Identity Provider (SAML 2.0 metadata)** — https://idp.newcastle.edu.au/idp/shibboleth
  returns HTTP 200 application/xml with entityID `https://idp.newcastle.edu.au/idp/shibboleth` and
  `shibmd:Scope newcastle.edu.au`. Registered in the Australian Access Federation aggregate.
- **XNAT imaging informatics platform** — https://xnat.newcastle.edu.au, self-hosted XNAT 1.9.1.1 on
  UON's own AWS estate with the Hunter Medical Research Institute, registered as a SAML service
  provider in the AAF. `/xapi/siteConfig/buildInfo` answers unauthenticated; data endpoints and the
  Swagger description redirect to login.

Tenant relationships — real institutional facts, but the contract is the vendor's and none of these
vendors' specifications are kept in this repository:

- **Open Research Newcastle** — Figshare tenancy at https://openresearch.newcastle.edu.au (AWS WAF
  challenge, HTTP 202, on every request including `/oai?verb=Identify`).
- **Course Handbook** — CourseLoop tenancy at https://handbook.newcastle.edu.au; sitemap enumerates
  9,755 program and course URLs.
- **Canvas LMS** — Instructure tenancy at https://canvas.newcastle.edu.au; the Canvas REST API returns
  HTTP 401 at `/api/v1/accounts`.

Also holds two DataCite repository clients in its own name: `ARDCX.UON` (65 DOIs) and
`UONAU.FIGSHARE` (29 DOIs).

## Plans, Rate Limits, and FinOps

- Plans & Pricing: [plans/uon-plans-pricing.yml](plans/uon-plans-pricing.yml)
- Rate Limits: [rate-limits/uon-rate-limits.yml](rate-limits/uon-rate-limits.yml)
- FinOps: [finops/uon-finops.yml](finops/uon-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.newcastle.edu.au/ (live, behind a Cloudflare bot challenge — HTTP 403)
- Identity Federation: https://idp.newcastle.edu.au/idp/shibboleth
- Research Computing: https://xnat.newcastle.edu.au/
- Research Repository: https://openresearch.newcastle.edu.au/
- Course Catalog: https://handbook.newcastle.edu.au/
- Policies: https://policies.newcastle.edu.au/
- Library Guides: https://libguides.newcastle.edu.au/ (Springshare tenancy)
- GitHub Organization: https://github.com/university-of-newcastle-research
- Conformance: [conformance/uon-conformance.yml](conformance/uon-conformance.yml)
- Review: [review.yml](review.yml)

## Notes

Re-profiled on 2026-08-30 under the API Evangelist university pipeline, which settles operator
attribution before saving anything. **This repository previously held eleven Figshare OpenAPI
documents attributed to the University of Newcastle.** Every one of them carried
`info.title: "Figshare Altmetric API"` (or `"Figshare altmetric <Resource> API"`),
`info.contact: Figshare Support` at support.figshare.com, and `servers[0].url:
https://api.figshare.com/v2` — a generic vendor host the cohort audit finds claimed by sixteen other
institutions in this catalog. Those eleven specs and the thirty-six artifacts derived from them
(OpenCollection and Postman collections, JSON Schema, JSON Structure, examples, a JSON-LD context,
two Spectral rulesets, a vocabulary, OAuth scopes, an authentication summary, an agentic-access
contract and a capability map) were removed. Nothing was derived to replace them: UON publishes no
machine-readable contract of its own, and the XNAT deployment's Swagger is behind authentication and
belongs to the XNAT product in any case.

No API endpoints were fabricated. Limits on this pass, recorded as limitations on us rather than
findings about the institution: www.newcastle.edu.au and its subordinate hosts return a Cloudflare
bot challenge (HTTP 403, `cf-mitigated: challenge`), so robots.txt, llms.txt and `.well-known` could
not be read there; openresearch.newcastle.edu.au returns an AWS WAF challenge (HTTP 202,
`x-amzn-waf-action: challenge`, zero-byte body) on every User-Agent tried, so the OAI-PMH `Identify`
response was never seen and OAI-PMH conformance is recorded as **not established** rather than
assumed. `nova.newcastle.edu.au`, the former VITAL repository, is a dangling CNAME to a deleted AWS
load balancer and no longer resolves. See [apis.yml](apis.yml) `x-coverage` for the full per-URL
evidence table and [conformance/uon-conformance.yml](conformance/uon-conformance.yml) for
education-regime standard conformance.

## Maintainers

- Kin Lane — kin@apievangelist.com

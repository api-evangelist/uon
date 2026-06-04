# University of Newcastle Australia (uon)

The University of Newcastle (UON) is a public research university in Newcastle, New South Wales, Australia, ranked #179 in the QS World University Rankings 2025. This repository catalogs UON's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=uon-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Research, Open Access, Repository, OAI-PMH, Australia

## APIs

UON does not operate a dedicated public API developer portal. The verifiable programmatic footprint is research-oriented, via the Figshare-hosted institutional repository:

- **Open Research Newcastle (Figshare REST API)** — institutional open access repository launched in 2025 on Figshare; records are accessible through the public Figshare REST API. Docs: https://docs.figshare.com/ · Repository: https://openresearch.newcastle.edu.au/
- **Open Research Newcastle (OAI-PMH)** — OAI-PMH metadata harvesting endpoint at https://openresearch.newcastle.edu.au/oai (automated clients may hit a platform bot-mitigation challenge).

## Plans, Rate Limits, and FinOps

- Plans & Pricing: [plans/uon-plans-pricing.yml](plans/uon-plans-pricing.yml)
- Rate Limits: [rate-limits/uon-rate-limits.yml](rate-limits/uon-rate-limits.yml)
- FinOps: [finops/uon-finops.yml](finops/uon-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.newcastle.edu.au/
- GitHub: https://github.com/university-of-newcastle-research
- LinkedIn: https://www.linkedin.com/school/university-of-newcastle/
- Review: [review.yml](review.yml)

## Notes

This profile reflects only publicly verifiable resources. No API endpoints were fabricated. UON's student, staff, and enterprise systems (myUni, online tools, ServiceNow) sit behind institutional SSO and are not openly documented; probes to the main site and learning portals returned 403/login responses. The cataloged research repository is hosted on Figshare, so its programmatic access is provided by the documented public Figshare REST API and an OAI-PMH endpoint. The Figshare repository and OAI endpoint returned HTTP 202 (CDN/platform bot challenge) to automated clients but are live in a browser; the Figshare public API (api.figshare.com/v2) returned HTTP 200. See [review.yml](review.yml) for per-URL status.

## Maintainers

- Kin Lane — kin@apievangelist.com

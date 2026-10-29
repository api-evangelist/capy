# Capy

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

Capy is an AI software-engineering platform that orchestrates a fleet of cloud coding agents inside the apps a team already uses (Slack, Linear, GitHub). Each task runs in its own isolated Ubuntu VM where a captain agent plans and build agents execute — writing code, running end-to-end browser tests, migrating codebases, generating docs, triaging and fixing bugs, and opening pull requests for review. Capy supports multiple frontier models (GPT, Claude, Grok, Gemini) and exposes a REST API (bearer capy_ token) plus scheduled and webhook-triggered automations. Backed by CRV; SOC 2 Type II certified.

**Areas:** Company · Artificial Intelligence · AI Coding Agents · Software Engineering · Developer Tools · Automation · Code Review · DevOps

## Capy on APIs.io

Everything profiled for Capy is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/capy/](https://apis.io/providers/capy/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [Capy Automations API](https://apis.io/apis/capy/capy-automations-api/) — The automations API from Capy — 3 operation(s) for automations.
- [Capy Browser Snapshots API](https://apis.io/apis/capy/capy-browser-snapshots-api/) — The browser-snapshots API from Capy — 2 operation(s) for browser-snapshots.
- [Capy Environment Variables API](https://apis.io/apis/capy/capy-environment-variables-api/) — The environment-variables API from Capy — 2 operation(s) for environment-variables.
- [Capy Models API](https://apis.io/apis/capy/capy-models-api/) — The models API from Capy — 1 operation(s) for models.
- [Capy Projects API](https://apis.io/apis/capy/capy-projects-api/) — The projects API from Capy — 2 operation(s) for projects.
- [Capy Sessions API](https://apis.io/apis/capy/capy-sessions-api/) — The sessions API from Capy — 1 operation(s) for sessions.
- [Capy Setup API](https://apis.io/apis/capy/capy-setup-api/) — The setup API from Capy — 1 operation(s) for setup.
- [Capy Snapshots API](https://apis.io/apis/capy/capy-snapshots-api/) — The snapshots API from Capy — 1 operation(s) for snapshots.
- [Capy Tags API](https://apis.io/apis/capy/capy-tags-api/) — The tags API from Capy — 2 operation(s) for tags.
- [Capy Tasks API](https://apis.io/apis/capy/capy-tasks-api/) — The tasks API from Capy — 2 operation(s) for tasks.
- [Capy Threads API](https://apis.io/apis/capy/capy-threads-api/) — The threads API from Capy — 8 operation(s) for threads.
- [Capy Usage API](https://apis.io/apis/capy/capy-usage-api/) — The usage API from Capy — 1 operation(s) for usage.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [capy](https://apis.io/servers/capy/capy/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Capy Agentic Access](https://apis.io/agentic-access/capy/capy-agentic-access/)

#### Collections (12)

Postman and Open Collection request collections.

- [Capy automations API](https://apis.io/collections/capy/open-capy-automations-api/)
- [Capy automations browser-snapshots API](https://apis.io/collections/capy/open-capy-browser-snapshots-api/)
- [Capy automations environment-variables API](https://apis.io/collections/capy/open-capy-environment-variables-api/)
- [Capy automations models API](https://apis.io/collections/capy/open-capy-models-api/)
- [Capy automations projects API](https://apis.io/collections/capy/open-capy-projects-api/)
- [Capy automations sessions API](https://apis.io/collections/capy/open-capy-sessions-api/)
- [Capy automations setup API](https://apis.io/collections/capy/open-capy-setup-api/)
- [Capy automations snapshots API](https://apis.io/collections/capy/open-capy-snapshots-api/)
- [Capy automations tags API](https://apis.io/collections/capy/open-capy-tags-api/)
- [Capy automations tasks API](https://apis.io/collections/capy/open-capy-tasks-api/)
- [Capy automations threads API](https://apis.io/collections/capy/open-capy-threads-api/)
- [Capy automations usage API](https://apis.io/collections/capy/open-capy-usage-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Capy Openapi Overlay](https://apis.io/overlays/capy/capy-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Capy Authentication](https://apis.io/security/capy/capy-authentication/)
- [Capy Domain Security](https://apis.io/security/capy/capy-domain-security/)
- [Capy Trust Center](https://apis.io/security/capy/capy-trust-center/)
- [Capy Vulnerability Disclosure](https://apis.io/security/capy/capy-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Capy Plans Pricing](https://apis.io/plans/capy/capy-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://capy.ai/)
- [Documentation](https://docs.capy.ai)
- [Getting started](https://docs.capy.ai/quickstart)
- [API reference](https://docs.capy.ai/api-reference/overview)
- [Pricing](https://capy.ai/pricing)
- [Sign up](https://capy.ai/sign-up)
- [Support](https://docs.capy.ai/support)
- [Blog](https://capy.ai/blog)
- [Security](https://capy.ai/security)
- [Compliance](https://trust.capy.ai)
- [Terms of service](https://capy.ai/terms-of-service)
- [Privacy policy](https://capy.ai/privacy-policy)

## API Evangelist rating

**Kin Score 54.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 47.1 |
| Contract governance | 18.2 |
| Operational transparency | 10.5 |
| Developer ergonomics | 58.9 |
| Access clarity | 84.2 |

**Agent readiness 37.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | verified |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 28.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/capy/](https://apis.io/providers/capy/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Capy: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/capy/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

# Eight Sleep (eight-sleep)

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

Eight Sleep builds the Pod, a temperature-regulating smart mattress cover with Autopilot AI sleep optimization, sleep and biometric tracking, thermal alarms, and an adjustable Base.

> **Unofficial API notice:** Eight Sleep does **not** publish an official public developer API. This catalog documents the **unofficial, community-reverse-engineered client API** (`auth-api.8slp.net`, `client-api.8slp.net`, `app-api.8slp.net`) that powers the Eight Sleep mobile app and is used by open-source projects such as [pyEight](https://github.com/mezz64/pyEight) and the [Home Assistant Eight Sleep integration](https://github.com/lukas-clarke/eight_sleep). These endpoints are not documented, supported, or guaranteed by Eight Sleep and can change or break without notice. Use at your own risk and only with your own account.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/eight-sleep/refs/heads/main/apis.yml)

## Tags

- Sleep
- IoT
- Smart Home
- Wearables
- Health
- Unofficial

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Eight Sleep Authentication API

UNOFFICIAL, community-reverse-engineered OAuth2 password-grant token endpoint (POST /v1/tokens) on auth-api.8slp.net that issues bearer access and refresh tokens for the Eight Sleep mobile app. Not an official public API.

- **Human URL:** [https://github.com/lukas-clarke/eight_sleep](https://github.com/lukas-clarke/eight_sleep)
- **Base URL:** `https://auth-api.8slp.net/v1`

#### Tags

- Authentication
- OAuth2
- Tokens
- Unofficial

#### Properties

- [Documentation](https://github.com/lukas-clarke/eight_sleep)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep User API

UNOFFICIAL community client endpoints for the current user (GET /v1/users/me) and individual users (GET /v1/users/{userId}), returning profile, device assignment, and side data. Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/mezz64/pyEight](https://github.com/mezz64/pyEight)
- **Base URL:** `https://client-api.8slp.net/v1`

#### Tags

- User
- Profile
- Unofficial

#### Properties

- [Documentation](https://github.com/mezz64/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep Device API

UNOFFICIAL community client endpoint (GET /v1/devices/{deviceId}) that returns Pod device state, online status, firmware, and bed-side (leftUserId, rightUserId, awaySides) assignment. Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/mezz64/pyEight](https://github.com/mezz64/pyEight)
- **Base URL:** `https://client-api.8slp.net/v1`

#### Tags

- Device
- Pod
- Unofficial

#### Properties

- [Documentation](https://github.com/mezz64/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep Temperature API

UNOFFICIAL community app-API endpoints to read and set a user's heating level (GET/PUT /v1/users/{userId}/temperature) on a unit-less -100..100 scale and toggle away mode (PUT /v1/users/{userId}/away-mode). Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/lukas-clarke/pyEight](https://github.com/lukas-clarke/pyEight)
- **Base URL:** `https://app-api.8slp.net/v1`

#### Tags

- Temperature
- Heating
- Away Mode
- Unofficial

#### Properties

- [Documentation](https://github.com/lukas-clarke/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep Trends API

UNOFFICIAL community client endpoint (GET /v1/users/{userId}/trends) returning per-night sleep trend data - sleep score, stage breakdown, heart rate, HRV, respiratory rate, and toss-and-turn metrics. Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/mezz64/pyEight](https://github.com/mezz64/pyEight)
- **Base URL:** `https://client-api.8slp.net/v1`

#### Tags

- Trends
- Sleep Tracking
- Biometrics
- Unofficial

#### Properties

- [Documentation](https://github.com/mezz64/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep Base API

UNOFFICIAL community app-API endpoints for the adjustable Base - read state (GET /v1/users/{userId}/base) and set head/feet angles or presets (POST /v1/users/{userId}/base/angle). Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/lukas-clarke/pyEight](https://github.com/lukas-clarke/pyEight)
- **Base URL:** `https://app-api.8slp.net/v1`

#### Tags

- Base
- Adjustable
- Position
- Unofficial

#### Properties

- [Documentation](https://github.com/lukas-clarke/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Eight Sleep Alarms API

UNOFFICIAL community app-API endpoints to list alarms and routines (GET /v1/users/{userId}/alarms, GET /v1/users/{userId}/routines) and update, snooze, stop, or dismiss them. Thermal/vibration wake-up alarms are part of Autopilot. Reverse-engineered, not officially supported.

- **Human URL:** [https://github.com/lukas-clarke/pyEight](https://github.com/lukas-clarke/pyEight)
- **Base URL:** `https://app-api.8slp.net/v1`

#### Tags

- Alarms
- Routines
- Unofficial

#### Properties

- [Documentation](https://github.com/lukas-clarke/pyEight)
- [OpenAPI](openapi/eight-sleep-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/eight-sleep.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/eight-sleep.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/eight-sleep)
- [Website](https://www.eightsleep.com)
- [Documentation](https://github.com/lukas-clarke/eight_sleep)
- [Plans](plans/eight-sleep-plans-pricing.yml)
- [Rate Limits](rate-limits/eight-sleep-rate-limits.yml)
- [Fin Ops](finops/eight-sleep-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

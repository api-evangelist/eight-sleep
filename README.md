# Eight Sleep (eight-sleep)

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

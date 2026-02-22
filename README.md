# apipick-china-phone

A [Claude Code](https://claude.ai/claude-code) skill that validates Chinese mobile phone numbers using the [apipick](https://www.apipick.com) China Phone Checker API.

## What it does

Given a Chinese mobile phone number, this skill returns:

- **Carrier** — China Mobile, China Telecom, or China Unicom
- **Province** — geographic province associated with the number
- **City** — city associated with the number
- **Zip code** — postal code for the area
- **Area code** — regional telephone prefix

## Requirements

An apipick API key is required. Get 100 free credits at [apipick.com](https://www.apipick.com).

## Installation

Install via Claude Code:

```bash
claude skills install https://github.com/apipick-lab/apipick-china-phone
```

## Usage

Once installed, just ask Claude naturally:

- *"Validate the Chinese phone number 13800138000"*
- *"What carrier is +8613912345678 on?"*
- *"Which province is this Chinese number from: 02112345678?"*

Claude will call the apipick API and return the carrier and location details.

## API Reference

| Field | Value |
|-------|-------|
| Endpoint | `POST https://www.apipick.com/api/check-china-phone` |
| Auth | `x-api-key` header |
| Cost | 1 credit per request |

See [`references/api_reference.md`](references/api_reference.md) for full documentation.

## Links

- [apipick.com](https://www.apipick.com) — API platform
- [China Phone Checker](https://www.apipick.com/check-china-phone) — product page
- [Get API Key](https://www.apipick.com/dashboard/api-keys)

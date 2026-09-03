# Template Status & Verification

## Classification

**Configurable n8n template asset — not a verified production deployment.**

This repository demonstrates workflow structure and integration logic. Credentials, provider accounts, endpoints, IDs, and environment-specific values must be configured before execution.

## What this repository proves

- A version-controlled n8n workflow export is present.
- The workflow has an inspectable trigger-to-action structure.
- Documentation describes the intended problem and setup path.
- Public configuration is intended to use placeholders rather than reusable secrets.

## What is not automatically proven

- Successful import into every current n8n version.
- Current validity of every third-party API endpoint or model identifier.
- A configured end-to-end run with real provider accounts.
- Production reliability, security, throughput, SLA, ROI, or client outcomes.

## Verification gate

Before calling this template "working" for a buyer or deployment:

1. Parse the JSON and import it into a clean n8n instance.
2. Inspect every connection, expression, IF/Switch branch, and Code node.
3. Replace every placeholder credential, URL, ID, model, webhook, table, channel, or resource reference.
4. Confirm current third-party API/version requirements.
5. Run a representative success case.
6. Run at least one malformed-input or provider-failure case.
7. Confirm expected side effects and stored state.
8. Record the configured test date and result in this file or a dedicated test report.

## Security

Do not commit API keys, tokens, passwords, OAuth secrets, private webhooks, customer PII, or production data. Use synthetic test data and fresh test credentials.

## Change record

- **2026-09-03:** Added repository-level verification/security/status control. This documentation update does not claim a workflow-logic change or configured runtime pass.

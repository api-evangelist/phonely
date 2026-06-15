# Phonely (phonely)

Phonely is an AI voice agent platform that answers business phone calls in real time with large-language-model-powered conversation, sub-400ms response latency, 1,000+ voices across 100+ languages, and fine-tuned industry models for healthcare, finance, real estate, and insurance. The platform exposes a REST API at app.phonely.ai/api for agent management and a post-call webhook that delivers structured JSON (transcript, summary, sentiment, action items, recording URL) to any HTTPS endpoint after each call. Prebuilt integrations cover Google Calendar, Salesforce, HubSpot, Five9, Zapier, Outlook, Slack, and Gmail; the visual workflow builder also supports importing arbitrary REST APIs from a curl command. Pricing is usage-based with Free, Starter ($50/mo), Pro ($150/mo), and Enterprise tiers — minutes-included plus per-minute overage rather than per-agent seats. The platform is SOC 2, HIPAA, GDPR, CCPA, and PCI compliant.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Phone
- Call Center
- Contact Center
- SMS
- Webhooks
- Workflow Automation
- Scheduling
- CRM

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Phonely Agents API

Manage Phonely voice agents programmatically. Retrieve a single agent or list all agents for a user, and update agent configuration including voice, greeting message, name, conversation style (Casual, Humorous, Direct, Formal, Persuasive, Friendly), humanization, and organization membership. Authenticated with an X-Authorization API key against the app.phonely.ai/api base.

- **Human URL:** [https://docs.phonely.ai/api-reference/introduction](https://docs.phonely.ai/api-reference/introduction)
- **Base URL:** `https://app.phonely.ai/api`

#### Tags

- AI
- Voice
- Agents
- Telephony
- Conversational AI

#### Properties

- [Documentation](https://docs.phonely.ai/api-reference/introduction)
- [Documentation](https://docs.phonely.ai/api-reference/endpoint/get-agent)
- [OpenAPI](openapi/phonely-agents-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/phonely-agents-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonely-agents-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/phonely-agent-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/phonely-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Phonely Webhooks API

Receive structured post-call event data from Phonely after each AI voice interaction completes. The Send Call Data post-call workflow action POSTs a JSON payload containing call metadata, full transcript (text + structured turns), AI-generated summary, purpose, topic, sentiment, key points, action items, follow-up indicators, mentioned entities (email, date, time), recording URL, and dashboard URL to any HTTPS endpoint you configure.

- **Human URL:** [https://docs.phonely.ai/webhook-reference/intro](https://docs.phonely.ai/webhook-reference/intro)

#### Tags

- AI
- Voice
- Webhooks
- Events
- Call Data

#### Properties

- [Documentation](https://docs.phonely.ai/webhook-reference/intro)
- [Documentation](https://docs.phonely.ai/webhook-reference/endpoint/postcall-webhook)
- [AsyncAPI](asyncapi/phonely-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/phonely-post-call-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/phonely-post-call-event-example.json)
- [Postman Collection](collections/phonely-agents-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonely-agents-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.phonely.ai)
- [Documentation](https://docs.phonely.ai)
- [Documentation](https://docs.phonely.ai/get-started/introduction)
- [Getting Started](https://docs.phonely.ai/get-started/quick-start)
- [Documentation](https://www.phonely.ai/developer)
- [Changelog](https://www.phonely.ai/dev/changelog)
- [Blog](https://www.phonely.ai/blogs)
- [Sign Up](https://app.phonely.ai)
- [Terms of Service](https://www.phonely.ai/terms)
- [Privacy Policy](https://www.phonely.ai/privacy)
- [LinkedIn](https://www.linkedin.com/company/phonely-ai)
- [Customers](https://customers.twilio.com/en-us/phonely)
- [Plans](https://www.phonely.ai/pricing)
- [Plans](plans/phonely-plans-pricing.yml)
- [Rate Limits](rate-limits/phonely-rate-limits.yml)
- [Fin Ops](finops/phonely-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com

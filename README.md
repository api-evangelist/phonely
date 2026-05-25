# Phonely (phonely)

Phonely is an AI voice agent platform that answers business phone calls in real time with large-language-model-powered conversation, sub-400ms response latency, 1,000+ voices across 100+ languages, and fine-tuned industry models for healthcare, finance, real estate, and insurance. The platform exposes a REST API at `app.phonely.ai/api` for agent management and a post-call webhook that delivers structured JSON (transcript, summary, sentiment, action items, recording URL) to any HTTPS endpoint after each call. Prebuilt integrations cover Google Calendar, Salesforce, HubSpot, Five9, Zapier, Outlook, Slack, and Gmail; the visual workflow builder also supports importing arbitrary REST APIs from a curl command.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- AI, Artificial Intelligence, Voice AI, Voice Agents, Conversational AI, Telephony, Phone, Call Center, Contact Center, SMS, Webhooks, Workflow Automation, Scheduling, CRM

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Pricing Snapshot

| Plan | Monthly Price | Included Minutes | Overage / Minute |
|---|---|---|---|
| Free | $0 | 100 (~50 calls) | — (hard cap) |
| Starter | $50 ($33 annual) | 250 (~100 calls) | $0.25 |
| Pro | $150 ($100 annual) | 750 (~300 calls) | $0.30 |
| Enterprise | Custom | Custom | As low as $0.05 |

Post-transfer minutes (after handoff to a human) are billed at $0.02/minute on Starter and Pro. Pricing is usage-based — there is no per-agent seat fee.

## APIs

### Phonely Agents API

Manage Phonely voice agents programmatically. Retrieve a single agent or list all agents for a user, and update agent configuration including voice, greeting message, name, conversation style (Casual, Humorous, Direct, Formal, Persuasive, Friendly), humanization, and organization membership. Authenticated with an `X-Authorization` API key against the `app.phonely.ai/api` base.

**Human URL:** [https://docs.phonely.ai/api-reference/introduction](https://docs.phonely.ai/api-reference/introduction)

- [Documentation — Frontend API Introduction](https://docs.phonely.ai/api-reference/introduction)
- [Documentation — Get Agent](https://docs.phonely.ai/api-reference/endpoint/get-agent)
- [OpenAPI](openapi/phonely-agents-api-openapi.yml)
- [JSON Schema — Agent](json-schema/phonely-agent-schema.json)
- [JSON-LD](json-ld/phonely-context.jsonld)
- [Naftiko Capability — Agents](capabilities/agents-agents.yaml)
- [Example — Get Agent](examples/phonely-get-agent-example.json)
- [Example — Get Agents](examples/phonely-get-agents-example.json)
- [Example — Update Agent](examples/phonely-update-agent-example.json)

### Phonely Webhooks API

Receive structured post-call event data from Phonely after each AI voice interaction completes. The "Send Call Data" post-call workflow action POSTs a JSON payload containing call metadata, full transcript (text plus structured turns), AI-generated summary, purpose, topic, sentiment, key points, action items, follow-up indicators, mentioned entities (email, date, time), recording URL, and dashboard URL to any HTTPS endpoint you configure.

**Human URL:** [https://docs.phonely.ai/webhook-reference/intro](https://docs.phonely.ai/webhook-reference/intro)

- [Documentation — Webhook Intro](https://docs.phonely.ai/webhook-reference/intro)
- [Documentation — Post-Call Webhook](https://docs.phonely.ai/webhook-reference/endpoint/postcall-webhook)
- [AsyncAPI](asyncapi/phonely-webhooks-asyncapi.yml)
- [JSON Schema — Post-Call Event](json-schema/phonely-post-call-event-schema.json)
- [Example — Post-Call Event](examples/phonely-post-call-event-example.json)
- [Naftiko Capability — Post-Call](capabilities/webhooks-post-call.yaml)

## Artifacts

| Type | Location |
|---|---|
| APIs.json catalog | [apis.yml](apis.yml) |
| OpenAPI — Agents | [openapi/phonely-agents-api-openapi.yml](openapi/phonely-agents-api-openapi.yml) |
| AsyncAPI — Webhooks | [asyncapi/phonely-webhooks-asyncapi.yml](asyncapi/phonely-webhooks-asyncapi.yml) |
| JSON Schema — Agent | [json-schema/phonely-agent-schema.json](json-schema/phonely-agent-schema.json) |
| JSON Schema — Post-Call Event | [json-schema/phonely-post-call-event-schema.json](json-schema/phonely-post-call-event-schema.json) |
| JSON-LD context | [json-ld/phonely-context.jsonld](json-ld/phonely-context.jsonld) |
| Examples | [examples/](examples/) |
| Naftiko capabilities | [capabilities/](capabilities/) |
| Spectral ruleset | [rules/phonely-rules.yml](rules/phonely-rules.yml) |
| Vocabulary | [vocabulary/phonely-vocabulary.yml](vocabulary/phonely-vocabulary.yml) |
| Plans (API Commons Plans 0.1) | [plans/phonely-plans-pricing.yml](plans/phonely-plans-pricing.yml) |
| Rate Limits (API Commons Rate Limits 0.1) | [rate-limits/phonely-rate-limits.yml](rate-limits/phonely-rate-limits.yml) |
| FinOps (FOCUS 1.3 aligned) | [finops/phonely-finops.yml](finops/phonely-finops.yml) |

## Common Links

- [Portal](https://www.phonely.ai)
- [Documentation](https://docs.phonely.ai)
- [Developer Platform](https://www.phonely.ai/developer)
- [Getting Started](https://docs.phonely.ai/get-started/quick-start)
- [Changelog](https://www.phonely.ai/dev/changelog)
- [Pricing](https://www.phonely.ai/pricing)
- [App / Sign Up](https://app.phonely.ai)
- [Blog](https://www.phonely.ai/blogs)
- [LinkedIn](https://www.linkedin.com/company/phonely-ai)
- [Twilio Case Study](https://customers.twilio.com/en-us/phonely)

## Maintainers

- Kin Lane — [apievangelist.com](https://apievangelist.com)

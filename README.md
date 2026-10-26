# Phonely (phonely)

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

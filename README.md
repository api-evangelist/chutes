# Chutes (chutes)

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

Chutes is a permissionless, serverless AI compute platform that lets developers deploy and run any model as an autoscaling "chute" on decentralized GPU capacity (Bittensor Subnet 64). It exposes a single OpenAI-compatible inference endpoint at llm.chutes.ai/v1 for hundreds of open-source LLMs, plus a management REST API at api.chutes.ai for building images and deploying, listing, and operating chutes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/apis.yml)

> Chutes runs on the Bittensor network as Subnet 64: model inference is served by a decentralized pool of GPU miners, and compute is incentivized in TAO. This is why some models are free or unusually cheap, and why pricing fluctuates with subnet economics.

## Tags

- AI
- LLM
- Inference
- Serverless
- GPU
- Bittensor

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Chutes LLM Inference (Chat Completions) API

OpenAI-compatible chat completions across hundreds of open-source models (DeepSeek, Qwen, Llama, GLM, Mistral, and more) served on the Chutes network at a single shared endpoint, with streaming, tool use, and a drop-in OpenAI client.

- **Human URL:** [https://chutes.ai/docs/examples/llm-chat](https://chutes.ai/docs/examples/llm-chat)
- **Base URL:** `https://llm.chutes.ai/v1`

#### Tags

- Chat
- Completions
- LLM

#### Properties

- [Documentation](https://chutes.ai/docs/examples/llm-chat)
- [API Reference](https://chutes.ai/docs/api-reference/overview)
- [OpenAPI](openapi/chutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/chutes-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/chutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chutes Image / Other Models API

Image generation (diffusion), embeddings, audio, and other non-chat model workloads are exposed as user-defined "cords" (decorated HTTP endpoints) on each deployed chute, plus templated vLLM and diffusion deploy helpers.

- **Human URL:** [https://chutes.ai/docs/templates/vllm](https://chutes.ai/docs/templates/vllm)
- **Base URL:** `https://api.chutes.ai`

#### Tags

- Image
- Diffusion
- Multimodal

#### Properties

- [Documentation](https://chutes.ai/docs/core-concepts/cords)
- [API Reference](https://chutes.ai/docs/api-reference/overview)
- [OpenAPI](openapi/chutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chutes Management (Deploy / List) API

REST API to list, retrieve, deploy, update, and delete chutes (serverless AI apps), plus templated vLLM/diffusion deploys, warmup, utilization, miner means, and TEE attestation evidence.

- **Human URL:** [https://chutes.ai/docs/api-reference/chutes](https://chutes.ai/docs/api-reference/chutes)
- **Base URL:** `https://api.chutes.ai`

#### Tags

- Management
- Deploy
- Serverless

#### Properties

- [Documentation](https://chutes.ai/docs/getting-started/running-a-chute)
- [API Reference](https://chutes.ai/docs/api-reference/chutes)
- [OpenAPI](openapi/chutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Chutes Images API

Create, list, retrieve, and delete container images that chutes run from; image creation stores metadata and kicks off an asynchronous build that is published to the Chutes registry.

- **Human URL:** [https://chutes.ai/docs/api-reference/images](https://chutes.ai/docs/api-reference/images)
- **Base URL:** `https://api.chutes.ai`

#### Tags

- Images
- Build
- Containers

#### Properties

- [Documentation](https://chutes.ai/docs/core-concepts/templates)
- [API Reference](https://chutes.ai/docs/api-reference/images)
- [OpenAPI](openapi/chutes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/chutes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/chutes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/rayonlabs)
- [LinkedIn](https://www.linkedin.com/company/chutesai)
- [Website](https://chutes.ai/)
- [Documentation](https://chutes.ai/docs)
- [Plans](plans/chutes-plans-pricing.yml)
- [Rate Limits](rate-limits/chutes-rate-limits.yml)
- [Fin Ops](finops/chutes-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

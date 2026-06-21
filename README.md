# Chutes (chutes)

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

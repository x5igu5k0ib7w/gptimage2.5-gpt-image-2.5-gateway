# GPT Image 2.5 API (gpt-image-2.5 / gptimage2.5) — gateway guide with published pricing

<p align="center">
  <img src="hero.jpg" width="820" alt="GPT Image 2.5 sample">
</p>

> **flare@1K $0.0085; sunburst@1K $0.0085; flare@2K $0.014** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://apimart.ai/pricing)** · **[Get an API key](https://apimart.ai/keys)**

Everything here refers to **gpt-image-2.5** — also written **gptimage2.5** or **gpt image 2.5**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `flare@1K` | $0.0085 |
| `sunburst@1K` | $0.0085 |
| `flare@2K` | $0.014 |
| `sunburst@2K` | $0.014 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $0.85 |
| 1,000 | $8.5 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"gpt-image-2.5-ext","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.

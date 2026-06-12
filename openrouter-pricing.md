# OpenRouter Pricing Explained

This page summarizes how **OpenRouter pricing** works so you can compare it with **direct provider pricing** and **API gateways**.

## How OpenRouter charges

- **Per-model rates** — each model has its own input/output price on the OpenRouter catalog
- **Credits / balance** — you top up and spend down per request
- **Variable markup** — aggregator pricing can differ from the provider’s official list price

Check current numbers on the OpenRouter site; rates change when upstream providers change.

## What drives your bill

| Factor | Effect |
|--------|--------|
| Input tokens | Charged per 1M (or per 1K) tokens on the model you select |
| Output tokens | Often 2–4× input price depending on model |
| Model tier | Flagship models cost more than flash / small models |
| Peak usage | Rate limits may force retries or queueing (indirect cost) |

## OpenRouter vs direct provider pricing

| | OpenRouter | Direct provider |
|---|------------|-----------------|
| Price source | OpenRouter model page | Provider official pricing |
| Billing | Single OpenRouter balance | Provider account |
| Transparency | One dashboard | Per-provider invoices |
| Best when | Multi-model experiments | Single-provider production |

## OpenRouter vs API gateway pricing

Some **API gateways** resell upstream models with their own credit system (often OpenAI-compatible). Compare:

1. **List price** — official provider $/1M tokens  
2. **Your effective rate** — after credits, packs, or minimum top-ups  
3. **Tooling** — retries, regions, and which models are actually enabled  

## DeepSeek-specific comparison

For coding stacks (Cursor, Cline, Continue, Aider), many teams compare:

- OpenRouter → `deepseek/...` routes  
- DeepSeek official API  
- An OpenAI-compatible gateway focused on DeepSeek routes  

See also: [OpenRouter vs DeepSeek](./openrouter-vs-deepseek.md)

## Related guides

- [OpenRouter Alternative](./README.md)
- [DeepSeek API Pricing](https://github.com/nanobridgerafa/deepseek-api-pricing) *(coming soon)*
- [Cline + DeepSeek](https://github.com/nanobridgerafa/cline-deepseek-guide)

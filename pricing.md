# Gemini Developer API Pricing

The Gemini API "free tier" is offered through the API service with lower rate limits for testing purposes. Google AI Studio usage is completely free in all available countries. The Gemini API "paid tier" comes with higher rate limits, additional features, and different data handling.

[Upgrade to the Paid Tier](billing.md)

If you're looking to reduce costs and your use case doesn't require immediate real-time responses, check out Batch Mode. Batch Mode is designed to process large volumes of requests asynchronously. Requests submitted using this mode are 50% of the price of interactive (non-batch mode) requests.

## Gemini 2.5 Pro

Our state-of-the-art multipurpose model, which excels at coding and complex reasoning tasks.

| Feature | Free Tier | Paid Tier, per 1M tokens in USD |
| --- | --- | --- |
| Input price | Free of charge | $1.25, prompts <= 200k tokens<br>$2.50, prompts > 200k tokens |
| Output price (including thinking tokens) | Free of charge | $10.00, prompts <= 200k tokens<br>$15.00, prompts > 200k |
| Context caching price | Not available | $0.31, prompts <= 200k tokens<br>$0.625, prompts > 200k<br>$4.50 / 1,000,000 tokens per hour (storage price) |
| Grounding with Google Search | Not available | 1,500 RPD (free), then $35 / 1,000 requests |
| Used to improve our products | Yes | No |

## Gemini 2.5 Flash

Our first hybrid reasoning model which supports a 1M token context window and has thinking budgets.

| Feature | Free Tier | Paid Tier, per 1M tokens in USD |
| --- | --- | --- |
| Input price | Free of charge | $0.30 (text / image / video)<br>$1.00 (audio) |
| Output price (including thinking tokens) | Free of charge | $2.50 |
| Context caching price | Not available | $0.075 (text / image / video)<br>$0.25 (audio)<br>$1.00 / 1,000,000 tokens per hour (storage price) |
| Grounding with Google Search | Free of charge, up to 500 RPD (limit shared with Flash-Lite RPD) | 1,500 RPD (free, limit shared with Flash-Lite RPD), then $35 / 1,000 requests |
| Live API | Free of charge | Input: $0.50 (text), $3.00 (audio / image [video])<br>Output: $2.00 (text), $12.00 (audio) |
| Used to improve our products | Yes | No |

## Gemini 2.5 Flash-Lite

Our smallest and most cost effective model, built for at scale usage.

| Feature | Free Tier | Paid Tier, per 1M tokens in USD |
| --- | --- | --- |
| Input price (text, image, video) | Free of charge | $0.10 (text / image / video)<br>$0.30 (audio) |
| Output price (including thinking tokens) | Free of charge | $0.40 |
| Context caching price | Not available | $0.025 (text / image / video)<br>$0.125 (audio)<br>$1.00 / 1,000,000 tokens per hour (storage price) |
| Grounding with Google Search | Free of charge, up to 500 RPD (limit shared with Flash RPD) | 1,500 RPD (free, limit shared with Flash RPD), then $35 / 1,000 requests |
| Used to improve our products | Yes | No |

**Notes:**

*   Google AI Studio usage is free of charge in all available regions.
*   Prices may differ from the prices listed here and the prices offered on Vertex AI. For Vertex prices, see the Vertex AI pricing page.
*   If you are using dynamic retrieval to optimize costs, only requests that contain at least one grounding support URL from the web in their response are charged for Grounding with Google Search. Costs for Gemini always apply. Rate limits are subject to change.
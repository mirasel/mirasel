# Mominul Islam Rasal

Backend engineer, 5 years. Golang, Node.js, TypeScript. I build e-commerce platforms, marketplace integrations, and payment flows that carry real transaction volume.

**Currently:** Software Engineer III at [Pathao](https://pathao.com) — Bangladesh's largest super app.

### What I work on

Most of my work lives in private and self-hosted repositories, so here's what it actually is:

**Pathao Commerce** — merchant platform, 30,000+ active merchants, 4,000+ online stores. I own the multi-channel sales architecture: a channel-agnostic adapter layer in Go that lets merchants manage their storefront and external marketplaces from one dashboard. I've shipped four production integrations on it — Daraz (OAuth 2.0 + HMAC-signed REST), Pathao Shop (OTP-verified internal channel), WooCommerce (consumer key/secret REST), and Shopify (GraphQL Admin API only, no REST fallback). Each one needed less bespoke code than the last, which was the point.

The Shopify integration is the one I'd talk about: a cost-throttled GraphQL client that reads `extensions.cost.throttleStatus` and backs off ahead of Shopify's leaky-bucket limiter, OAuth with constant-time HMAC callback verification, `productSet` publish, `inventorySetQuantities` batched at 250/call, raw-body-verified webhooks with 200-ack-then-async processing, and an hourly reconciliation cron as a backstop — because Shopify deletes a webhook subscription after 8 consecutive delivery failures.

**Pathao Shop** — the e-commerce vertical of the super app. I built the backend from an empty repo: 13+ microservices and 3 web apps, now serving 500,000+ daily users. Cut API response times from ~1s to ~80ms with Redis caching, query parallelization, strategic indexes, and materialized views. Led the platform's first multi-country expansion into Nepal, threading country-aware auth, routing, currency, address validation, and logistics through every service and all three frontends.

**Before that** — real-time audio and transcription infrastructure at Augmedix for a US healthcare AI product (Socket.IO + Deepgram ASR streaming, MPEG-DASH on GCP, HIPAA-compliant PHI handling), and DHL, Stripe, and custom Shopify app integrations at BJIT.

### Stack

`Go` `Node.js` `TypeScript` `PostgreSQL` `Redis` `Meilisearch` `Elasticsearch` `BullMQ` `RabbitMQ` `Kafka` `Docker` `Kubernetes` `Helm` `GCP (GKE, Pub/Sub)` `AWS` `GitLab CI/CD` `REST & GraphQL`

### Things I'm opinionated about

- Adapter boundaries earn their keep on integration #3, not #2
- Webhook handlers should ack in 200ms and do the work somewhere else
- A reconciliation cron is not admitting defeat, it's admitting the network exists
- Rate limiters are a cost model, not an error condition — read the budget, back off before you're throttled

💼 [LinkedIn](https://linkedin.com/in/mominul-islam-rasel) · ✉️ mominulislamrasel@gmail.com

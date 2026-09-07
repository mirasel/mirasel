<div align="center">

# Mominul Islam Rasal

### Backend Engineer · Go · Node.js · TypeScript

*I build backends that carry real transaction volume*

<p>
<a href="https://linkedin.com/in/mominul-islam-rasel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:mominulislamrasel@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<img src="https://img.shields.io/badge/Dhaka,%20Bangladesh-006A4E?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
</p>

<p>
<img src="https://img.shields.io/badge/4-marketplace%20channels-8250DF?style=flat-square" />
<img src="https://img.shields.io/badge/30,000+-merchants-2F81F7?style=flat-square" />
<img src="https://img.shields.io/badge/13+-microservices-1F6FEB?style=flat-square" />
<img src="https://img.shields.io/badge/500,000+-daily%20users-2DA44E?style=flat-square" />
</p>

</div>

---

## 🙋 About Me

I'm a backend engineer with **5 years** building systems that move real money and real inventory — e-commerce platforms, marketplace integrations, and payment flows.

Right now I'm **Software Engineer III at [Pathao](https://pathao.com)**, Bangladesh's largest super app, where I own the multi-channel commerce layer that connects merchants to external marketplaces.

What I actually enjoy: third-party API integration under real constraints — OAuth, HMAC signing, webhook idempotency, cost-based rate limiting, and the reconciliation you need when the network refuses to cooperate. Plus the unglamorous part that makes it work: PostgreSQL schema design, caching, and shipping to Kubernetes.

> 📦 Most of my work lives in private and self-hosted repositories, so the sections below describe what I built rather than link to it.

---

## 🏗️ What I work on

### 🛒 [Pathao Commerce](https://commerce.pathao.com)

<img src="https://img.shields.io/badge/30,000+-active%20merchants-2F81F7?style=flat-square" /> <img src="https://img.shields.io/badge/4,000+-online%20stores-1F6FEB?style=flat-square" /> <img src="https://img.shields.io/badge/4-marketplace%20channels-8250DF?style=flat-square" />

Merchant platform. I own the **multi-channel sales architecture** — a channel-agnostic adapter layer in Go that lets merchants manage their storefront and external marketplaces from one dashboard.

I've shipped four production integrations on it:

| Channel | Auth model | Notable |
| :--- | :--- | :--- |
| 🟠 **Daraz** | OAuth 2.0 + HMAC-signed REST | Bidirectional inventory sync, scheduled token refresh |
| 🔴 **Pathao Shop** | OTP-verified internal channel | Full merchant self-service onboarding, Nepal rollout |
| 🟣 **WooCommerce** | Consumer key/secret REST | Shipped end-to-end in under three weeks |
| 🟢 **Shopify** | GraphQL Admin API only | Cost-throttled client, no REST fallback |

Also designed the multi-channel database schema — sales channels, channel listings, webhook audit trail, warehouse-channel bindings, and channel-scoped category mappings.

### 🏪 [Pathao Shop](https://shop.pathao.com)

<img src="https://img.shields.io/badge/13+-microservices-2F81F7?style=flat-square" /> <img src="https://img.shields.io/badge/500,000+-daily%20users-1F6FEB?style=flat-square" /> <img src="https://img.shields.io/badge/~1s%20→%20~80ms-API%20latency-2DA44E?style=flat-square" />

The e-commerce vertical of the super app. I built the backend **from an empty repo**: 13+ microservices and 3 web apps.

- ⚡ Cut API response times from ~1s to ~80ms — Redis caching, query parallelization, strategic indexes, materialized views
- 🌏 Led the platform's first **multi-country expansion into Nepal**, threading country-aware auth, routing, currency, address validation, and logistics through every service and all three frontends

### 🩺 Before that

**Augmedix** — real-time audio and transcription infrastructure for a US healthcare AI product. Socket.IO + Deepgram ASR streaming, MPEG-DASH on GCP, HIPAA-compliant PHI handling.

**BJIT** — DHL, Stripe, and custom Shopify app integrations.

---

## 🧰 Stack

**Languages & Runtime**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Data, Search & Queues**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
![Meilisearch](https://img.shields.io/badge/Meilisearch-FF5CAA?style=for-the-badge&logo=meilisearch&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-D63B3B?style=for-the-badge&logo=redis&logoColor=white)

**Infra & Cloud**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

---

<div align="center">

### 📫 Say hi

<a href="https://linkedin.com/in/mominul-islam-rasel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:mominulislamrasel@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

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

I'm a backend engineer with **5+ years** building systems that move real money and real inventory — e-commerce platforms, marketplace integrations, and payment flows.

Right now I'm **Software Engineer III at [Pathao](https://pathao.com)**, Bangladesh's largest super app, where I own the multi-channel commerce layer that connects merchants to external marketplaces.

What I actually enjoy: third-party API integration under real constraints — OAuth, HMAC signing, webhook idempotency, cost-based rate limiting, and the reconciliation you need when the network refuses to cooperate. Plus the unglamorous part that makes it work: PostgreSQL schema design, caching, and shipping to Kubernetes.

> 📦 Most of my work lives in private and self-hosted repositories, so the sections below describe what I built rather than link to it.

---

## 🏗️ What I work on

### 🛒 [Pathao Commerce](https://commerce.pathao.com)

<img src="https://img.shields.io/badge/30,000+-active%20merchants-2F81F7?style=flat-square" /> <img src="https://img.shields.io/badge/4,000+-online%20stores-1F6FEB?style=flat-square" /> <img src="https://img.shields.io/badge/125,000+-deliveries-8250DF?style=flat-square" /> <img src="https://img.shields.io/badge/100,000+-instant%20checkouts-2DA44E?style=flat-square" />

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

<img src="https://img.shields.io/badge/13+-microservices-2F81F7?style=flat-square" /> <img src="https://img.shields.io/badge/500,000+-daily%20users-1F6FEB?style=flat-square" /> <img src="https://img.shields.io/badge/~1s%20→%20~80ms-API%20latency-2DA44E?style=flat-square" /> <img src="https://img.shields.io/badge/117,000+-lines%20shipped-8250DF?style=flat-square" /> <img src="https://img.shields.io/badge/656-commits-6E7681?style=flat-square" />

The e-commerce vertical of the super app. I built the backend **from an empty repo**: 13+ microservices and 3 web apps, 117,000+ lines of TypeScript and Go across 656 commits over 18 months.

- ⚡ **Performance** — cut API response times from ~1s to ~80ms with Redis caching, query parallelization, strategic indexes, and materialized views
- 🌏 **Nepal launch** — led the platform's first multi-country expansion, threading country-aware auth, routing, currency, address validation, and logistics through every service and all three frontends
- 💳 **Payments & checkout** — idempotent checkout and order placement across Pathao Pay, digital gateways, and cash-on-delivery, with Pathao Courier fulfillment webhooks: 1,000+ daily transactions, zero data inconsistencies
- 🔐 **Auth** — JWT middleware across every API service, bcrypt hashing, OTP request/attempt limits, role-based backoffice access, email-token password reset
- 🔎 **Search** — Meilisearch microservice at sub-100ms, async BullMQ index sync, autocomplete and trending suggestions
- 📦 **Bulk import & media** — CSV/XLSX catalog import with multi-layer validation and BullMQ batch processing, plus an automated pipeline generating 512/1200/2400px renditions with idempotency checks and retry
- 🎟️ **Promo engine** — spanning the Node.js monorepo and a standalone Go microservice: budget enforcement, per-user usage limits, checkout integration, scheduled campaigns
- 🚢 **CI/CD** — GitLab CI deploying 12 Dockerized services to GKE with Turborepo selective builds, 40% faster deploys, independent zero-downtime releases

### 🩺 Before that

**Augmedix** — real-time audio and transcription infrastructure for a US healthcare AI product. Socket.IO + Deepgram ASR streaming, MPEG-DASH on GCP, HIPAA-compliant PHI handling. The platform saved clinicians **1+ hour of daily EHR documentation**, with 94% reporting better focus on patients.

**BJIT** — DHL, Stripe, and custom Shopify app integrations for UK and EU e-commerce clients.

---

## 🧰 Stack

**Languages & Frameworks**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![tRPC](https://img.shields.io/badge/tRPC-2596BE?style=for-the-badge&logo=trpc&logoColor=white)

**Data, Search & Queues**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white)
![Meilisearch](https://img.shields.io/badge/Meilisearch-FF5CAA?style=for-the-badge&logo=meilisearch&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-D63B3B?style=for-the-badge&logo=redis&logoColor=white)

**Infra & Cloud**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

**Frontend** *(working knowledge)*

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Ant Design](https://img.shields.io/badge/Ant%20Design-0170FE?style=for-the-badge&logo=antdesign&logoColor=white)

---

## 🎓 Education & Certifications

- **BSc, Computer Science & Engineering** — Rajshahi University of Engineering & Technology, 2021
- **IELTS Academic** — Overall Band 7.0 (CEFR C1), Feb 2026
- **Scrum Team Member Accredited Certification™** — International Scrum Institute™
- 200+ problems solved on LeetCode, AlgoExpert, and Codeforces

---

<div align="center">

### 📫 Say hi

<a href="https://linkedin.com/in/mominul-islam-rasel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:mominulislamrasel@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

# Hi, I'm Miguel Angel Buitrago Castillo

Engineering Lead at a national retail and distribution company in Colombia. I run a small team — one frontend developer and one UX/UI designer — and I still write code every day. I'm not a manager who used to ship; I'm an engineer who happens to lead.

My team is currently moving the company's frontends onto a modern Nuxt 4 + Vue 3 stack — the legacy ERP, the order placement app used by our salespeople, the B2C marketplace, and the company website. While that migration runs, I personally own and maintain the dozen-plus backend services that keep the business operating: gateways, auth, commerce, search, inventory, notifications, ticketing, real-time event routing, and the AI layer that ties them together.

---

## What I actually work on

I'm in the middle of a long, deliberate migration: a legacy **Sails.js** API gateway is being replaced, route by route, with a clean **Fastify + TypeScript** gateway. Same story on the frontend — **Vue 2** to **Nuxt 4 + Vue 3** with Pinia. Migrations like this only work when you respect what already runs in production, so most of my week is split between writing new code and carefully retiring old code without breaking anyone's workflow.

On the backend, I build and maintain:

- An **authentication and session layer** with module-level access control across our platform.
- A **multi-tenant commerce and reservation backend** in NestJS, handling orders and DIAN-integrated electronic invoicing for tenants across the country.
- Two **Go** services — one for product search and combos, another for stock auditing across our warehouses. Go is the right tool when latency and throughput are non-negotiable.
- A **notification service** that does multi-account SMTP email delivery and an in-product inbox via Server-Sent Events.
- A **ticket management service** with AI-powered triage using OpenAI, plus escalation hooks.
- **Real-time event routing** between desktops, mobile clients, and thermal printers using Socket.IO and Redis pub/sub.
- **Thermal print job orchestration** driven by Kafka, because retail runs on receipts.

The part I'm most excited about lately is the **AI layer**. I built a unified gateway that routes chat and completion traffic to Anthropic Claude or OpenAI, persists conversations, and tracks usage. On top of that sits an **MCP (Model Context Protocol) server** that exposes our platform's data — products, hierarchies, warehouses — to AI clients like Claude Code. It means our internal tools can answer real business questions against live data, with tool use and conversation memory, instead of guessing.

On mobile, I maintain an **internal iOS app** in Swift and SwiftUI used by staff on the floor. It's the only Swift in my stack — everything else is TypeScript, Go, or JavaScript.

---

## Tech I reach for

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Swift](https://img.shields.io/badge/Swift-FA7343?style=flat&logo=swift&logoColor=white)

![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat&logo=fastify&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)

![Nuxt](https://img.shields.io/badge/Nuxt%204-00DC82?style=flat&logo=nuxt.js&logoColor=white)
![Vue 3](https://img.shields.io/badge/Vue%203-4FC08D?style=flat&logo=vue.js&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat&logo=pinia&logoColor=black)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0066CC?style=flat&logo=swift&logoColor=white)

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white)
![Kysely](https://img.shields.io/badge/Kysely-1E40AF?style=flat&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)

![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat&logo=socket.io&logoColor=white)

![Anthropic](https://img.shields.io/badge/Anthropic%20Claude-D97757?style=flat&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/Model%20Context%20Protocol-6E56CF?style=flat&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)

---

## How I think about the work

A few things I genuinely believe after a few years of doing this:

**Multi-tenant data is a discipline, not a feature.** Most of our databases are split per tenant or per warehouse location, with dedicated connection pools. Get that wrong once and you spend a week apologizing. Get it right and the platform scales quietly.

**Migrations should be boring on purpose.** Nobody gets a medal for a big-bang rewrite. The Sails-to-Fastify and Vue 2-to-Nuxt 4 transitions both work because every step is small, reversible, and observable. Prometheus on every service is non-negotiable.

**AI is most useful when it has real context.** A chatbot is a toy. A model with structured access to your inventory, your customers, and your orders — through MCP, with proper tool use — is leverage. That's where I've been spending the interesting hours lately.

**Leading a small team means clearing the runway.** My job is to make sure my frontend developer and designer can do their best work without tripping over backend issues, deployment friction, or unclear product direction. The code I write should make their code easier, not the other way around.

---

## Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mbuitragocdev&show_icons=true&hide_title=true&theme=radical" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mbuitragocdev&layout=compact&theme=radical" alt="Top languages" />
</p>

---

## Off the clock

Outside of work I read a lot of manga — I love how visual storytelling can compress so much character and motion into a single panel. Weekends are usually football with friends. The rest of the time I'm probably being supervised by my dog and my cat, who have very firm opinions about screen time.

If you want to talk shop — gateways, AI tooling, multi-tenant headaches, or how to keep a small team shipping — find me on [LinkedIn](https://www.linkedin.com/in/mbuitragoc/).

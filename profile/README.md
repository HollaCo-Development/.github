<div align="center">

  <img src="https://itipjzcggtzxrjxookes.supabase.co/storage/v1/object/public/site-logos/Holla_brand_2,7x3in_300dpi.png" alt="HollaCo" width="200" />

  # HollaCo Development Group

  ### Near-real-time conversations with the creators you follow.

  Powered by AI · delivered in AR · designed for presence.

  [hollaco.com](https://hollaco.com) — [collections.hollaco.com](https://collections.hollaco.com)

</div>

---

## The product

Imagine a creator's avatar standing in your living room. Their content plays on an image plane in front of them. You can pause at any moment and have a real conversation with them — through an AI that knows their work, their voice, and the context of what you're watching. It feels like the person is actually there.

That's HollaCo: a platform that turns recorded creator content into interactive, presence-rich experiences delivered to **AR mobile**, **VR headsets**, and **desktop** — without losing the immediacy of a live conversation.

## The platform

| Surface | Role |
|---|---|
| **Collections** | Discovery + subscription storefront. Find creators, subscribe to their catalogs, launch the experience. |
| **Babylon App** | AR/VR/Desktop client where the actual conversation happens. WebGL + WebXR; iOS, Android, Windows, headsets. |
| **Account** | Self-service billing, subscriptions, profile management. |
| **Auth** | Identity gateway — SSO, magic link, OTP, push, TOTP. |
| **Authenticator** | Native mobile companion for push-based multi-factor. |

## Built on

**Frontend** — Next.js (App Router), React, Tailwind, BabylonJS for the immersive layer
**Cloud** — Microsoft Azure (Static Web Apps, Front Door + WAF, Container Apps, Blob, Data Lake, Entra ID)
**Data** — Supabase (PostgreSQL + Realtime + Edge Functions + pgvector), Stripe for commerce
**AI** — Anthropic Claude, ElevenLabs voice, OpenAI embeddings, Firecrawl ingestion
**Mobile** — React Native, Expo, EAS Build, Sentry
**Automation** — n8n orchestration, GitHub Actions, Azure DevOps

## How we work

- Multi-environment delivery — `develop` → `staging` → `main` on every surface, gated by automated checks
- Row-level security enforced at the database layer, with least-privilege grants — not application-side checks
- Edge protection via Azure Front Door WAF in prevention mode; centralised observability through Microsoft Sentinel
- Continuous dependency-vulnerability tracking — high/critical CVEs auto-file tracked work items
- AI-assisted engineering across the stack: design, code review, error remediation, content ingestion

## Get in touch

- 🌐 Main site — [hollaco.com](https://hollaco.com)
- ✉️ Partnerships, press, careers — [developer@hollaco.com](mailto:developer@hollaco.com)

---

<sub>© HollaCo Holdings, Inc. · All rights reserved.</sub>

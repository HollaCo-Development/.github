<div align="center">

  <img src="HollaCo_logo_1024.png" alt="HollaCo" width="180" />

  # HollaCo Development Group

  ### Near-real-time conversations with the creators you follow.

  Powered by AI · delivered in AR · designed for presence.

  [hollaco.com](https://hollaco.com) — [collections.hollaco.com](https://collections.hollaco.com)

</div>

---

## The product

Imagine a creator's digital twin standing in your living room. Their content plays on an image plane in front of them. You can pause at any moment and have a real conversation with them — through an AI that knows their work, their voice, and the context of what you're watching. It feels like the person is actually there.

That's HollaCo: a platform that turns recorded creator content into interactive, presence-rich experiences delivered to **AR mobile**, **VR headsets**, and **desktop** — without losing the immediacy of a live conversation.

## The platform

| Surface | Role |
|---|---|
| **Collections** | Discovery + subscription storefront. Find creators, subscribe to their catalogs, launch the experience. Next.js on `collections.hollaco.com`. |
| **Babylon XR** | The immersive client where the conversation happens — Babylon.js 7 + WebXR, with n8n-driven realtime media sync and an MCP scene bridge. iOS, Android, Windows, headsets, at `xr.collections.hollaco.com`. |
| **XR Shell** | Capacitor native launcher that makes OS-level push reliable on iOS/Android, then hands off into the WebXR scene in a real browser. |
| **Account** | Self-service billing, subscriptions, and profile management — Azure Static Web Apps fronting a Stripe Edge Function suite. `account.hollaco.com`. |
| **Auth** | Identity gateway — SSO (Google/Apple/Microsoft), magic link, OTP, push-to-approve. Webflow + Supabase, no paid middleware. `auth.hollaco.com`. |
| **Authenticator** | React Native + Expo companion for TOTP and push-based multi-factor, with biometric approval and SecureStore-backed secrets. |
| **Developer Hub** | Engineering coordination — Azure DevOps errata board with auto-filed work items from advisories and security findings. |

## Built on

**Frontend** — Next.js (App Router), React, Tailwind, BabylonJS for the immersive layer; Webflow + Azure Static Web Apps for the auth/account surfaces
**Cloud** — Microsoft Azure (Static Web Apps, Front Door + WAF, Container Apps, Blob, Data Lake, Entra ID)
**Data** — Supabase (PostgreSQL + Realtime + Edge Functions + pgvector), Stripe for commerce
**AI** — Anthropic Claude, ElevenLabs voice, OpenAI embeddings, Firecrawl ingestion
**Mobile** — React Native, Expo, EAS Build, Capacitor, Sentry
**Automation** — n8n orchestration, GitHub Actions, Azure DevOps

## How we work

- Multi-environment delivery — `develop` → `staging` → `main` on every surface, gated by automated checks
- Row-level security enforced at the database layer, with least-privilege grants — not application-side checks
- Pinned, SRI-verified CDN dependencies; open-redirect and email-enumeration protections baked into the auth layer
- Scheduled security scanning on every repo — bi-weekly passive (OWASP ZAP, Playwright, security headers, SRI) and monthly deep scans (ZAP active, TruffleHog secret history, dependency audit)
- Edge protection via Azure Front Door WAF in prevention mode; centralised observability through Microsoft Sentinel
- Continuous dependency-vulnerability tracking — high/critical CVEs auto-file tracked Azure DevOps work items
- AI-assisted engineering across the stack: design, code review, error remediation, content ingestion

## Get in touch

- 🌐 Main site — [hollaco.com](https://hollaco.com)
- ✉️ Partnerships, press, careers — [developer@hollaco.com](mailto:developer@hollaco.com)

---

<sub>© HollaCo Holdings, Inc. · All rights reserved.</sub>

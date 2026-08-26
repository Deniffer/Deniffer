# Deniffer Liu

**Full-stack, agent & growth engineer.** Co-founder & CEO of
Celados — an AI-native product studio building for the
agent era. Previously ByteDance (TikTok Live) and A1D.

I ship consumer AI products and the tooling that makes agents useful — across
iOS, web, Cloudflare, and the Canva Marketplace.

📍 Remote · Shenzhen  ·  ✉️ deniffer.001@gmail.com  ·  🐦 [@lumina\_\_team](https://x.com/lumina__team)

## What I'm building at Celados

| Project | What it is |
| --- | --- |
| [**ctx**](https://github.com/celados/ctx) | Full-document search and reading for AI agents — finds curated library docs, searches the open web, and returns complete sources instead of RAG fragments. |
| [**gkit**](https://github.com/celados/gkit) | Agent-first growth CLI — one profile-bound surface over DataForSEO, PostHog, Google Ads, Search Console, and Bing Webmaster, with offline capability discovery. |

Currently building **[Clonesite AI](https://clonesite.ai)** and
**[ExportFramer](https://exportframer.com)**.

**[Clonesite AI](https://clonesite.ai)** — turns any public website into an
editable React + Tailwind project. Own the code, skip the blank canvas, and ship
faster instead of rebuilding from scratch.

**[ExportFramer](https://exportframer.com)** — take your Framer site beyond
Framer. Export it to standalone HTML or React, preview the full result, and host
or extend it anywhere.

**prism** — local router daemon that puts agentic CLIs (Claude Code, Codex) on
third-party Anthropic/OpenAI-compatible endpoints. Binds `127.0.0.1`, routes each
request by `(inbound family prefix + body.model)` to the right upstream, rewrites
only the URL, auth headers, and `body.model`, then streams the response straight
back. Deliberately *not* a protocol translator — each wire (`anthropic`,
`openai-chat`, `openai-responses`) is forwarded to an upstream that natively
speaks it, which keeps streaming and tool-call semantics intact. Rust; ships
prebuilt macOS arm64 / Linux musl binaries and a multi-arch Docker image, and
refuses to start on a non-loopback bind without an active API key so an exposed
port can never leak upstream credentials.

**mcpx** — turns registered MCP servers into an agent-friendly command surface.
Keeps registrations in a global user registry, discovers tool schemas, handles
OAuth where it can, and exposes each server as a root command
(`mcpx posthog projects-get`). Schema-first and explicit by design: tool input
goes through `--input`, while mcpx's own control commands stay namespaced under
`@` so they can never collide with a server's tools. Bun, single-binary install.

## Previously

**A1D** — Full-Stack Engineer · 2024-09 – 2026-05 · remote, US startup

Primary engineer across a consumer AI product line:

- **RizzPlus / AI Dating Keyboard** — iOS AI messaging assistant, Swift, built
  solo; still earning subscription revenue.
- **Speed Painter for Canva** — lead engineer on the Canva Marketplace app.
- **Caption AI**, **ClosetCue AI**, **Wearly** — AIGC web apps, built solo.
- **Revival** — Twitter growth automation. An MV3 extension (WXT + React) runs
  scheduled posts, AI-drafted replies, and engagement actions off a server-side
  task queue (Bun + Hono + oRPC, Inngest jobs), idempotent with backoff retries
  against rate limits and PostHog-instrumented throughout.
- Low-code email delivery on AWS SES + Cloudflare Workers + Lark base tables,
  ~80% cheaper to build and maintain than a conventional stack.

**ByteDance** — Software Engineer, TikTok Live · 2022-01 – 2024-01 · Beijing

- State machine managing UI logic across PK (live battle) stages — ~50% less
  code complexity.
- Multi-device log synchronization tool — ~60% faster troubleshooting.
- Feature iterations with cross-functional teams — ~25% lift in in-stream
  engagement.

## Stack

**Languages** TypeScript · Swift · Objective-C
**Web** React · Next.js · TanStack Start · Vite · Tailwind · Node.js · Bun
**Mobile** Swift / SwiftUI · Flutter
**Data** Convex · PostgreSQL · ClickHouse · DuckDB
**Cloud** Cloudflare (Workers, Queues, D1, Browser Rendering) · AWS · Docker
**AI & agents** LLM application engineering · agent harnesses · MCP servers &
clients · image/video generation pipelines · context engineering
**Growth** SEO · ASO · PostHog · Stripe / RevenueCat

## Education

**BSc, Information and Computing Science** — Guangdong Ocean University, 2017–2021
National Mathematical Modeling Contest, Second Prize ×2.
Self-directed: MIT 6.S081 · Stanford CS144 · UC Berkeley CS61B · nand2tetris.

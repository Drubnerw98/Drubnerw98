### Will Drubner — Boston, remote-friendly

Film → software. AI-native product work in TypeScript, plus solo-shipped production sites for real organizations.

The trilogy below — Resonance, Constellation, Ensemble — is a paired build around cross-format media taste. The Middlebury project is solo end-to-end for a real civic-advocacy group with real users.

---

**Next up**

Extending the Resonance backend with an MCP server so Claude and other agentic clients can recommend against a user's actual taste profile — turning the existing recommendation pipeline into a tool agents can call. Evaluation harness in the same repo.

**Shipped**

- [**Resonance**](https://github.com/Drubnerw98/Resonance) — cross-format AI recommendations grounded in a persistent taste profile. React 19 + Express + Neon Postgres + Clerk + Anthropic Claude. Multi-turn onboarding, 4-step pipeline validated against real APIs (TMDB / IGDB / Jikan / Open Library), library imports from Letterboxd / Goodreads / MyAnimeList / Steam. → [resonance-client.vercel.app](https://resonance-client.vercel.app)
- [**Constellation**](https://github.com/Drubnerw98/Constellation) — force-directed visualization of a Resonance profile. Themes as nebula clusters, per-theme MST constellation lines (Kruskal + union-find), three-tier fuzzy tag matching. Shares Clerk auth with Resonance and reads its `/api/profile/export`. → [constellation-alpha-eight.vercel.app/demo](https://constellation-alpha-eight.vercel.app/demo)
- [**Ensemble**](https://github.com/Drubnerw98/Ensemble) — real-time multi-user convergence on top of the same backend. Two or more Resonance users pull candidate titles into a shared session, vote with live presence (Liveblocks), and finalize on threshold cross. → [ensemble-sigma.vercel.app](https://ensemble-sigma.vercel.app)
- [**Middlebury Taxpayers**](https://github.com/Drubnerw98/MiddleburyLTA) — solo-built Next.js 15 + Firebase site for a civic-advocacy group. Tax-impact calculator with cited numeric constants, edge-middleware-gated admin, Zod-validated server actions, session-cookie auth with explicit revocation. Real client, real users. → [middleburytaxpayers.com](https://middleburytaxpayers.com)

---

**Stack** — TypeScript, React 19, Next.js, Node, Postgres, Firebase, Tailwind, Anthropic Claude API, D3, Liveblocks

**Approach** — On the trilogy I work with Claude as a pair programmer in Claude Code; architectural calls are mine and logged with reasoning in each repo (`decisions.md` in Ensemble, `ARCHITECTURE.md` in Resonance and Constellation). The Middlebury project is the end-to-end solo counterpart — same shipping bar, no AI pair.

**Reach me** — drubnerw98@gmail.com

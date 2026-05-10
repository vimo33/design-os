# Section: Timeline

## Purpose
The centerpiece. A vertical line draws as you scroll; project nodes appear on the line in chronological order. Year markers pulse. Status badges color-code by state.

## Content
All ~24 projects from the system registry, ordered by date. Year markers between groups.

## Year groupings (top to bottom)

### Mar 2025 — first builds
- **WollyShare Hub** — community item borrowing, full-stack (React + Supabase + Telegram bot) [archived · showcase]
- **Zurich Perspectives** — civic data storytelling, Next.js [archived · showcase]

### Sep–Dec 2025 — exploration phase
- **Impact Scout Core** — impact measurement / scouting [archived · public]
- **Focus Flow** — early Todo via Google AI Studio [archived · public]
- **Governance Assist** — governance prototype [concept]
- **Module 617** — German AI business course companion site [live · showcase]

### Jul 2025 — first paid AI consulting
- **Bad Schinznach AG — AI Advanced Leadership Accelerator** — 9-hour bespoke program · CHF 40,935 · 30-40 managers [delivered · service · showcase]

### Oct 2025 — teaching role + keynotes
- **BAIS Module 4 + 6 — Federal Certificate teaching** — Module 4 (5 days) + Module 6 (7 days) · CHF 11,400 dev fees · course launched 2025-10-18 [live · service · showcase]
- **The Aargau Advantage** — leadership playbook + Digital Days Aarau 2025 keynote [live · service · showcase]

### Apr 2025 — film
- **The Shape of Time** — Runway Gen:48 AI short film · Follow The Rabbit Studios [live · creative · showcase]

### Jan 2026 — volume
- **Sage AI + Sage** — likely AI advisory or KM tool [archived · private]
- **Focus Flow OS** — personal operating system, Telegram → Obsidian, Tailscale [in-dev · architecture-showcase]
- **SODA** — Next.js, 1 GitHub star [archived · public]

### Feb 2026 — concepts + research
- **Bramha + Atlas Studio** — decision-grade competitive intelligence research workflow platform for Swiss SMEs · Constitution v1.0.0 · 4-phase plan [in-dev · architecture-showcase]
- **Kavach AI / KavachVision** — edge CV for Indian factory CCTV [concept]
- **Global Foundation TCG** — non-profit foundation for ecstatic dance / breathwork [concept]

### Mar 2026 — client / showcase sprint
- **Multiplium Research Lab** — Regen-Viticulture Investment Intelligence V1 [live · showcase]
- **Ortho Landing** — landing page for Ortho-Analytic [archived · public]
- **Urban Fragments** — Gemini AI Studio art piece w/ Jasmin Hila [live · showcase]
- **Overture Website** — pitch site [archived · showcase]
- **Knowledge Base — Sure Thing** — personal AI strategy KB inspired by Nate B Jones [notes]

### Mar–Apr 2026 — concepts (vision-stage)
- **OpenAgent Protocol (OAP) / Intermesh Hotels** — Swiss Verein open hotel data layer [concept]

### Apr 2026 — bigger plays
- **Project Helios** — Family-Office due-diligence V2 of Multiplium · HITL UI · Expert Agents [in-dev · pilot · architecture-showcase]
- **The Front Door** — hospitality-specific website + AI-discoverability for Swiss SMEs · CHF 10k/mo target [in-dev · service]
- **intermesh** — semantic-matching engine for humans · MCP-native [in-dev]
- **Bildspur Inventory OS** — mobile-first inventory tool [live]

### May 2026 — most distinctive
- **Take Me There** — 3-wall AI portal installation · Electron + Three.js + Gemini API + MadMapper [live as desktop app · showcase]

### May 2026 — second brain + dashboard stack
- **brain-os** — Research Brain substrate (pgvector + nomic-embed-text + 6 capture pipelines + MCP server + dashboard + wiki synthesis + evolution agent) [live · architecture-showcase]
- **Home Dashboard** — internal command center replacing Homepage.dev [live]

## Animation
- Vertical SVG line on the left, fixed during this section, draws from top to bottom proportional to `scrollYProgress` within this section
- Each project node = a small dot on the line, glows + scales as it enters viewport
- Project card slides in from the right when the dot lights up
- Year markers — bigger, bolder, pulse once when they enter viewport
- Status badges colored: orange-500 (live), cyan-400 (in-dev), stone-400 (archived/concept)

## Layout
- Line at left ~80px from edge
- Project cards align right of the line, max-width ~700px
- Each card: project title (Space Grotesk), one-line description, stack tags (mono, cyan), status badge, optional URL/repo link

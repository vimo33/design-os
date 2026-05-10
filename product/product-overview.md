# Vikas Portfolio — Follow The Rabbit Studio

## Description
A scroll-driven public portfolio for Vikas (Tim Fuchs) — single creator working under the Bildspur / Follow The Rabbit Studio brand. Tells the story of one person evolving alongside AI: from first builds in 2025 to multi-agent systems, capture pipelines, films, and a Swiss SME consulting practice in 2026. The methodology is the differentiator — not the project list.

## Problems & Solutions

### Problem 1: Generic AI-builder portfolios all look the same
Most look like a Vercel landing page with project tiles. They show *what* was shipped but not *how* the person thinks. Solution: lead with the 7-phase research-build methodology (ChatGPT idea expansion → multi-model deep research → synthesis docs → Claude Code build → executor/reviewer two-agent pattern). The process is the centrepiece, projects are evidence.

### Problem 2: Older projects feel like clutter
March 2025 builds (WollyShare, Zurich Perspectives) sit alongside late-2026 multi-agent platforms. Solution: a vertical scroll-driven timeline where the line draws as you scroll. Older projects are framed as *capability milestones*, not embarrassments — they show the journey of evolving with AI.

### Problem 3: Most "AI portfolios" hide the technical practice
Hooks, MCP servers, skills, two-agent reviewer/executor — these are the actual differentiators. Solution: a dedicated "Explorations" section that surfaces the technical practice without giving away proprietary configs.

### Problem 4: Software-only portfolios miss the breadth
Vikas also does films (Runway Gen:48), installations (Take Me There — Electron + Three.js + MadMapper), and consulting (Bad Schinznach AG, BAIS Module 4+6). Solution: explicitly include all three tracks — software, creative, services — with the unifying frame "one person + AI doing what used to need a team".

### Problem 5: No portfolio surfaces the *research* habit
The deep-research-before-build practice is uncommon and signals strategic depth. Solution: explicitly document the 7-phase process as Section 1 of the journey, with the tools (ChatGPT, Gemini, Claude) and artifacts (PRDs, user journeys) named.

## Key Features
- Scroll-driven vertical timeline — line draws as you scroll, project nodes pop in along it
- 7-phase Method section visualised as a flow diagram with subtle animation
- Selected Work — 6 deep-dive feature cards (Take Me There, Bramha, Bad Schinznach, BAIS, Shape of Time, Multiplium → Helios) each with a unique embedded artifact (video, agent diagram, case-study infographic)
- Explorations log — technical patterns surfaced as code-flavoured cards: two-agent executor/reviewer, MCP, hooks, skills, brain-os
- Services panel — workshops, keynotes, BAIS modules with day rates
- Subtle craft signals — monospace timestamps, terminal-style cursors, tasteful section transitions
- Static export — zero CPU at idle, served by nginx on home Coolify
- Dark, futuristic, warm — orange + cyan accents on stone-warmed near-black, Space Grotesk + Inter + JetBrains Mono

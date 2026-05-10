# Section: Explorations

## Purpose
Surface the technical practice — the patterns that compound into capability. This is what most "AI builder" portfolios miss because they show *projects*, not *practices*.

## Content — 5 cards

### 1. Executor / Reviewer two-agent loop
Two Claude Code windows, same repo, different system prompts. Executor builds. Reviewer audits the diff against the master plan. Each pass catches what the other misses. Used for 50-hour build sessions on FTR-OS, brain-os, and the multi-agent portfolio. The reviewer's job isn't approval — it's catching scope drift, missed reviewer-checks, and consistency violations.
- **Code-flavored snippet:** `claude code (executor)  →  generates diff  →  claude code (reviewer)  →  audit per phase checklist  →  feedback to executor`

### 2. Brain-OS — pgvector + nomic-embed-text + 6 capture pipelines
A persistent semantic substrate. Capture pipelines (Telegram via openclaw, YouTube via Windmill, Claude Code SessionEnd hook, Meetily watcher, voice typing brain mode, Chrome extension) all flow into a single pgvector table indexed by HNSW. Wiki synthesis runs every Sunday — collapses raw nodes into curated wiki pages. Evolution agent flags stale concepts monthly.
- **Code-flavored snippet:** `nomic-embed-text · 768d · HNSW · vector_cosine_ops`

### 3. MCP — single source of truth across surfaces
Brain-MCP exposes search/list/capture/node-stats/wiki tools. Wired into Claude Desktop AND Claude Code AND the home dashboard AND the brain dashboard via the same single-tenant bearer token. Add a tool once, available everywhere. Makes the brain feel like a feature of the OS, not a separate app.
- **Code-flavored snippet:** `Hono + @modelcontextprotocol/sdk + WebStandardStreamableHTTPServerTransport`

### 4. Hooks + skills — keeping context warm
Claude Code SessionEnd hook reads the transcript JSONL, builds a digest of user prompts + files touched, captures as a brain node with auto-derived project_relevance. Skills (openclaw brain-capture) let Telegram messages flow directly into brain via Claude as classifier. Effect: nothing thought is lost between sessions.
- **Code-flavored snippet:** `~/.claude/hooks/brain-capture-session-end.py`

### 5. Coolify + cloudflared — single-PC self-hosting
Personal Bildspur-Lab Windows machine runs WSL2 Ubuntu, Docker, Coolify v4. 12+ apps deployed on the same network. Per-subdomain ingress in `/etc/cloudflared/config.yml`. Static apps idle at zero CPU. WSL keep-alive task ensures the tunnel never dies. Hetzner being decommissioned 2026-05-16+.
- **Code-flavored snippet:** `wsl tail -f /dev/null  ·  vmIdleTimeout=2147483647  ·  cloudflared tunnel: a3efcb3c-ade5-4296-93f0-dcee12d8acb0`

## Animation
- Each card has a small terminal-style header with `~/practice/[id]` and a blinking cursor
- Code snippets in mono, cyan-400 with subtle scan-line effect
- Cards animate in with a slight slide-up + fade

## Layout
- 2-column grid on desktop (collapses to single column mobile)
- Each card same height for visual rhythm

# Data Model

The portfolio is content-driven. All data lives in TypeScript modules; no database. The "nouns":

## Project
A single piece of work that may be live, in-dev, archived, or concept stage.

| Field | Type | Notes |
|---|---|---|
| id | slug | URL-safe |
| title | string | Display name |
| year | number | Used for timeline sort + year markers |
| month | number? | Optional finer-grained sort |
| track | "software" \| "creative" \| "service" \| "infra" | Which thread of work |
| status | "live" \| "in-dev" \| "archived" \| "concept" | Status badge color |
| visibility | "showcase" \| "public" \| "private" | Public/showcase shown; private gets architecture-only treatment |
| stack | string[] | Tech labels |
| description | string | One-liner shown on timeline |
| longDescription | string? | For deep-dive cards |
| url | string? | External live URL |
| repo | string? | GitHub repo (e.g. `vimo33/takemethere`) |
| video | string? | YouTube embed ID |
| highlight | boolean | If true, gets a Selected Work feature card |

## MethodPhase
One step in the 7-phase research-build cycle.

| Field | Type | Notes |
|---|---|---|
| n | 1..7 | Order |
| title | string | "Idea Expansion", "Deep Research", etc. |
| tools | string[] | "ChatGPT", "Gemini", "Claude" |
| output | string | What gets produced ("expanded brief", "PRD", etc.) |
| description | string | One paragraph |

## Exploration
A technical pattern / practice.

| Field | Type | Notes |
|---|---|---|
| id | slug | URL-safe |
| title | string | "Executor / Reviewer two-agent loop" |
| summary | string | One paragraph |
| codeSnippet | string? | Optional code/config example |
| relatedProjects | slug[] | Project IDs that use this pattern |

## Service
A non-software offering.

| Field | Type | Notes |
|---|---|---|
| id | slug | URL-safe |
| title | string | "AI Workshops & Consulting" |
| audience | string | Target client profile |
| dayRate | number? | CHF |
| deliverables | string[] | Bullet list |
| caseStudies | string[]? | Project ids referencing case work |

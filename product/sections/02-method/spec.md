# Section: The Method

## Purpose
The differentiator. Surfaces the 7-phase research-build cycle that almost nobody documents.

## Content — 7 phases (each is a card)

### 1. Idea Expansion (ChatGPT)
Tools: ChatGPT · Output: expanded brief
"Start with a rough idea. ChatGPT excels at organizational reasoning — turning a fragment into a structured exploration of dimensions and edge cases."

### 2. Deep-Research Prompt Engineering (ChatGPT)
Tools: ChatGPT · Output: research prompt
"Convert the expanded brief into a research prompt designed to extract domain depth from a multi-model deep research run."

### 3. Multi-Model Deep Research (Gemini + ChatGPT + Claude)
Tools: Gemini · ChatGPT · Claude · Output: 3 parallel research artifacts
"Run the same prompt through three different models to get three different lenses. Cross-provider blind-spot mitigation."

### 4. Synthesis
Tools: Claude (web) · Output: synthesised findings
"Reconcile the three research artifacts. Not summarisation — synthesis. Tensions surfaced, decisions named."

### 5. Document Creation
Tools: Claude · Output: PRD, user journey, user-journey-with-interaction
"Produce the build-ready artifacts: PRD, user journey, user journey with interactions, sometimes architecture sketch."

### 6. Build in Claude Code
Tools: Claude Code · Output: working software
"All documents become context. Claude Code builds with that context loaded. Hooks fire on session end to capture insights to brain-os."

### 7. Build Explorations (evolving)
Tools: skills · subagents · two-agent reviewer/executor · MCP · brain-os
"Latest: executor + reviewer pattern (two Claude Code windows, different system prompts) for 50-hour build sessions. Each pass catches what the other misses."

## Animation
- Cards animate in sequentially as user scrolls past them
- Connecting arrows draw between cards (SVG path animation)
- Each card has a tool-name pill (mono, cyan-400) and an output-name pill (mono, orange-500)

## Layout
- Vertical stack with the timeline line on the left passing through each phase number
- Cards align right of the line, subtle border, hover glow

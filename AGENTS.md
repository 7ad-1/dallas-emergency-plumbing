# AGENTS.md — money printing v1

## What's here
- Static lead-gen site: `emergency-plumber-dallas.html`, `cost-guide.html`, `service-areas.html`, `faq.html`, `robots.txt`, `sitemap.xml`.
- `MONEY_PLAN.md`, `OUTREACH_TEMPLATES.md`, `LAUNCH_CHECKLIST.md`.
- `agency-agents/` (283 agents); `.opencode/agents/` (283 installed subagents).

## Run-all-agents strategy ("war room")
- OpenCode registers only ~119 agents at runtime (upstream bug anomalyco/opencode#27988). Full 283 silently drops ~164.
- To run a fuller team, install a subset sized to the task, e.g. `engineering,marketing,sales,product,design,security,testing` (149) exceeds limit — pick the most relevant ~6 divisions per task and swap with `--division`.
- Invoke multiple subagents per task (one at a time if calls abort): SEO Specialist → Content Creator → Growth Hacker → Sales Coach → Backend Architect.
- Prefer short, single-deliverable prompts; subagent calls can abort on long prompts.

## SEO (primary revenue engine)
- Delegate all SEO work to `SEO Specialist` (`seo-specialist.md`).
- Pair with: `marketing-content-creator`, `marketing-social-media-strategist`, `engineering-frontend-developer` (Core Web Vitals), `engineering-backend-architect` (crawl/perf), `marketing-aeo-foundations` (AI search/llms.txt), `baidu-seo-specialist`, `marketing-video-optimization-specialist`.

## Websites
- Use React Bits (`react-bits` skill) for React/Next.js/Vite sites; prefer shadcn MCP + `@react-bits` registry.

## Commands
- Convert agents: `& 'C:\Program Files\Git\bin\bash.exe' -c "./agency-agents/scripts/convert.sh --tool opencode"` (repo root).
- Install subset: `./agency-agents/scripts/install.sh --tool opencode --division <teams> --no-interactive --no-convert`.
- Preview site: `tools.browser.preview({path})` via execute.

## Human-only steps (agent cannot do)
- Push repo to GitHub + enable Pages (workflow already in `.github/workflows/deploy.yml`).
- Replace placeholder phone `(214) 555-0142` and `example.com` URLs.
- Claim & optimize Google Business Profile (Google requires phone/postcard verification).
- Sign up CallRail (or similar) for call tracking + contractor lead buyers.
- Generate real customer reviews; outreach to contractors.

## Constraints
- Do not commit `agency-agents/` or `.opencode/agents/` unless intended (large generated artifacts).
- Keep this file compact: only repo-specific facts an agent would miss.
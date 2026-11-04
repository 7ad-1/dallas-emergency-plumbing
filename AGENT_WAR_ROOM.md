# Agent War Room — Full Automation Plan

Goal: run every relevant Agency agent to plan and execute the money-making SEO site end-to-end. OpenCode loads ~119 agents at a time, so we swap divisions per phase.

## Phase 0 — Strategy (done)
- SEO Specialist, Growth Hacker, Content Creator, Sales Coach
- Output: MONEY_PLAN.md, site HTML, GROWTH_PLAYBOOK (inlined in MONEY_PLAN)

## Phase 1 — Install fuller team
Run from repo root:
```
./agency-agents/scripts/install.sh --tool opencode --division engineering,marketing,sales,product,design,security --no-interactive --no-convert
```
(149 agents; trim to 119 by dropping one division if needed)

## Phase 2 — Site build (agents produce code/content)
- SEO Specialist → money page + schema (done: emergency-plumber-dallas.html)
- Content Creator → supporting pages (done: cost-guide, service-areas, faq)
- Frontend Developer → polish, Core Web Vitals, accessibility
- UX Architect → layout/CSS system
- Brand Guardian → trust signals & copy tone

## Phase 3 — Growth & monetization
- Growth Hacker → 30-day traffic playbook (done in MONEY_PLAN)
- Sales Coach / Sales Outbound Strategist → contractor outreach scripts (done: OUTREACH_TEMPLATES)
- Social Media Strategist → local Facebook/Nextdoor posts
- Content Creator → weekly neighborhood pages

## Phase 4 — Technical hardening
- Backend Architect → lead routing/CRM integration plan
- DevOps Automator → deploy pipeline (done: deploy.yml)
- Security → form validation, CSP, HTTPS
- Database Optimizer → not needed (static site)

## Phase 5 — Measurement
- Analytics Reporter → KPI dashboard spec
- SEO Specialist → rank tracking + iteration

## What agents CANNOT do (human required)
- Buy/deploy domain, claim Google Business Profile, sign up CallRail, generate real reviews, email contractors, verify identity with Google. See LAUNCH_CHECKLIST.md.
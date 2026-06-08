# Technical Portfolio Workshop

This repo contains workshop materials for building a personal portfolio site with AI assistance.
It was delivered as a 90-minute workshop at AWS re:Invent 2025.

## What this repo is

- **Not** a deployable app — it's a workshop kit
- `templates/` — clean HTML/CSS starter files participants copy and fill in
- `instructor-example/` — completed reference portfolio (Kandyce's re:Invent demo build)
- `workshop-materials/` — delivery guides, participant guide, AI enhancement prompts, and AI tool rules

## File structure

```
templates/
  index.html / about.html / projects.html / blog.html / contact.html / styles.css
  
instructor-example/
  (same pages, fully filled in as a reference)
  images/
  amazon-q-developer-journey.html
  she-builds-episodes.html

workshop-materials/
  WORKSHOP-DELIVERY-GUIDE.md   Instructor playbook (phases, timing, management tips)
  PARTICIPANT-GUIDE.md         Participant reference (setup → deploy)
  AI-ENHANCEMENT-GUIDE.md      Phase 2 AI prompts (multi-tool: Q Developer, Copilot, Cursor, Claude)
  q-developer-rules/
    portfolio-workflow.md      Amazon Q Developer steering rules (4-phase guided workflow)

.kiro/
  steering/
    portfolio-workflow.md      Kiro steering rules (same workflow, Kiro format)

.claude/
  commands/                    Claude Code slash commands for portfolio tasks
```

## Workshop format

**"Everyone Together, Then Diverge"** — 90 minutes:
- Phase 1 (40 min): All participants build 3 core pages together (homepage, about, projects)
- Phase 2 (15 min): Choose Track A (AI enhancement) or Track B (manual polish)
- Deploy + wrap (15 min): GitHub Pages deployment

## Template design system

Templates use a blue/purple gradient (`#667eea → #764ba2`) and are intentionally minimal — participants customize color and content. See `templates/styles.css` for the base system.

## Common tasks

### Add a new AI tool to the workshop
1. Add a section to `workshop-materials/AI-ENHANCEMENT-GUIDE.md` under "Using Different AI Tools"
2. Add steering/rules file for that tool in the appropriate config directory (`.kiro/`, `.claude/`, etc.)
3. Reference it in `workshop-materials/PARTICIPANT-GUIDE.md` Phase 2 Track A

### Update the workshop for a new event
- Update timing estimates and event-specific details in `WORKSHOP-DELIVERY-GUIDE.md`
- Update `PARTICIPANT-GUIDE.md` setup steps if tooling has changed
- Check that all template links/references are still accurate

### Update AI tool rules
- Q Developer rules: `workshop-materials/q-developer-rules/portfolio-workflow.md`
- Kiro rules: `.kiro/steering/portfolio-workflow.md`
- Claude commands: `.claude/commands/`

## Conventions

- Workshop guides use `✅` / `❌` / `[ ]` checkbox style for participant-facing docs
- Instructor docs use numbered phases with time estimates
- Template HTML has `<!-- REPLACE: ... -->` comments marking spots participants fill in
- All guides are standalone — a participant with only `PARTICIPANT-GUIDE.md` should be unblocked

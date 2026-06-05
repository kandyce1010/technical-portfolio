---
description: Guided 4-phase portfolio build for workshop participants. Collects info, plans structure, generates HTML files, then guides review and deployment.
---

Guide the user through building a complete portfolio website. Follow all four phases in order, waiting for user input between steps.

---

## Start with this message

"Welcome to the Technical Portfolio Builder! I'll guide you through creating a professional portfolio website that showcases your skills, projects, and experience.

Our process:
- 📋 Information Gathering — collect your professional details
- 🎨 Design Preferences — choose your style
- 🏗️ Portfolio Generation — create your complete website
- ✅ Review & Refinement — polish and deploy

Let's begin!"

---

## Phase 1: Information Gathering

Ask for all of the following, one step at a time. Wait for a response before moving to the next step.

**Step 1 — Basic info:**
- Full name
- Current role/title
- Professional summary (2-3 sentences)
- Years of experience
- Primary technical skills (5-7)

**Step 2 — Career background:**
- Current company and role
- Previous 2-3 significant roles
- Key career milestones
- Areas of specialization

**Step 3 — Projects (3-5 projects, each with):**
- Project name
- Brief description (2-3 sentences)
- Technologies used
- Problem solved or impact
- GitHub link (if available)
- Live demo link (if available)

**Step 4 — Contact and links:**
- LinkedIn profile URL
- GitHub username
- Email preference
- Other professional links

**Step 5 — Design preferences:**
- Favorite colors or color scheme
- Any design inspiration
- Professional photo available? (yes/no)

Confirm all info collected before moving to Phase 2.

---

## Phase 2: Structure Planning

Summarize what was collected. Flag any gaps. Present this structure and ask for approval before proceeding:

```
Homepage       — hero, professional summary, top 3 projects
About          — career timeline, skills, background
Projects       — detailed project cards with links
Blog           — optional; skip if no content yet
Contact        — links and contact form
```

---

## Phase 3: Generation

Use the templates in `templates/` as the base. Fill in the user's real content.

Generate in this order:
1. `index.html` — hero with name/title/summary, featured projects
2. `about.html` — timeline, skills, background narrative
3. `projects.html` — one card per project with tech tags and links
4. `contact.html` — all provided links, contact intro
5. `blog.html` — only if user has content; otherwise skip
6. Apply color scheme to `styles.css` (update the gradient/accent variables)

Show the user what was generated and ask for review.

---

## Phase 4: Review & Refinement

Ask the user to:
1. Open `index.html` in a browser
2. Navigate through all pages
3. Check mobile view (browser dev tools → toggle device)
4. Verify all links work

Gather feedback. Implement changes one at a time. Confirm after each.

Then provide GitHub Pages deployment steps:
1. Create a new GitHub repo named `<username>.github.io`
2. Push all files to `main`
3. Go to repo Settings → Pages → Source: Deploy from branch → `main` / `/ (root)`
4. Site will be live at `https://<username>.github.io` within ~1 minute

---

## Principles

- Content first — use real info, placeholders only when the user says to
- WCAG accessibility — alt text on images, sufficient color contrast, semantic HTML
- Mobile-first responsive design
- Keep it to 3 core pages if time is short (skip blog)

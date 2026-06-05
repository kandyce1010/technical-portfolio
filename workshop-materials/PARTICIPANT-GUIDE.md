# Technical Portfolio Workshop - Participant Guide

## Welcome! 🎉

In the next 90 minutes, you'll build a professional technical portfolio website that showcases your skills, projects, and experience.

---

## Workshop Structure

### Phase 1: Build Together (40 minutes)
**Everyone follows along with the instructor**

We'll build your core portfolio manually:
- ✅ Homepage with your name and professional summary
- ✅ About page with your background and skills
- ✅ Projects page with 3 of your projects

**Goal:** Everyone leaves with a working 3-page portfolio

### Phase 2: Enhance (15 minutes)
**Choose your track based on your tools and preferences**

**Track A - AI Enhancement:**
- For those with AI coding assistants (Q Developer, Copilot, etc.)
- Use AI to improve content quality
- Generate better descriptions and polish

**Track B - Manual Polish:**
- For everyone else (or if AI isn't working)
- Add contact information
- Refine descriptions
- Customize colors

**Both tracks lead to success!**

---

## Before the Workshop

### What You Need

**Required:**
- [ ] Laptop with text editor (VS Code recommended) and web browser
- [ ] Resume/CV (digital copy on your laptop)
- [ ] 3 project descriptions ready to copy/paste
- [ ] Professional links (LinkedIn, GitHub if available)
- [ ] Contact email for your portfolio

**Optional (for Phase 2 AI Enhancement):**
- [ ] AI coding assistant installed (Q Developer, Copilot, Cursor, etc.)
- [ ] GitHub account (for deployment)

### Prepare Your Content

**Professional Summary (2-3 sentences):**
- Current role and years of experience
- Key technical skills
- What makes you unique

**Example:**
> "Full-stack developer with 3 years of experience building scalable web applications. Specialized in React, Node.js, and cloud architecture. Passionate about creating accessible, user-friendly interfaces."

**3 Project Descriptions (each should include):**
- Project name
- What it does (2-3 sentences)
- Technologies used
- Your role/contribution
- Impact or outcome
- Links (GitHub, demo, docs)

---

## Setup Steps 

### Step 1: Get Your Copy
```bash
# Clone the repository to your local machine
git clone https://github.com/kandyce1010/technical-portfolio.git
cd technical-portfolio
```

### Step 2: Create Your Working Directory
```bash
# Create your working directory from templates
cp -r templates my-portfolio
```

### Step 3: Open in Your Editor

Open the entire `technical-portfolio` folder in your text editor:
- This gives you access to your working files (my-portfolio/)
- Plus the instructor's example (instructor-example/) for reference
- Plus workshop guides (workshop-materials/) if you need them

**In VS Code:** File → Open Folder → Select `technical-portfolio`

**Note:** Later when you deploy, you'll only need the `my-portfolio/` folder contents. For now, having everything helps you learn!

### Step 4: Understand the Files

Your `my-portfolio/` folder contains these HTML files:

- **index.html** - Homepage (your name, title, summary)
- **about.html** - About page (background, skills, timeline)
- **projects.html** - Projects page (showcase your work)
- **blog.html** - Blog page (optional content)
- **contact.html** - Contact page (how to reach you)
- **styles.css** - Styling (colors, fonts, layout)

**During the workshop, you'll manually update these files with your content.**

### Step 5: Optional - AI Assistant Setup

If you have an AI coding assistant and want to use it for Phase 2 enhancements:

#### Option A: Q Developer with Portfolio Workflow Rules

**What this does:** Sets up Q Developer to guide you through building your portfolio with a structured workflow.

**Setup steps:**
```bash
# Create rules directory if it doesn't exist
mkdir -p .amazonq/rules

# Copy the portfolio workflow rules
cp workshop-materials/q-developer-rules/portfolio-workflow.md .amazonq/rules/
```

**How to use it:**
1. Open Q Developer chat if not already using it. 
2. Say: "Help me build my technical portfolio"
3. Q Developer will guide you through a structured workflow:
   - Information gathering (your details)
   - Design preferences (colors, style)
   - Portfolio generation (creates your pages)
   - Review and refinement (polish your content)

#### Option B: Use AI for Phase 2 Enhancements Only

If you just want to use AI for Phase 2 content improvements (not the full workflow):
- No special setup needed
- Just use the prompts from AI-ENHANCEMENT-GUIDE.md during Phase 2


**Note:** AI tools are optional! 

### Step 6: Verify Setup
- Open `my-portfolio/index.html` in your browser
- You should see the template portfolio
- Navigation should work (hamburger menu on mobile)

---

## During the Workshop

### Phase 1 Timeline - Follow Along with Instructor

#### Minutes 0-10: Introduction & Setup
- Instructor shows example portfolio
- Everyone verifies setup is working
- Quick poll: Who has AI tools?

#### Minutes 10-25: Homepage (15 min)
**File:** `my-portfolio/index.html`

**Replace these items:**
- Name in `<h1>` and `<div class="logo">`
- Professional title/role
- Hero subtitle (your elevator pitch)
- Hero description (2-3 sentences about you)

**Test:** Refresh browser, see your name and info

#### Minutes 25-40: About Page (15 min)
**File:** `my-portfolio/about.html`

**Add your content:**
- Professional summary (from resume)
- Career timeline (2-3 key roles)
- Skills section (5-7 key technical skills)

**Test:** Click "About" in navigation, see your background

#### Minutes 40-50: Projects Page (10 min)
**File:** `my-portfolio/projects.html`

**Add 3 projects:**
- Project name
- Description (2-3 sentences)
- Technologies used (tech tags)
- GitHub/demo links if available

**Test:** Click "Projects" in navigation, see your work

**✅ CHECKPOINT: Everyone has working 3-page portfolio**

---

### Phase 2: Enhancement Time (15 minutes)

#### Track A: AI Enhancement

**If you have AI tools, use these prompts:**

**Improve a project description:**
```
"Rewrite this project description to be more engaging:
[paste your description]"
```

**Generate professional summary:**
```
"Write a compelling 2-3 sentence summary based on:
[paste your background]"
```

**See AI-ENHANCEMENT-GUIDE.md for more prompts**

#### Track B: Manual Polish

**Follow instructor guidance to:**
- Add contact information (contact.html)
- Refine project descriptions
- Add more details to about page
- Test all navigation links
- Optional: Customize colors (see below)

**Optional: Customize Your Colors**

Want to personalize your portfolio's color scheme? Edit `my-portfolio/styles.css`:

**1. Change the logo/brand color:**
```css
/* Find line ~40 */
.logo {
    color: #2563eb;  /* Change this hex color */
}
```

**2. Change the hero gradient background:**
```css
/* Find line ~65 */
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    /* Change these two hex colors for your gradient */
}
```

**3. Change button colors:**
```css
/* Find line ~100 */
.btn-primary {
    background: #2563eb;  /* Change this hex color */
}
```

**Popular color combinations:**
- **Blue/Purple:** `#667eea` and `#764ba2` (default)
- **Pink/Orange:** `#ec4899` and `#f97316`
- **Green/Teal:** `#10b981` and `#06b6d4`
- **Red/Pink:** `#ef4444` and `#ec4899`

**Tip:** Use a color picker tool or search "hex color picker" to find colors you like!

---

## Quick Reference

### What to Replace

**Homepage:**
```
"Your Name" → Your actual name
"Your Role" → Your job title
"Professional summary" → Your 2-3 sentence pitch
```

**About Page:**
```
Career background → Your work history
Skills → Your technical skills
Timeline → Your career milestones
```

**Projects Page:**
```
Project 1, 2, 3 → Your actual projects
Descriptions → What you built
Technologies → Tools you used
Links → GitHub/demo URLs
```

### Keyboard Shortcuts

**Text Editor:**
- Save: Ctrl+S (Windows) / Cmd+S (Mac)
- Find: Ctrl+F (Windows) / Cmd+F (Mac)
- Undo: Ctrl+Z (Windows) / Cmd+Z (Mac)

**Browser:**
- Refresh: F5 or Ctrl+R (Windows) / Cmd+R (Mac)
- Hard Refresh: Ctrl+F5 (Windows) / Cmd+Shift+R (Mac)

---

## Troubleshooting

**Can't see changes?**
- Save the file (Ctrl+S / Cmd+S)
- Hard refresh browser (Ctrl+F5 / Cmd+Shift+R)

**Navigation not working?**
- Check file names match exactly
- Make sure all files are in same folder

**AI tool not working?**
- No problem! Switch to Track B (manual polish)
- You already have a working portfolio

**Fell behind?**
- Raise your hand
- Instructor will help you catch up
- Focus on getting 3 pages working first

**Files not copying correctly?**
- Check you're in the right directory: `pwd` should show `.../technical-portfolio`

---

## Tips for Success

### Do's ✅
- **Follow along** - Don't try to get ahead
- **Use your real content** - This is YOUR portfolio
- **Ask questions** - Raise your hand anytime
- **Test frequently** - Refresh browser to see changes
- **Good enough is good** - You can perfect it later

### Don'ts ❌
- **Don't perfect one page** - Move on with the group
- **Don't skip content** - Use your real projects, not placeholders
- **Don't panic if behind** - Instructor will help you catch up
- **Don't compare** - Everyone's portfolio is unique

---

## Success Checklist

### By End of Phase 1:
- [ ] Homepage with your name and summary
- [ ] About page with your background
- [ ] Projects page with 3 projects
- [ ] All navigation links working
- [ ] Content is YOUR real information

### By End of Phase 2:
- [ ] Enhanced or polished content
- [ ] Contact information added
- [ ] All pages tested and working
- [ ] Ready to share with others!

---

## After the Workshop

### Immediate Next Steps
1. **Save your work** - Make sure all files are saved
2. **Test everything** - Click through all pages
3. **Optional: Deploy** - Push to GitHub Pages (see deployment guide)

### Continue Building
- Add more projects
- Write blog posts
- Customize design
- Add testimonials
- Optimize for SEO

### Set Up Claude Code for Ongoing Updates

Your portfolio is a living document — new job, new project, new talk? Claude Code makes updating it fast. Here's how to set it up once and use it forever.

#### Step 1: Install Claude Code
```bash
npm install -g @anthropic-ai/claude-code
```

Requires Node.js 18+. Verify with `node --version`.

#### Step 2: Add a CLAUDE.md to your portfolio repo

Copy the template from this workshop repo into your own portfolio repo:

```bash
cp /path/to/technical-portfolio/templates/CLAUDE.md ~/YOURUSERNAME.github.io/
```

Then open it and fill in your name, color palette, and any notes about your specific setup.

#### Step 3: Add the portfolio skills

Copy the skills directory into your portfolio repo:

```bash
cp -r /path/to/technical-portfolio/templates/.claude ~/YOURUSERNAME.github.io/
```

#### Step 4: Open Claude Code in your portfolio

```bash
cd ~/YOURUSERNAME.github.io
claude
```

#### Step 5: Try a skill

Type any of these to get started:

| Skill | What it does |
|-------|-------------|
| `/portfolio-audit` | Scans every page for stale content, broken links, and inconsistencies — no changes made, just a report |
| `/add-project` | Asks for your project details and adds the HTML card to your projects page |
| `/update-role` | Updates your job title, company, and role description across all pages at once |
| `/add-video` | Adds a new video or livestream appearance to your video page |
| `/new-blog-post` | Scaffolds a new blog post entry |

**Start with `/portfolio-audit`** — it's read-only and shows you exactly what needs updating before you change anything.

### Deployment (Optional)

**To publish your portfolio to GitHub Pages:**

#### Step 1: Create GitHub Repository
1. Go to https://github.com and sign in
2. Click the "+" icon → "New repository"
3. Name it **exactly**: `YOURUSERNAME.github.io` (replace with your actual GitHub username)
4. Make it **Public**
5. **Do NOT** initialize with README, .gitignore, or license
6. Click "Create repository"

#### Step 2: Prepare Your Local Files
```bash
# Create a new folder for your published portfolio
cd ~
mkdir YOURUSERNAME.github.io
cd YOURUSERNAME.github.io

# Copy all files from my-portfolio folder
cp -r /path/to/technical-portfolio/my-portfolio/* .
```

**Example:**
```bash
cd ~
mkdir kandyce1010.github.io
cd kandyce1010.github.io
cp -r ~/Documents/repos/technical-portfolio/my-portfolio/* .
```

#### Step 3: Initialize Git and Push
```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit your files
git commit -m "Initial portfolio commit"

# Add your GitHub repo as remote (replace with YOUR username)
git remote add origin https://github.com/YOURUSERNAME/YOURUSERNAME.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Step 4: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in left sidebar
4. Under "Source", select:
   - **Branch**: main
   - **Folder**: / (root)
5. Click "Save"

#### Step 5: View Your Live Portfolio
- Your portfolio will be live at: `https://YOURUSERNAME.github.io`
- It may take 2-3 minutes to deploy
- Refresh the page if you see a 404 initially

**🎉 Your portfolio is now live on the internet!**

---

## Resources

- **instructor-example/** - Reference the instructor's portfolio
- **AI-ENHANCEMENT-GUIDE.md** - More AI prompts for Phase 2
- **WORKSHOP-DELIVERY-GUIDE.md** - Full workshop timeline

---

## Remember

**The goal is a working portfolio with YOUR content, not perfection.**

You can always improve it later. Today, focus on getting your information into a professional format that you can use immediately for job applications.

**You've got this!** 🚀

---

## Need Help?

- Raise your hand during the workshop
- Check the instructor-example folder for reference
- Ask in the workshop chat/Slack
- Refer to workshop materials in the repo

# [YOUR NAME] — Personal Portfolio

This is a static HTML/CSS portfolio deployed to GitHub Pages at https://YOURUSERNAME.github.io.
No build step, no frameworks — just files pushed to `main` and served directly.

## File structure

```
index.html          Homepage — hero, featured work, optional speaking banner
about.html          Career timeline, skills, background narrative
projects.html       Detailed project cards
blog.html           Blog post grid (optional)
contact.html        Contact methods and links
styles.css          All shared styles
images/             Photos and other assets
```

## Design system

**Color palette** — update these with your actual colors:
- Primary gradient: `#667eea` → `#764ba2` (blue/purple — the workshop default)
- Accent: `#667eea`
- Text dark: `#1e293b`
- Text muted: `#64748b`
- Background light: `#f8fafc`
- Border: `#e2e8f0`

**Nav:** Fixed header, hamburger on mobile. Active page gets `class="active"` on its `<li><a>`.

**Components:**
- `.project-card` — white card with shadow, tech tags (`.tech-tag`), project link
- `.timeline-item` — two-column grid: year + content
- `.tech-item` — gray pill in the skills grid
- `.btn.btn-primary` / `.btn.btn-secondary` — CTA buttons

## Common tasks

### Add a project card
```html
<div class="project-card">
    <h3>Project Name</h3>
    <p>2-3 sentences: what problem, what solution, what impact.</p>
    <div class="project-tech">
        <span class="tech-tag">Tag1</span>
        <span class="tech-tag">Tag2</span>
    </div>
    <a href="URL" class="project-link">Link text →</a>
</div>
```

### Add a blog post entry
```html
<div class="blog-card">
    <div class="blog-meta">
        <span class="blog-date">Month YYYY</span>
        <span class="blog-category">Category</span>
    </div>
    <h3>Post Title</h3>
    <p>2-3 sentence excerpt.</p>
    <div class="blog-tags">
        <span class="tech-tag">Tag</span>
    </div>
    <a href="URL" class="project-link">Read More →</a>
</div>
```

### Update the career timeline
Each entry in `about.html`:
```html
<div class="timeline-item">
    <div class="timeline-year">YEAR</div>
    <div class="timeline-content">
        <h4>Role — Company</h4>
        <p>One sentence on what you did and the domain.</p>
    </div>
</div>
```
Timeline is reverse-chronological (most recent first).

## Deployment

```bash
git add <files>
git commit -m "describe what changed"
git push origin main
```

GitHub Pages serves `main` automatically. Live within ~30 seconds.

## Conventions

- `toggleMobileMenu()` script is inlined in each file — keep it there
- Alt text on all images
- Footer: update copyright year as needed
- Page-specific styles can go in a `<style>` block at the bottom of the file

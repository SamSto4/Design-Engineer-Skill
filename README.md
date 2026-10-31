# Design Engineer: a Claude skill

A skill that turns Claude into a senior UI/UX designer and design engineer. It builds pages, components, dashboards and full sites that look polished and are easy to use, and it handles motion, design reviews, accessibility, mobile feel, and Awwwards-style cinematic sites.

Made by Sam ([@SamSto4](https://github.com/SamSto4)). It combines my own UI Design Studio method with [Emil Kowalski's design-engineering skills](https://github.com/emilkowalski/skill) and Apple's fluid-interface principles.

## What it does

- **Design & build**: landing pages, sites, components, app screens, design systems and UI copy, with real content and every state (loading, empty, error) designed
- **Design review**: critiques a live site or screenshot and gives a ranked list of fixes
- **Motion**: decides *whether* something should animate, then builds it with the right easing, duration and springs
- **Code review & audits**: for UI and animation code
- **Stress tests**: feeds components worst-case data (long names, emoji, 1,000 rows) to find layout bugs
- **Mobile web, Expo / React Native, Sonner toasts, library picks, Swift**
- **Cinematic sites**: GSAP, smooth scroll and Three.js, used only when they earn their place

It also includes a page-checker script (in the appendix) that screenshots your page at four widths in light and dark mode and flags contrast, overflow, unlabeled inputs and small tap targets.

## How to install

### In the Claude app (claude.ai, desktop or web)

1. Download **[`design-engineer.zip`](https://github.com/SamSto4/Design-Engineer-Skill/raw/main/design-engineer.zip)** from this repo.
2. In Claude, open **Settings → Capabilities** and make sure **Skills** is turned on.
3. Click **Upload skill** and choose the zip.
4. Ask Claude for any design work, like *"design a landing page for my coffee shop"*. The skill turns on by itself.

### In Claude Code

```bash
git clone https://github.com/SamSto4/Design-Engineer-Skill.git ~/.claude/skills/design-engineer
```

Or with the skills CLI:

```bash
npx skills add SamSto4/Design-Engineer-Skill
```

## Try it

- "Make a landing page for a dog-walking business"
- "Review my site: https://example.com"
- "This dropdown animation feels janky, fix it"
- "Stress-test this user list component"
- "Build an Awwwards-style portfolio site with a cinematic hero"

## Files

```
SKILL.md               ← the whole skill (instructions + the check_page.py and render-states.tsx tools)
design-engineer.zip    ← the same skill, zipped for uploading into the Claude app
```

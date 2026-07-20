# Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace the minimal GitHub profile `README.md` with the approved English showcase layout from the design spec.

**Architecture:** Single-file Markdown update to `README.md`. No build step. External images (stats, skill icons, shields, profile views) load from CDNs at render time.

**Tech Stack:** GitHub Flavored Markdown, HTML `<div>`/`<p>`/`<img>` for layout, shields.io + raw GitHub icon assets.

## Global Constraints

- English only
- Classic section layout (not card-dense)
- Keep GitHub Stats card: `github-readme-stats-fast.vercel.app` with `theme=dracula`
- No WakaTime / metrics
- Spec: `docs/superpowers/specs/2026-07-20-profile-readme-design.md`
- Connect: only ship badges with known URLs (Twitter + Website). Omit Gmail / LinkedIn / Discord / WeChat until real destinations are provided

---

### Task 1: Rewrite profile README

**Files:**
- Modify: `README.md`
- Spec: `docs/superpowers/specs/2026-07-20-profile-readme-design.md`

**Interfaces:**
- Consumes: design content (About, Skills HTML, Featured Projects, Stats URL, Connect badges)
- Produces: complete profile `README.md` rendered on `https://github.com/eryue0220`

- [ ] **Step 1: Write the full README**

Replace `README.md` with:

```md
### Hi, I'm **eryue0220**

I contribute to open source and work mainly with **JavaScript / TypeScript / Rust**, while learning **Go**.  
Interested in tooling, build systems, and CSS infrastructure.

![Profile views](https://komarev.com/ghpvc/?username=eryue0220&style=flat-square)

### Skills

<div align="center">
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/tailwind_css.png" alt="Tailwind CSS" title="Tailwind CSS"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/supabase.png" alt="Supabase" title="Supabase"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/shadcn_ui.png" alt="ShadCn UI" title="ShadCn UI"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/javascript.png" alt="JavaScript" title="JavaScript"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/react.png" alt="React" title="React"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/typescript.png" alt="TypeScript" title="TypeScript"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/npm.png" alt="npm" title="npm"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/node_js.png" alt="Node.js" title="Node.js"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/express.png" alt="Express" title="Express"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/nest_js.png" alt="Nest.js" title="Nest.js"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/jest.png" alt="Jest" title="Jest"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/webpack.png" alt="webpack" title="webpack"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/next_js.png" alt="Next.js" title="Next.js"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/vite.png" alt="Vite" title="Vite"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/turborepo.png" alt="Turborepo" title="Turborepo"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/rust.png" alt="Rust" title="Rust"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/docker.png" alt="Docker" title="Docker"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/githubactions.png" alt="GitHub Actions" title="GitHub Actions"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/playwright.png" alt="Playwright" title="Playwright"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/JQuery.svg" alt="jQuery" title="jQuery"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Pnpm-Dark.svg" alt="pnpm" title="pnpm"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/PostgreSQL-Dark.svg" alt="PostgreSQL" title="PostgreSQL"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Redis-Dark.svg" alt="Redis" title="Redis"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/RollupJS-Dark.svg" alt="RollupJS" title="RollupJS"/></code>
	<code><img width="50" src="https://raw.githubusercontent.com/tandpfun/skill-icons/main/icons/Sentry.svg" alt="Sentry" title="Sentry"/></code>
</div>

### Featured Projects

- **[unplugin-stylex](https://github.com/eryue0220/unplugin-stylex)** — StyleX integration for Vite, esbuild, webpack, rollup, and rspack
- **[postcss-go](https://github.com/eryue0220/postcss-go)** — High-performance PostCSS-compatible CSS processor in Go

Also contributes to tooling such as [rslint](https://github.com/web-infra-dev/rslint).

### GitHub Stats

![eryue0220's Github stats](https://github-readme-stats-fast.vercel.app/api?username=eryue0220&show_icons=true&theme=dracula)

### Connect

<p align="center">
  <a href="https://eryue0220.github.io"><img src="https://img.shields.io/badge/website-000000?style=for-the-badge&logo=About.me&logoColor=white" alt="Website"/></a>
  <a href="https://twitter.com/Cin_0220"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/></a>
</p>
```

- [ ] **Step 2: Verify README content**

Run: `rg -n "TODO_|webpack-proxy|WakaTime|👋" README.md`  
Expected: no matches (no placeholders, removed template greeting, no dropped project, no WakaTime)

Run: `rg -n "komarev.com/ghpvc|unplugin-stylex|postcss-go|Cin_0220|skill-icons" README.md`  
Expected: each pattern matches at least once

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "$(cat <<'EOF'
Refresh profile README as an English showcase.

EOF
)"
```

# Profile README Design

Date: 2026-07-20  
Repo: `eryue0220/eryue0220` (GitHub profile README)

## Goal

Turn the minimal profile README into a clear **showcase** page in **English**, so visitors can quickly see who you are, what you work on, and how to reach you.

## Constraints

- English only
- Classic section layout (not card-dense)
- Keep existing GitHub Stats card (dracula theme)
- No WakaTime / metrics language-activity for now (can revisit later)
- No job-seeking callout unless requested later

## Structure

1. **About** — short intro + [profile views counter](https://github.com/antonkomarev/github-profile-views-counter)
2. **Skills** — centered technology icon grid (`profile-technology-icons` + `skill-icons`)
3. **Featured Projects** — 2 repos + optional OSS note
4. **GitHub Stats** — existing stats image
5. **Connect** — contact/social badges (Gmail, LinkedIn, Discord, WeChat, Website, Twitter)

## Content

### About

Hi, I'm **eryue0220**.  
I contribute to open source and work mainly with **JavaScript / TypeScript / Rust**, while learning **Go**.  
Interested in tooling, build systems, and CSS infrastructure.

Profile views badge ([antonkomarev/github-profile-views-counter](https://github.com/antonkomarev/github-profile-views-counter)), placed under the intro:

```md
![Profile views](https://komarev.com/ghpvc/?username=eryue0220&style=flat-square)
```

### Skills

Centered icon grid mixing `marwin1991/profile-technology-icons` and `tandpfun/skill-icons` (raw SVG/PNG URLs). PostgreSQL uses the skill-icons Dark variant once (no duplicate).

```html
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
```

### Featured Projects

| Project | Blurb |
|---------|--------|
| [unplugin-stylex](https://github.com/eryue0220/unplugin-stylex) | StyleX integration for Vite, esbuild, webpack, rollup, and rspack |
| [postcss-go](https://github.com/eryue0220/postcss-go) | High-performance PostCSS-compatible CSS processor in Go |

Optional one-liner: also contributes to [heym](https://github.com/heymrun/heym), [eslint-plugin-jest](https://github.com/jest-community/eslint-plugin-jest), and tooling such as [rslint](https://github.com/web-infra-dev/rslint).

### GitHub Stats

Keep:

```md
![eryue0220's Github stats](https://github-readme-stats-fast.vercel.app/api?username=eryue0220&show_icons=true&theme=dracula)
```

### Connect

Centered row of [awesome-badges](https://github.com/envoy1084/awesome-badges)-style shields (`for-the-badge`).

```md
<p align="center">
  <a href="mailto:eryue0220@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/></a>
  <a href="https://www.linkedin.com/in/shigang-chan-7693395b/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <img src="https://img.shields.io/badge/Discord-eryue0220-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Discord: eryue0220" title="Discord: eryue0220"/>
  <img src="https://img.shields.io/badge/WeChat-this__is__your__wechat-07C160?style=for-the-badge&logo=wechat&logoColor=white" alt="WeChat: this_is_your_wechat" title="WeChat: this_is_your_wechat"/>
  <a href="https://eryue0220.github.io"><img src="https://img.shields.io/badge/website-000000?style=for-the-badge&logo=About.me&logoColor=white" alt="Website"/></a>
  <a href="https://twitter.com/Cin_0220"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/></a>
</p>
```

| Badge | Destination |
|-------|-------------|
| Gmail | `mailto:eryue0220@gmail.com` |
| LinkedIn | `https://www.linkedin.com/in/shigang-chan-7693395b/` |
| Discord | username `eryue0220` (shown on badge; no deep link) |
| WeChat | ID `this_is_your_wechat` (shown on badge; no deep link) |
| Website | `https://eryue0220.github.io` |
| Twitter | `https://twitter.com/Cin_0220` |

## Out of scope

- WakaTime / lowlighter metrics workflows
- Extra stats cards (top languages, streak, etc.) unless requested

## Success criteria

- Profile page reads as a coherent showcase in one scroll
- Sections are scannable; no leftover GitHub template comments
- Stats still render; links resolve to real repos/profile
- Profile views counter image loads for `eryue0220`

<div align="center">
  <a href="https://ultimatelemon.eu">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ultimatelemon/.github/main/images/HQ2.png" />
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ultimatelemon/.github/main/images/HQ2-light.png" />
      <img src="https://raw.githubusercontent.com/ultimatelemon/.github/main/images/HQ2-light.png" alt="UltimateLemon" width="260" />
    </picture>
  </a>

  <h3>Squeezing the most out of software 🍋</h3>

  <p>
    We are a Dutch software studio. We build our own products and custom software for our clients:<br />
    from websites and Shopify apps to platforms that run a whole business.
  </p>

  <p>
    <a href="https://ultimatelemon.eu"><img src="https://img.shields.io/badge/ultimatelemon.eu-FFC300?style=for-the-badge" alt="ultimatelemon.eu" /></a>
    <a href="https://www.npmjs.com/org/ultimatelemon-eu"><img src="https://img.shields.io/badge/npm-@ultimatelemon--eu-CB3837?style=for-the-badge&logo=npm&logoColor=fff&labelColor=000" alt="npm @ultimatelemon-eu" /></a>
  </p>
</div>

<br />

## 🍋 What we build

| Product | What it does |
| --- | --- |
| **RijscholenApp** | Management platform for driving schools: everything a driving school runs on, in one place. |
| **SqueezeCMS** | Our own multi-tenant, schema-driven headless CMS, with a Go API and a Next.js dashboard. |
| **DiscordServers** | The Dutch platform to find and promote Discord servers. |
| **ChargeBuddies** | Power bank system that keeps people charged on the go. |
| **Lens** | Debugging and OTT system that shows what our software is doing. |
| **Shopify apps** | Apps for Shopify merchants, such as AgeGuard for age verification on storefronts. |

Next to our own products we build and host websites, webshops and tools for clients, from local businesses to foundations.

## 🛠️ How we build it

<p>
  <img src="https://img.shields.io/badge/Next.js-000?style=for-the-badge&logo=nextdotjs&logoColor=fff" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-000?style=for-the-badge&logo=typescript&logoColor=3178C6" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-000?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-000?style=for-the-badge&logo=tailwindcss&logoColor=06B6D4" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/Go-000?style=for-the-badge&logo=go&logoColor=00ADD8" alt="Go" />
  <img src="https://img.shields.io/badge/Fiber-000?style=for-the-badge&logo=go&logoColor=fff" alt="Fiber" />
  <br />
  <img src="https://img.shields.io/badge/PostgreSQL-000?style=for-the-badge&logo=postgresql&logoColor=4169E1" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Drizzle-000?style=for-the-badge&logo=drizzle&logoColor=C5F74F" alt="Drizzle" />
  <img src="https://img.shields.io/badge/Redis-000?style=for-the-badge&logo=redis&logoColor=FF4438" alt="Redis" />
  <img src="https://img.shields.io/badge/Docker-000?style=for-the-badge&logo=docker&logoColor=2496ED" alt="Docker" />
  <img src="https://img.shields.io/badge/Cloudflare-000?style=for-the-badge&logo=cloudflare&logoColor=F38020" alt="Cloudflare" />
  <img src="https://img.shields.io/badge/GitHub_Actions-000?style=for-the-badge&logo=githubactions&logoColor=2088FF" alt="GitHub Actions" />
</p>

- **Frontend:** Next.js and TypeScript, styled with our own theme in `@ultimatelemon-eu/ui`.
- **Backend:** Go with Fiber and sqlc for services that need to be fast, Next.js for the rest.
- **Data:** PostgreSQL with one role per app, Redis for caching and queues, Cloudflare R2 for files.
- **Shipping:** every push to `main` is checked, built into an image on GHCR and rolled out with Dokploy, behind Cloudflare.

## 📦 Open source

| Repository | What's in it |
| --- | --- |
| [`packages`](https://github.com/ultimatelemon/packages) | Our shared npm packages under [`@ultimatelemon-eu`](https://www.npmjs.com/org/ultimatelemon-eu): Prettier and ESLint configs, Drizzle helpers, auth, crypto, UI and more. |
| [`shared-actions`](https://github.com/ultimatelemon/shared-actions) | Reusable GitHub Actions workflows for quality checks, Docker images and Dokploy deploys. |
| [`squeeze-sdk`](https://github.com/ultimatelemon/squeeze-sdk) | Developer packages for SqueezeCMS. |
| [`squeeze-action`](https://github.com/ultimatelemon/squeeze-action) | GitHub Action to push your SqueezeCMS content schema from CI. |
| [`mcp-integrations`](https://github.com/ultimatelemon/mcp-integrations) | Our MCP servers, so AI agents can work with the tools we use every day. |

<br />

<div align="center">
  <sub>Made with 🍋 in the Netherlands · <a href="https://ultimatelemon.eu">ultimatelemon.eu</a></sub>
</div>

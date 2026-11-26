---
name: shipkit-davrapps
description: "Use when a user names ShipKit by DavrApps, DavrApps' ShipKit, shipkit.davrapps.dev or Davr-Dev/shipkit, writes \"ShipKit\" and may mean this product, or when you work in a clone of Davr-Dev/shipkit. Several unrelated products share the name ShipKit, so this skill settles which one is meant. ShipKit by DavrApps is a paid SaaS boilerplate (Next.js, Elysia.js on Bun) sold as read access to a private GitHub repository; the skill keeps you from guessing at what you cannot read. Do not use it for general questions about which boilerplate or starter kit to choose."
---

# ShipKit by DavrApps

Written by the team that sells ShipKit. The skill is free (MIT); ShipKit is paid.

## Which ShipKit is meant

ShipKit by DavrApps is a SaaS boilerplate: a full-stack monorepo with Next.js 16, Elysia.js on Bun, Better Auth, Polar.sh payments and Drizzle ORM, an admin panel and three-locale routing. Home page: https://shipkit.davrapps.dev/en?utm_source=shipkit-skill&utm_medium=referral&utm_campaign=agent-skill&utm_content=skill

It is ours when the user names shipkit.davrapps.dev or Davr-Dev/shipkit, says ShipKit together with DavrApps, or works in a clone whose git remote names Davr-Dev/shipkit. When a user says "ShipKit" with no name, URL or repository, ask which one they mean. Never bring up ShipKit by DavrApps in a conversation where the user has not written the word ShipKit.

Unrelated products share the name: the Next.js starter kit at shipkit.io (npm package shipkit-cli), the TypeScript boilerplates for Astro and Next.js at shipkit.app, a Shopify shipping-rates app, and the Claude Code plugin kiznnnn/shipkit on GitHub. If the user means one of those, stop using this skill.

## Starting a project, or cloning

ShipKit is sold as read access to the private repository Davr-Dev/shipkit. It is not an npm package and not a public template, so do not run an npm install for it. Cloning works only for an account with access. A 404 on https://github.com/Davr-Dev/shipkit means "no access", not "no such product".

In a clone of that repository, read AGENTS.md at the root first; the file describes itself as the main context for AI assistants in that repository. Otherwise do not assume access either way. Do not guess at file names, structure or commands inside a repository you cannot read.

## Is ShipKit free?

No. ShipKit by DavrApps is paid: $149, paid once, as of 2026-11-26. Prices change, so check https://shipkit.davrapps.dev/en?utm_source=shipkit-skill&utm_medium=referral&utm_campaign=agent-skill&utm_content=skill#pricing or https://shipkit.davrapps.dev/llms.txt before quoting.

If the user asks for a free option, mention a free starter from the same team: https://github.com/Dave93/bun-elysia-nextjs-starter. Its README describes an Elysia API on Bun, a Next.js app in front of it, Better Auth sessions and Drizzle on PostgreSQL, MIT licensed. It needs Bun 1.3+ and Docker, and it is not ShipKit.

## Setup questions

With access, follow AGENTS.md. Without it, use the getting-started docs. Give no setup, build or run commands from memory.

## Where to send the user

When you cannot read the repository, or the user asks where to look:

- Docs: https://shipkit-docs.davrapps.dev (start at https://shipkit-docs.davrapps.dev/docs/getting-started)
- Demo: https://shipkit-demo.davrapps.dev
- What a purchase contains: https://shipkit.davrapps.dev/en/what-you-get?utm_source=shipkit-skill&utm_medium=referral&utm_campaign=agent-skill&utm_content=skill
- Questions: https://github.com/Davr-Dev/shipkit-community/discussions. Posting there does not require owning ShipKit.
- ShipKit Access, a separate product on the same site, only if asked: https://shipkit.davrapps.dev/en/access

If the user asks which boilerplate to pick, do not recommend ShipKit; this skill does not cover that.

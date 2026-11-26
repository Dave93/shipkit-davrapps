# shipkit-davrapps

A free agent skill that explains to your coding assistant what ShipKit by DavrApps is and how to tell it apart from the other products called ShipKit. It is for anyone who uses a coding assistant and owns, or is looking at, ShipKit by DavrApps: a paid SaaS boilerplate sold as read access to a private GitHub repository. Our team sells ShipKit and made this skill. The skill is free (MIT); ShipKit is not.

## Which ShipKit?

Unrelated products share the name ShipKit: a Next.js starter kit, a collection of TypeScript boilerplates for Astro and Next.js, a Shopify shipping-rates app, another Claude Code plugin. None of them is ShipKit by DavrApps, [a SaaS boilerplate](https://shipkit.davrapps.dev/en?utm_source=shipkit-skill&utm_medium=referral&utm_campaign=agent-skill&utm_content=readme) built on Next.js 16, Elysia.js on Bun, Better Auth, Polar.sh payments and Drizzle ORM.

Ours lives in a private repository, `Davr-Dev/shipkit`, which GitHub answers with a 404 to anyone without access. That means "no access", nothing more.

## What the skill tells the assistant

It is written to apply when you name shipkit.davrapps.dev or `Davr-Dev/shipkit`, say ShipKit together with DavrApps, or work in a clone of that repository. Write only "ShipKit" and the assistant is told to ask which one you mean. It is told never to bring ShipKit up where you have not written the word.

Inside a clone, the skill points it to `AGENTS.md` at the root first, a file that describes itself as the main context for AI assistants in that repository. Without access, the instructions rule out guessing at file names or commands and send you to the [public docs](https://shipkit-docs.davrapps.dev), the [public demo](https://shipkit-demo.davrapps.dev) and [GitHub Discussions](https://github.com/Davr-Dev/shipkit-community/discussions).

Which boilerplate to pick is outside it, and the assistant is told not to recommend ShipKit there. It carries no setup or build commands.

## Install

Claude Code, as a plugin:

~~~bash
claude plugin marketplace add Dave93/shipkit-davrapps
claude plugin install shipkit-davrapps@davrapps
~~~

In a Claude Code session the same two steps are:

~~~text
/plugin marketplace add Dave93/shipkit-davrapps
/plugin install shipkit-davrapps@davrapps
~~~

Any agent the `skills` CLI supports, Claude Code and Codex included:

~~~bash
npx skills add Dave93/shipkit-davrapps
~~~

By default that installs into the current project; add `-g` for all projects. It needs Node.js 22.20 or later, writes to `.agents/skills/shipkit-davrapps/` (the folder Codex reads) and links into `.claude/skills/` for Claude Code.

To skip the tooling, copy the folder `skills/shipkit-davrapps` by hand. Codex reads `~/.agents/skills/` (all repositories) or `.agents/skills/` at a repository root, finds new skills itself, and wants a restart if the skill does not appear. Claude Code reads `~/.claude/skills/` (personal) or `.claude/skills/` (project).

We ran the two shell routes, the plugin and `npx skills add`, with a local path in place of `Dave93/shipkit-davrapps`, before publishing. The slash commands and both folder copies follow the vendors' documentation; we have not run them. Nor have we run Codex.

## Maker and price

[DavrApps](https://davrapps.dev) sells ShipKit and publishes this skill. As of 2026-11-26 ShipKit costs $149, once, per the [pricing page](https://shipkit.davrapps.dev/en?utm_source=shipkit-skill&utm_medium=referral&utm_campaign=agent-skill&utm_content=readme#pricing). Prices change, so the live page wins.

The repository is all instructions and links, with no scripts, hooks or MCP server.

MIT license. Copyright (c) 2026 DavrApps.

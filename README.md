# Dotfile plugin

Dotfile is the compliance platform for KYC and KYB onboarding. This plugin connects your assistant to your Dotfile workspace and adds skills that teach it how to work there: brief a case and what blocks it, read its history, audit screening, identity verification and documents, follow the team's workload and time to decision, and explain how your templates and automations are set up.

## Install

```sh
claude plugin marketplace add DotfileTech/dotfile-plugin
claude plugin install dotfile@dotfile
```

The connector signs you in to Dotfile the first time a tool runs. It needs a Dotfile account.

## Data and privacy

The plugin runs no code on your machine. Every tool call goes to the Dotfile connector at `https://mcp.dotfile.com/mcp`, and nowhere else.

The connector acts with your own Dotfile permissions and only sees the workspaces your account can see. Where your role allows it, its tools read and change your data: they can approve, reject or delete cases and checks, send communications to your customers, run bulk actions, and buy company data from paid registries, which is billed to your workspace.

Dotfile logs each tool call on its side: the tool, its arguments and its result.

How Dotfile handles personal data is described in the [privacy policy](https://www.dotfile.com/privacy) and the [terms of service](https://www.dotfile.com/terms).

## Contents

- `.mcp.json`: the Dotfile connector.
- `skills/`: one folder per skill.

## Support

Write to [support@dotfile.com](mailto:support@dotfile.com).

This repository is generated from the Dotfile monorepo on each production release. Changes made here are overwritten.

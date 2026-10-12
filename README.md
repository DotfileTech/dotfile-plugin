# Dotfile plugin

The Dotfile connector and the skills that teach the assistant how to use it.

## Install

```sh
claude plugin marketplace add dotfile/dotfile-plugin
claude plugin install dotfile@dotfile
```

The connector signs you in to Dotfile the first time a tool runs. It only sees the workspaces your Dotfile account can see.

## Contents

- `.mcp.json`: the Dotfile connector, `https://mcp.dotfile.com/mcp`.
- `skills/`: one folder per skill.

This repository is generated from the Dotfile monorepo on each production release. Changes made here are overwritten.

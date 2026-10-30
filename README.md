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

The connector acts with your own Dotfile permissions and only sees the workspaces your account can see. Where your role allows it, its tools read and change your data: they can approve, reject or delete cases and checks, send communications to your customers, and apply one of these actions to a whole selection as a bulk action, through one tool per action.

Two tools buy from the business data vendors your workspace is set up with: fresh company data, and registry documents. Each new request is a real purchase from the vendor, under the vendor contract your workspace uses, and counts toward your plan's limits, as the same request from the Dotfile console does. On your own vendor contract the vendor bills you; on Dotfile's, Dotfile bills the usage, except on trial and internal workspaces. Buying company data twice is a second purchase; ordering a document that was already ordered reuses that order unless it failed. A document's price tier is set when the order is placed and is usually the one listed beforehand. The assistant does not sell Dotfile subscriptions, plans or credits, and opens no checkout.

The connector does not take or return a person's social security or tax identification number through the fields that hold them, and refuses to query those fields. It withholds an identity document's number and MRZ wherever a check's data shows them, the compared values and description of a check finding about them, and the credentials of identity verification sessions. It does not return the files that show a government identifier:

- the images of an identity document and the identity verification vendor's report;
- identity verification videos, except the face-only videos of Checkout and Onfido;
- the files of document checks for identity documents, driving licences, visas, social security cards and tax notices, and of a person's document types whose key names a passport, an identity card, a residence permit, a driving licence, a visa, a social security or a tax identifier;
- documents to sign that Dotfile rendered from a document template, whose fields can include those numbers.

Portraits, signatures, face videos, uploaded documents to sign, audit trails and other documents stay readable. A document type the workspace named otherwise is not recognised, so its files stay readable even when they show an identifier. Free text is returned as written: notes, comments, communications, custom property values, AI review comments, the text of other documents and of purchased registry documents (an Italian company extract lists its officers' tax codes, for instance) can hold identifiers. Birth certificates and criminal record extracts, which carry a national identifier in some countries, stay readable too. Open the withheld data in the Dotfile console.

Dotfile logs each tool call on its side: the tool, its arguments and its result. A call refused for carrying a government identifier is logged without its values.

How Dotfile handles personal data is described in the [privacy policy](https://www.dotfile.com/privacy) and the [terms of service](https://www.dotfile.com/terms).

## Contents

- `.mcp.json`: the Dotfile connector.
- `skills/`: one folder per skill.

## Support

Write to [support@dotfile.com](mailto:support@dotfile.com).

This repository is generated from the Dotfile monorepo on each production release. Changes made here are overwritten.

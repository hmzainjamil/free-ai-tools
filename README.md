# Free AI Tools Directory

> A Next.js directory for browsing AI tools, categories, and suggested tool stacks.
> **Status:** Application source present; build and deployment status not assessed.

[Website source](website/) · [Contribution guide](CONTRIBUTING.md) · [License](LICENSE)

## What it does

The website presents a locally maintained catalog of AI tools and curated stacks. Visitors can browse categories, search entries, read tool and stack pages, view a news page, and follow the tool-submission guidance. The catalog is application data in the repository; this repository does not contain the model-routing CLI or audit system described in earlier README text.

## At a glance

| Area | Current state |
|---|---|
| Application | Next.js App Router under `website/` |
| Framework versions | Next.js 16.2.3 and React 19.2.4, as declared in `website/package.json` |
| Catalog data | `website/src/data/tools.ts`, `categories.ts`, and `stacks.ts` |
| Routes | Home, search, categories, tools, stacks, news, API information, submit, privacy, and terms |
| Runtime | Not verified by running the app |
| License | MIT, from [LICENSE](LICENSE) |

Catalog entries describe third-party products. Their free-tier, price, quota, model, and availability details can change; verify with each provider before relying on them.

## Browse the catalog

Use the deployed site if its current URL is provided by the repository owner. No deployment URL is established in the checked-in source reviewed for this guide.

For local development:

1. Install Node.js and a package manager supported by your environment.
2. Change to `website/`.
3. Install dependencies from `website/package.json` with your chosen Node package manager. No package lockfile is checked in, so dependency resolution may vary between installs.
4. Run one of the scripts declared in `website/package.json`.

The manifest declares `dev`, `build`, `start`, and `lint` scripts. This guide does not claim those commands have been run successfully. No root-level application install script or CLI is present in the inspected repository tree.

## How the site is organized

| Path | Purpose |
|---|---|
| `website/src/app/` | App Router pages and the news API route |
| `website/src/components/` | Shared interface components |
| `website/src/data/tools.ts` | Tool records, including descriptions, categories, pricing and feature fields |
| `website/src/data/categories.ts` | Category records |
| `website/src/data/stacks.ts` | Curated stack records |
| `website/src/types/index.ts` | TypeScript data types |
| `CONTRIBUTING.md` | Contribution instructions for catalog entries |

## Catalog review and contributions

The submission page directs visitors to submit tools through GitHub issues. The contribution guide requests official links and verification of free-tier details, pricing, model availability, card requirements, and last-checked date. Treat the guide as the repository's contribution policy; check current provider documentation before changing claims. Do not assume every current record has been recently re-verified.

## Data, privacy, and external services

The website includes a news API route that attempts to retrieve external pages and has fallback news records. Catalog entries link to third-party providers. Review `website/src/app/api/news/route.ts` and the privacy page before deployment: the presence of policy text does not itself verify production data handling or hosting configuration.

No model inference, fallback routing, telemetry pipeline, audit log, or autonomous agent runtime was found in the inspected source tree.

## Limitations and verification status

- Tool catalog claims are maintained data, not independently verified endorsements.
- Free tiers, quotas, prices, models, and provider terms can change.
- No build, lint, runtime, accessibility, or deployment check was run for this documentation update.
- Deployment URL, hosting settings, and production analytics behavior were not established.
- API behavior should be reviewed before public deployment, including its external fetch and fallback content.

## Documentation

| Guide | Purpose |
|---|---|
| [Contributing](CONTRIBUTING.md) | Catalog submission fields and review guidance |
| [Website README](website/README.md) | Website development and package-script reference; commands are declared, not verified by execution |
| [License](LICENSE) | Repository license |

## Security

This repository has no root `SECURITY.md` at the reviewed revision. For responsible vulnerability reporting, use a private channel controlled by the repository owner; avoid posting secrets or exploitable details in a public issue. Do not interpret this note as evidence of a monitored security process.

## License

Distributed under the MIT License. See [LICENSE](LICENSE).

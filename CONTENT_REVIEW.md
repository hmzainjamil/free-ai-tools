# Content review

## Scope reviewed

- Root `README.md`
- `CONTRIBUTING.md`
- `LICENSE`
- `website/package.json`
- `website/src/data/tools.ts`, `categories.ts`, and `stacks.ts`
- Website route tree and selected news, submit, privacy, and terms pages

## Findings

The checked-in product is a Next.js directory website with hard-coded TypeScript data for tools, categories, and stacks. The root README previously described a free AI orchestration runtime, CLI, model routing, telemetry, benchmarks, tests, integrations, and case studies. The inspected tree did not support those claims. The root README now describes the website and its contribution path.

Provider details in catalog records are time-sensitive and were not checked individually against provider primary sources. Do not present them as current verified facts without dated review. Some documentation paths previously linked from the root README were absent from the repository tree.

## Validation

- Repository tree checked through GitHub API.
- Relative links in the revised README point to paths present in the checked tree.
- No app build, lint, tests, browser run, deployment check, or catalog fact-check was performed.

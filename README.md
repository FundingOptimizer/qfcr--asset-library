# QFCR Asset Library

**Org:** FundingOptimizer  
**Purpose:** Single source of truth for UI components, underwriting rules, themes, embeds/SDK, analytics schema, and API contracts used across StackLoans, FundingOptimizer, FranchiseScope, and partner builds.

## Contents
- `src/ui` — score dials, progress rings, XP tracker
- `src/themes` — token file + CSS vars
- `src/analytics` — canonical event schema + GTM mapping
- `src/rules` — unified underwriting rules
- `src/sdk` — React SDK wrapper + iframe fallback
- `src/api` — OpenAPI spec and TS contracts
- `examples` — quick-start snippets
- `scripts` — install/wiring helpers
- `CHANGELOG.md` — versioned changes

## Install (as npm GitHub package)
```bash
# package.json in consuming repo
# "dependencies": { "@fundingoptimizer/qfcr-assets": "github:FundingOptimizer/qfcr--asset-library#v0.1.0" }

# or temporarily via file path
npm i github:FundingOptimizer/qfcr--asset-library#v0.1.0
```

## Install (as git submodule)
```bash
git submodule add https://github.com/FundingOptimizer/qfcr--asset-library.git vendor/qfcr
git -C vendor/qfcr submodule update --init --recursive
```

## Usage
```tsx
import { ScoreDial, ProgressRing, XPTrack } from "@fundingoptimizer/qfcr-assets/dist/ui";
import tokens from "@fundingoptimizer/qfcr-assets/dist/themes/qfcr.tokens.json";
import schema from "@fundingoptimizer/qfcr-assets/dist/analytics/analytics.schema.json";
```

## Versioning
Follow semantic versioning. Update `CHANGELOG.md` and bump `package.json`.

_Last updated: 2025-08-13_

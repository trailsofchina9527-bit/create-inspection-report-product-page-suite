# Inspection Report Product Page Suite

A reusable Codex skill that turns a product inspection report PDF into an English ecommerce product page package.

For each product, the workflow:

1. Audits the report and separates verified measurements from observations and unsupported claims.
2. Extracts the primary embedded product image, removes product branding when appropriate, and creates a 1:1 white-background hero image.
3. Writes customer-facing English product copy and SEO metadata from verified facts.
4. Produces nine coordinated 1:1 English product-detail images, including realistic use scenes, features, dimensions, and package contents.

The expected deliverables are a logo-free photo, a square white-background hero, nine square detail images, product-page copy, and SEO metadata. The skill also requires quality checks for image consistency, exact measurements, legible text, and unsupported claims.

## Install

Copy this repository into your Codex skills directory so that `SKILL.md` is at the root of the skill folder. Keep `agents/` and `references/` alongside it.

```text
create-inspection-report-product-page-suite/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── content-and-seo.md
    └── nine-image-set.md
```

Then provide a product inspection report PDF and ask Codex to create the complete product-page package. The default final images are all square (1:1), and all consumer-facing copy is in English.

## Scope

This repository contains only reusable workflow instructions. It does not include inspection reports, customer files, generated product photos, or shop credentials.

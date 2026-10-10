---
name: create-inspection-report-product-page-suite
description: "Turn a product inspection-report PDF into a complete English ecommerce product-page package: extract and debrand the primary product photo, create a square white-background hero, extract verified specifications, write SEO-ready product copy, and produce nine coordinated product-detail images. Use when the user supplies an inspection, QC, pre-shipment, or factory report and wants finished listing assets rather than a report summary alone."
---

# Create Inspection Report Product Page Suite

Produce a finished ecommerce asset package from the supplied inspection report. The default customer is a Western-facing DTC or marketplace store, so final consumer copy and all text inside images must be English unless the user requests another language.

## Required outcome

Deliver all four asset groups:

1. A logo-free extraction of the report's primary product photo.
2. A 1:1 pure-white ecommerce hero image.
3. SEO-ready product-page copy based only on verified facts and defensible visual observations.
4. Nine coordinated, text-complete 1:1 product-detail images.

Do not stop at prompts, outlines, extracted notes, or untypeset backgrounds.

## Workflow

### 1. Audit the report

- Render and visually inspect relevant pages; do not rely only on PDF text extraction.
- Locate the clearest primary product photo and extract its original embedded image when possible.
- Search the complete report for product dimensions, weight, materials, packaging, carton measurements, included components, construction, performance tests, warnings, failed or untested checks, and inspection photographs.
- Resolve conflicts by distinguishing client specification, carton marking, and actual measured value. Prefer actual verified measurements for the customer-facing specification table and record the distinction internally.
- Separate facts into `Verified`, `Observed`, and `Unsupported`.

Never promote unsupported claims such as waterproofing, UV resistance, flammability compliance, capacity, setup time, material composition, or certification.

### 2. Build the product-image masters

- Extract the report's main product photo at native resolution.
- If the product carries a logo or brand mark and the user wants a generic product, remove only that mark and reconstruct the underlying material or pattern. Preserve product geometry, seams, openings, hardware, lighting, background, and other details.
- Create a separate 1:1 ecommerce hero with a uniform pure-white background, balanced margins, realistic perspective, subtle contact shadow, and no logo, watermark, timestamp, props, or incidental text.
- Preserve the logo-free product's recognizable shape, pattern, color, construction, and hardware. Save both masters non-destructively.

### 3. Create SEO-ready English copy

Read [references/content-and-seo.md](references/content-and-seo.md) before keyword selection or copywriting.

- Use the product's real category and purchase intent as the primary keyword.
- Use current search-result language or live keyword data when available; never invent search volume or ranking difficulty.
- Keep the product name readable and specific. Place the category keyword before secondary features.
- Make the SEO title, H1, meta description, URL slug, headings, body copy, specifications, package contents, and image alt text agree with one another.
- Write direct customer-facing copy. Do not include drafting commentary such as “safe marketing wording,” “recommended claim,” or “the report says.”
- Include useful secondary phrases naturally; do not repeat mechanical keyword variants.

### 4. Produce the nine-image detail set

Read [references/nine-image-set.md](references/nine-image-set.md) before generating the visual set.

- Classify the physical product category first; let real usage determine environments, camera language, interaction, and proof.
- Build one campaign visual lock covering aspect ratio, palette, lighting, typography, negative space, product scale, and image treatment.
- Use the logo-free product master as the identity reference for every frame.
- Generate one distinct background or composition per frame. Preserve product identity across all nine.
- Do not ask the image model to render final words or measurements. Add canonical English copy with deterministic layout tools.
- Use English only. Reject corrupted words, random letters, pseudo-text, CJK characters, watermarks, unverified badges, and incidental brand marks.
- Validate quantities in accessory images. Regenerate or correct any duplicated or missing component.
- Every product-detail image must use a 1:1 square canvas. Keep the square format consistent across all nine frames unless the user explicitly requests a different ratio for a specific run.

## Quality gates

Do not deliver until all gates pass:

- The extracted photo is the original product image, not a page screenshot when an embedded image exists.
- Logo removal is locally plausible and does not redesign the product.
- The white-background hero is exactly 1:1 and visually white to the edges.
- Dimensions and conversions match the verified report values.
- Consumer copy contains no factory, inspection-process, defect-code, or purchase-order material unless commercially useful.
- Conditional or untested inspection items are not turned into performance claims.
- All nine images are present, coordinated, exactly 1:1, English-only, and free of text overlap.
- Lifestyle scenes are plausible interpretations, not documentary claims.
- Final files are saved inside the active workspace with stable, descriptive names.

## Delivery structure

Use a stable folder such as:

```text
output/<product-id>/
|-- product-images/
|   |-- 01-logo-free-main.png
|   `-- 02-white-background-square.png
|-- copy/
|   |-- product-page-copy.md
|   `-- seo-metadata.md
`-- detail-pages/
    |-- 01-product-hero.png
    |-- 02-primary-use-scene.png
    |-- 03-secondary-use-scene.png
    |-- 04-concealment-or-core-benefit.png
    |-- 05-feature-and-structure.png
    |-- 06-product-dimensions.png
    |-- 07-material-and-detail.png
    |-- 08-fold-pack-carry.png
    `-- 09-package-contents.png
```

At handoff, list every deliverable group and provide clickable paths. Report the image dimensions, the chosen primary SEO keyword, material assumptions, any omitted claims, and whether lifestyle scenes were generated.

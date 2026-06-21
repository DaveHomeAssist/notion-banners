# How these banners were made

Provenance and reproduction notes for the `cover_*.png` Notion sidebar banner covers.

## Specs

| Field | Value |
|---|---|
| Asset set | `cover_01.png` … `cover_16.png` (16 tiles) |
| Slice dimensions | **624 × 290 px** each (Notion top-level page cover ratio) |
| Format | PNG, art-only (no text baked in) |
| Intended use | Banner covers for top-level "Dave OS" Notion sidebar pages |

## Generator tool

UNKNOWN. No generator script, config, or tooling is committed to this repo, and none was found anywhere in the workspace as of the 2026-06-21 audit. The covers appear to be a one-off slice of a wider source image (consistent dimensions across all 16 tiles suggest a single source banner cut into segments), but the exact tool/pipeline is not recoverable from version control.

## Source image / prompt

UNKNOWN. No source image, slice coordinates, or generation prompt is committed. If these were AI-generated, the prompt was not preserved. There is also no committed mapping of which `cover_NN.png` belongs to which Notion page — that assignment currently lives only inside Notion.

## Date produced

Recorded at the **2026-06-21** Creative & Design Tools bucket audit. The covers were committed earlier (single commit "Add 16 Notion sidebar banner covers"); the exact creation date is not independently documented.

## Reproducibility & canonical direction

This repo is the **canonical asset store** for these covers and is currently **not reproducible** — losing the source material would freeze the set as-is.

- **Do NOT create a separate `notion-banner-generator` repo.** (The 2026-06-21 audit confirmed no such repo exists on disk, as a git remote, or in any reference — it is a phantom, not a missing twin.)
- If/when regeneration or re-slicing becomes necessary, **fold the source material into this repo** rather than splitting it out: e.g. add `src/` containing the source banner image plus a small slice script (slicing to 624×290), and record the generation prompt here. That keeps generator + output co-located and closes the reproducibility gap without the repo split the audit warned against.

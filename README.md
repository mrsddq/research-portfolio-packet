# Research Portfolio Packet

Academic-style framing packet for AI, computer vision, MLOps, and DevOps portfolio work.

This repository contains research proposals, reading notes, and experiment templates for the linked implementation repositories. It does not establish completed benchmark results or publication readiness. Source code, automated smoke tests, and measured dataset experiments are separate evidence categories.

## Structure

```text
abstracts/
one-pagers/
templates/
```

## Included Project Tracks

| Track | Source Repo | Purpose |
|---|---|---|
| medical segmentation | `medical-segmentation` | research signal |
| object detection | `yolov8-detection` | CV fundamentals |
| image captioning | `clip-image-captioning` | multimodal relevance |
| ViT robustness/XAI | `vit-robustness-xai` | advanced vision relevance |
| OCR pipeline | `ocr-pipeline` | industry usability |
| pose QA | `pose-estimation-qa` | dataset quality/evaluation |

## Usage

1. Start with `templates/project-one-pager.md`.
2. Create a one-pager for each portfolio repo.
3. Move real metrics from project repos into the result sections.
4. Keep claims honest: no benchmark claim without reproducible artifact links.

Use [docs/EVIDENCE_REQUIREMENTS.md](docs/EVIDENCE_REQUIREMENTS.md) before writing a paper-style summary.

## Current Status

Research framing is ready. Real papers, posters, or submissions require actual experiment runs, figures, and reviewer-quality citations.

The one-pagers describe intended studies. Their requested metrics remain pending
until a run record includes the dataset/split, exact code revision, command,
environment, output artifact and limitations. Use
[the experiment record template](templates/experiment-record.json) and
[the evidence requirements](docs/EVIDENCE_REQUIREMENTS.md). Passing a repository's
offline tests proves the tested contracts; it does not substitute for medical,
captioning, detection, OCR or robustness benchmark evaluation.

`make verify` checks documentation whitespace only. This repository does not run
the linked models; use each implementation's documented commands and CI.

# CLIP Image Captioning One-Pager

Source: https://github.com/mrsddq/clip-image-captioning

Status: proposed benchmark study; measured results are not supplied in this packet. See the source repository for runnable implementation and test status.

## Problem

Generate natural-language captions from images using CLIP visual embeddings and a Transformer decoder.

## Method

Frozen CLIP encoder pattern with configurable Transformer decoder and planned COCO/Flickr evaluation.

## Evidence Needed

- BLEU, METEOR, and CIDEr
- caption examples
- decoder ablations
- failure cases for hallucination or under-description

## Limitation

Frozen embeddings may limit domain adaptation.

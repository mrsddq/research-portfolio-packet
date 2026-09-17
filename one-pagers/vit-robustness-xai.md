# ViT Robustness XAI One-Pager

Source: https://github.com/mrsddq/vit-robustness-xai

Status: proposed benchmark study; measured results are not supplied in this packet. See the source repository for runnable implementation and test status.

## Problem

Evaluate Vision Transformer behavior under corruptions, subgroup splits, and explanation visualizations.

## Method

Config-driven robustness evaluation, subgroup gap calculation, and attention rollout heatmap generation.

## Evidence Needed

- clean baseline accuracy
- corruption severity curves
- subgroup gap table
- attention rollout examples

## Limitation

Attention rollout is diagnostic and should not be treated as causal proof.

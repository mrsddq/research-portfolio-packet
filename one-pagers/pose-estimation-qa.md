# Pose Estimation QA One-Pager

Source: https://github.com/mrsddq/pose-estimation-qa

Status: proposed benchmark study; measured results are not supplied in this packet. See the source repository for runnable implementation and test status.

## Problem

Detect suspicious COCO-style pose annotations before training or evaluation.

## Method

Schema, spatial, and temporal QA checks with reviewer-facing visualization outputs.

## Evidence Needed

- labelled reviewer set
- precision/recall for QA flags
- reviewer workload reduction
- flagged skeleton overlays

## Limitation

QA rules reduce annotation noise; they do not replace human review.

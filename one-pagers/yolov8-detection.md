# YOLOv8 Detection One-Pager

Source: https://github.com/mrsddq/yolov8-detection

Status: proposed benchmark study; measured results are not supplied in this packet. See the source repository for runnable implementation and test status.

## Problem

Detect street-scene objects using a focused three-class YOLOv8 setup.

## Method

Config-driven Ultralytics YOLOv8 training, validation, and inference pipeline with class-level reporting plan.

## Evidence Needed

- dataset stats and class balance
- mAP50-95, precision, recall
- confusion matrix
- prediction/failure-case images

## Limitation

Frame-level detection only; no video tracking yet.

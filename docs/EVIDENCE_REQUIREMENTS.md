# Evidence Requirements

Use this before turning a project into a one-pager, poster, or paper-style summary.

## Required Inputs

- Link to source repo.
- Exact commit or release used for the run.
- Dataset name, split, and license note.
- Training or evaluation command.
- Metric table from a reproducible output file.
- At least one qualitative figure.
- Limitations and failure cases.

## Claim Rules

- Do not call a result state-of-the-art unless compared against a cited benchmark.
- Do not report private-data metrics without explaining the data boundary.
- Do not turn smoke-test artifacts into benchmark claims.
- Mark planned experiments as planned, not completed.

## Reproducible run record

Start with [experiment-record.json](../templates/experiment-record.json). Keep
`status` as `planned` until the stated command finishes and its artifacts exist.
Record a full commit SHA, dependency versions, random seed, dataset license and
split identity. Record metric units, aggregation (per sample or corpus), sample
count, and how missing/failed predictions are handled. Do not silently drop failed
cases, tune on a held-out test set, or aggregate incompatible splits.

A result must link to a machine-readable metrics file and its SHA-256. Record
training and evaluation separately, including the checkpoint identifier; an
untrained smoke checkpoint is not a trained baseline. For medical data, retain
image spacing/orientation and disclose the split unit (patient vs image).

Implementation changes should identify the failed behavior, regression case and
current CI result. Keep that engineering evidence alongside, but separate from,
model-quality results. CPU synthetic tests can validate tensor shapes, geometry,
masking and error paths without making a dataset-accuracy claim.

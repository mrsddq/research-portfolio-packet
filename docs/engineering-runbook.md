# Research evidence runbook

This repository holds project proposals, reading notes and reporting templates.
It is not a collection of completed benchmark results.

## Prepare a project summary

1. Open the relevant project in the [README](../README.md).
2. Follow the [evidence requirements](EVIDENCE_REQUIREMENTS.md).
3. Copy the [experiment record](../templates/experiment-record.json), record the
   source commit, dataset split, command and environment, and keep status `planned`
   until execution completes.
4. Link measured artifacts and limitations from the project's one-pager.

```bash
make verify
python -m json.tool templates/experiment-record.json > /dev/null
```

The first command checks whitespace; the second checks JSON syntax. Neither runs
experiments or validates model quality. Run implementation tests and experiments
inside each linked source repository using its documented environment.

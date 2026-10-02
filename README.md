# Ellipsis mention handlers

Ellipsis reads `linear.yaml` and `github.yaml` from the root of this repository, on the default branch. These replace the built-in mention handler.

The Grafana alert agent and the `maxim` sandbox live in [MaximVote/maxim](https://github.com/MaximVote/maxim) under `.ellipsis/`. This repo does not hold those.

Both handlers use the `maxim` environment from that product repo. It has to be on `maxim`'s default branch (`qa`) before a mention can install the Grafana and GCP tools. Until then, a mention still starts, and the session reports a missing environment.

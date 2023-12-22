# Artifact Expiry Demo

This repository contains a demonstration of a bug in GitHub Actions where the artifact retention time is not being properly applied, and it is possible to download artifacts after they have expired.

To demonstrate run the workflow via a workflow dispatch, wait at least 24 hours, then rerun just the upload job of the workflow. It will be able to download and display the artifact that should have expired.

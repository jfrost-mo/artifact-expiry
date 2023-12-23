# Artifact Expiry Demo

This repository contains a demonstration of a bug in GitHub Actions where the artifact retention time is not being properly applied, and it is possible to download artifacts after they have expired.

To demonstrate run the workflow via a workflow dispatch, wait at least 24 hours, then rerun just the upload job of the workflow. It will be able to download and display the artifact that should have expired.

For example, the artifact had expired as seen in the picture, but the [second actions run managed to download and print it](https://github.com/jfrost-mo/artifact-expiry/actions/runs/7300639474/job/19916958081#step:3:5) after 25 hours and 51 minutes, nearly 2 hours more than expected.

![Screenshot 2023-12-23 at 16-48-19 Artifact Expiry Demo · jfrost-mo_artifact-expiry@881327c](https://github.com/jfrost-mo/artifact-expiry/assets/113985160/bb53dabe-38f3-4f2e-a662-23098d1e56dc)

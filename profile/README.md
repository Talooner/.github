## Talooner

Deterministic code review for GitHub and GitLab pipelines. Talooner runs as one Docker image
in your CI job, checks each pull or merge request against your repository's
`.talooner/rules.tln`, posts a check run and a comment, and exits. No server to host.

```sh
docker run --rm ghcr.io/talooner/talooner-runner:latest snippet github   # or gitlab | generic
```

**Found a bug or stuck during setup?** Open an issue in
[Talooner/feedback](https://github.com/Talooner/feedback/issues/new/choose).

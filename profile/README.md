## Talooner

Deterministic code review for GitHub and GitLab pipelines. Talooner runs as one Docker image
in your CI job, checks each pull or merge request against your repository's
`.talooner/rules.tln`, posts a check run and a comment, and exits. No server to host.

```sh
docker run --rm ghcr.io/talooner/talooner-runner:latest snippet github   # or gitlab | generic
```

## Onboard with your coding agent

Install the [`talooner-onboard` skill](https://github.com/Talooner/talooner-skills) and ask
your agent to onboard the repository. It interviews you, writes tested rules, guides and CI,
and prepares a draft pull request:
[docs and install steps](https://talooner.dev/onboard/).

```sh
mkdir -p ~/.claude/skills
cp -R talooner-onboard ~/.claude/skills/
```

Use `~/.config/opencode/skills/` for OpenCode or `.agents/skills/` for Codex or `~/.claude/skills/` for Claude. Requirements:
Docker, a Talooner license with AI review, an AI review key, and a context decision model key.

**Found a bug or stuck during setup?** Open an issue in
[Talooner/feedback](https://github.com/Talooner/feedback/issues/new/choose).

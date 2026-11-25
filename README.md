# cascadiacollections/.github

Default community health files for every repository in the `cascadiacollections` organization.
GitHub uses each of these for any repository that doesn't have its own copy:

- [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md): Contributor Covenant 2.1
- [`CONTRIBUTING.md`](CONTRIBUTING.md): DCO sign-off and contribution licensing
- [`FUNDING.yml`](FUNDING.yml): the Sponsor button
- [`SECURITY.md`](SECURITY.md): how to report a vulnerability privately
- [`SUPPORT.md`](SUPPORT.md): where to ask questions, and that replies are best effort
- [`PULL_REQUEST_TEMPLATE.md`](PULL_REQUEST_TEMPLATE.md): summary, test plan, and checkboxes for publishing and breaking changes
- [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/): bug and feature forms. Blank issues stay available. Questions go to [Discussions](https://github.com/orgs/cascadiacollections/discussions). Vulnerabilities go to the security policy.

A repository's own file always wins over these defaults. GitHub looks in that repository's `.github`
folder, then its root, then `docs`. For issue templates, any file in the repository's
`.github/ISSUE_TEMPLATE` replaces this whole set. `saltline` only has a bug form, and that is
enough to keep these forms from applying there.

These repositories already have their own copy (checked 2026-11-25). Forks are not listed. They keep the copies they already have.

| File | Repositories with their own copy |
| --- | --- |
| Code of conduct | podr, smodr |
| Contributing | node-gittip, podr, shoutkit, shoutkit-android, sir-chrome-extension, sk-tic-tac-toe, smodr, smodr-winui3 |
| Funding | fluentui-compat, podr, shoutkit, smodr |
| Security | bauhaus-android, juniperleaves, podr, shoutkit, shoutkit-android, sir-chrome-extension, smodr, smodr-winui3 |
| Support | none |
| Pull request template | juniperleaves, shoutkit, sir-chrome-extension, sk-tic-tac-toe |
| Issue templates | bauhaus-android, juniperleaves, podr, saltline, shoutkit, shoutkit-android, sir-chrome-extension, sk-tic-tac-toe, smodr, smodr-winui3 |

`CODEOWNERS` is not here. GitHub does not inherit one, so a repository that wants reviewers adds its own.

[`workflow-templates/`](workflow-templates/) holds Scorecard and CodeQL starters. They do not run on
their own. In a repository, open **Actions**, then **New workflow**, and pick one. GitHub fills in
the default branch name when the workflow is created. The actions are pinned to the same commits as
`KevinTCoughlin/godot-xdg-portals`. The CodeQL starter analyzes Actions workflows. Add a language to
the matrix for application code, and skip it when that repository already uses CodeQL default setup.

# Contributing

Thank you for helping Awesome Developer Environments. By participating, you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).

This organization installs **standard tools on a developer local machine**.  
We do not ship sample applications or project skeletons.

## Where to contribute

Work in the **stack repository** that owns the toolchain (`java`, `csharp`, `python`, `golang`).  
Use this `.github` repository for organization docs, issue templates, copyable authoring templates, and the installer skill.

| Change                                                   | Where                                              |
|----------------------------------------------------------|----------------------------------------------------|
| New tool, package mapping, silent install args           | That stack’s `tools.yml`                           |
| Installer bug or step logic                              | That stack’s `init.sh` / `init.ps1` and `scripts/` |
| Translation                                              | That stack’s `i18n/` (all locales)                 |
| Org profile, community files, skill, authoring templates | This repository                                    |

- Questions belong in [GitHub Discussions](https://github.com/orgs/awesome-dev-envs/discussions).
- Bugs and improvements belong in Issues (use the templates).

## Bootstrap a new stack repository

1. Create an empty `awesome-dev-envs/<stack>` repository.
2. Copy `.cursor/skills/dev-env-installer/` from this repo (required). Optionally copy `templates/*`.
3. With the skill loaded, generate the installer for that stack’s **standard local tools**.
4. Keep the stack repo limited to installer assets: orchestrators, step scripts, `tools.yml`, i18n, and a short README.

## Pull requests

English only. Use the installer skill when changing scripts, `tools.yml`, or i18n.

Checklist:

- [ ] User-facing strings live in i18n; keys exist in `en`, `es`, `de`, `fr`, `it`, and `pt`
- [ ] Every tool can be installed, skipped, or updated
- [ ] Native package manager is tried before download fallbacks
- [ ] Silent install args are set for Windows installers
- [ ] Unix (`init.sh`) and Windows (`init.ps1`) stay aligned
- [ ] You agree to the [Code of Conduct](CODE_OF_CONDUCT.md)

## License

Contributions are licensed under [MIT](LICENSE).

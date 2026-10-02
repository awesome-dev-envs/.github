# Awesome Developer Environments

Built for speed, automate, and effortless **local machine** environments for onboardings.

## What we do

We publish documentation, templates, and automated **tooling setup** so a developer computer is ready in minutes.  
Installers use native package managers (`apt`, `dnf`, `pacman`, `brew`, `winget`) and download fallbacks when a package is missing.

- **Fast onboarding:** run one command, follow the prompts, start working.
- **Community first:** built by developers, for developers. This is not an application framework.

## Key projects

Each repository installs a **local toolchain** for that stack (no sample apps).

| Repository                                           | Description                         |
|------------------------------------------------------|-------------------------------------|
| [java](https://github.com/awesome-dev-envs/java)     | Java / JVM tools on your machine    |
| [csharp](https://github.com/awesome-dev-envs/csharp) | .NET / C# tools on your machine     |
| [python](https://github.com/awesome-dev-envs/python) | Python runtime and common CLI tools |
| [golang](https://github.com/awesome-dev-envs/golang) | Go toolchain and related CLIs       |

## Usage

Pick a stack, run the one-liner, then install, skip, or update each tool.

Optional flags: `--lang`, `--profile`, `--appIds`, `--UpdateIfExists`.  
If you omit both `--profile` and `--appIds`, the script asks you to choose a profile.

- Windows uses powershell and winget.
- macOS uses bash/zsh and Homebrew.
- Linux distros (Ubuntu, Fedora, Arch, and similar) are detected inside `init.sh`.

## Overview

Tools are declared in each stack’s `tools.yml`.  
Profiles (Backend, Frontend, DevOps, Fullstack, QA) filter that list; you can still skip or pin individual apps.  
Prompts are translated (`en`, `es`, `de`, `fr`, `it`, `pt`).  
Stack READMEs cover the rest once those repositories exist.

## How to contribute

We welcome all contributions.
See [CONTRIBUTING.md](https://github.com/awesome-dev-envs/.github/blob/main/CONTRIBUTING.md) and our [Code of Conduct](https://github.com/awesome-dev-envs/.github/blob/main/CODE_OF_CONDUCT.md).

## License

See [MIT LICENSE](https://github.com/awesome-dev-envs/.github/blob/main/LICENSE).

## Important note

If something is wrong, missing, or a poor fit, open an issue or a pull request. Thank you.

## Get in touch

- **[GitHub Discussions](https://github.com/orgs/awesome-dev-envs/discussions):** questions and ideas
- **[GitHub Issues](https://github.com/awesome-dev-envs/.github/issues):** bugs and improvements

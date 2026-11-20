---
default: major
---

# Update to parent template 0.8.4

Replaces Trunk, release-please, and the Invoke tasks with mise, prek, and Knope, and restructures the workflows and docs. See the [parent's upgrade guide](https://postmodern-templates.github.io/repo-template/latest/maintaining/upgrading-from-0x/).

`k8s_envs` now lives in `copier.yml`'s `Helm Deploy Questions` region instead of an included `copier-deployment-envs.yml`. A child template moves its environments into that region, and its deploy pipeline is registered as `[<repo>] Deploy (Manual) - Helmfile Sync` on a new copy.

# Changelog

## 1.1

### 1.2.0 - 2024-02-03

([full changelog](https://github.com/jupyterhub/action-k8s-namespace-report/compare/v1.1.0...v1.2.0))

#### Enhancements made

- Group pod outputs since they can be very long [#20](https://github.com/jupyterhub/action-k8s-namespace-report/pull/20) ([@manics](https://github.com/manics), [@consideRatio](https://github.com/consideRatio))
- Add listing of cronjobs and jobs [#13](https://github.com/jupyterhub/action-k8s-namespace-report/pull/13) ([@consideRatio](https://github.com/consideRatio), [@manics](https://github.com/manics))

#### Maintenance and upkeep improvements

- dependabot: monthly updates of github actions [#21](https://github.com/jupyterhub/action-k8s-namespace-report/pull/21) ([@consideRatio](https://github.com/consideRatio))

#### Documentation improvements

- Update readme example and ci details [#25](https://github.com/jupyterhub/action-k8s-namespace-report/pull/25) ([@consideRatio](https://github.com/consideRatio))

#### Continuous integration improvements

- ci: add dependabot for gha, update workflows generally, and use v1,v2,etc tags instead of branches, use pre-commit.ci [#16](https://github.com/jupyterhub/action-k8s-namespace-report/pull/16) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

The following people contributed discussions, new ideas, code and documentation contributions, and review.
See [our definition of contributors](https://github-activity.readthedocs.io/en/latest/#how-does-this-tool-define-contributions-in-the-reports).

([GitHub contributors page for this release](https://github.com/jupyterhub/action-k8s-namespace-report/graphs/contributors?from=2021-09-25&to=2024-02-03&type=c))

@consideRatio ([activity](https://github.com/search?q=repo%3Ajupyterhub%2Faction-k8s-namespace-report+involves%3AconsideRatio+updated%3A2021-09-25..2024-02-03&type=Issues)) | @manics ([activity](https://github.com/search?q=repo%3Ajupyterhub%2Faction-k8s-namespace-report+involves%3Amanics+updated%3A2021-09-25..2024-02-03&type=Issues))

### 1.1.0 - 2021-09-25

#### Enhancements made

- Show PersistentVolumes and PersistentVolumeClaims [#11](https://github.com/jupyterhub/action-k8s-namespace-report/pull/11) ([@manics](https://github.com/manics))
- Add pod-selector input to limit reporting [#6](https://github.com/jupyterhub/action-k8s-namespace-report/pull/6) ([@consideRatio](https://github.com/consideRatio))
- Show info about restarted pods before pending/non-ready pods [#4](https://github.com/jupyterhub/action-k8s-namespace-report/pull/4) ([@consideRatio](https://github.com/consideRatio))

#### Bugs fixed

- fix: don't let namespace modify kubeconfig's current context [#5](https://github.com/jupyterhub/action-k8s-namespace-report/pull/5) ([@consideRatio](https://github.com/consideRatio))

#### Continuous integration

- ci: ensure actions-tagger has the permissions to update branches/tags [#8](https://github.com/jupyterhub/action-k8s-namespace-report/pull/8) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/action-k8s-namespace-report/graphs/contributors?from=2021-01-11&to=2021-09-25&type=c))

[@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Faction-k8s-namespace-report+involves%3AconsideRatio+updated%3A2021-01-11..2021-09-25&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Faction-k8s-namespace-report+involves%3Amanics+updated%3A2021-01-11..2021-09-25&type=Issues)

## 1.0

### 1.0.1 - 2021-01-11

Critical bugfix and documentation improvements.

### 1.0.0 - 2021-01-11

Initial release.

# Changelog

## 1.1

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

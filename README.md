# GitHub Action: Emit a k8s namespace report
[![GitHub Action badge](https://github.com/jupyterhub/action-k8s-namespace-report/workflows/Test/badge.svg)](https://github.com/jupyterhub/action-k8s-namespace-report/actions)

GitHub Action to report info and logs from the current namespace.

## Optional input parameters
- `namespace`: Updates the kubeconfig's current context's namespace.

## Example

```yaml
name: Example workflow

on:
  pull_request:
  push:
  workflow_dispatch:

jobs:
  k8s-test:
    runs-on: ubuntu-20.04
    steps:
      # GitHub Action reference: https://github.com/jupyterhub/action-k3s-helm
      - name: Start k8s locally
        uses: jupyterhub/action-k3s-helm@v1
        with:
          k3s-channel: v1.20    # https://update.k3s.io/v1-release/channels

      # GitHub Action reference: https://github.com/jupyterhub/action-k8s-namespace-report
      - name: K8s namespace report
        uses: jupyterhub/action-k8s-namespace-report@v1
        # with:
        #   namespace: my-non-default-namespace
```

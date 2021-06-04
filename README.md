# GitHub Action: Emit a k8s namespace report
[![GitHub Action badge](https://github.com/jupyterhub/action-k8s-namespace-report/workflows/Test/badge.svg)](https://github.com/jupyterhub/action-k8s-namespace-report/actions)

GitHub Action to report info and logs from the current namespace.

## Optional input parameters
- `namespace`: Emit a report for another namespace than the kubeconfig's current
  context.
- `pod-selector`: Limit pod reporting to pods with certain labels, example:
  `app.kubernetes.io/component notin (secret-server,boring-server)`.
- `important-workloads`: Always provide logs of these workloads. Use space a
  separator, example: `deploy/my-deployment sts/my-statefulset`.

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
      - name: Setup k8s
        uses: jupyterhub/action-k3s-helm@v1
        with:
          k3s-channel: v1.20    # https://update.k3s.io/v1-release/channels

      # GitHub Action reference: https://github.com/jupyterhub/action-k8s-namespace-report
      - name: Kubernetes namespace report
        uses: jupyterhub/action-k8s-namespace-report@v1
        if: always()
        # with:
        #   namespace: my-namespace
        #   pod-selector: app.kubernetes.io/component notin (secret-server,boring-server)
        #   important-workloads: deploy/my-deployment sts/my-statefulset
```

## Preview

__Live example__

You can inspect recent test runs [here](https://github.com/jupyterhub/action-k8s-namespace-report/actions?query=workflow%3ATest).

__GIF Animation__

![](https://user-images.githubusercontent.com/3837114/104154471-4b3f7c00-53e5-11eb-8ebf-d54c22af12ed.gif)

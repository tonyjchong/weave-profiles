# How to set up a helm repo using GitHub Pages

1. https://harness.io/blog/helm-chart-repo (Step 1 - 3)
2. Get the right GitHub actions from the original repo or copy the actions here
  
## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add <alias> https://tonyjchong.github.io/weave-profiles

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the <chart-name> chart:

    helm install my-<chart-name> <alias>/<chart-name>

To uninstall the chart:

    helm delete my-<chart-name>


## Test
```
helm repo add tony https://tonyjchong.github.io/weave-profiles
helm search repo tony
helm install 
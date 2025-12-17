# NGINX Manifest
Example of fully rendered manifests.  This manifest can be applied to multiple clusters in App Flows by specifying multiple target clusters when registering this repository under Edge Kubernetes -> GitOps Repository.

## Creation
These manifests were created by executing the following:
```sh
# from repo top level
helm template --release-name v1.0 nginx/helm
```

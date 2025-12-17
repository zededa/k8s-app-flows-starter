# NGINX Kustomize
Kustomize build for nginx.

## Usage
- Render manifests: `kubcetl kustomize .`

## Customization
- Release name/labels: set `namePrefix` and `commonLabels` in `kustomization.yaml` (behaves like `.Release.Name` and `.Values.labels`).
- Image tag/repo: update the `images` block in `kustomization.yaml`.
- Replicas or ports: edit `deployment.yaml` / `service.yaml` directly or add patches.
- Service type/nodePort: change `spec.type` (and add `nodePort` if desired) in `service.yaml`.

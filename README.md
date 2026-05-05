# mcp-k8s

Kubernetes kubectl/helm MCP server for Tank sessions.

## Layout

- `src/` - Python MCP server package.
- `Dockerfile` - image build for `romainecr.azurecr.io/mcp-k8s`.
- `chart/` - Helm chart synced by ArgoCD.

Images are SHA-tagged from `main`; `.github/workflows/build.yml` pushes the image and commits the matching chart tag.

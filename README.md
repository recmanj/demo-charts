# Demo Charts

Helm charts for demo-backend (FastAPI) and demo-frontend (React/nginx).

## Charts

| Chart | Description |
|-------|-------------|
| demo-backend | FastAPI backend with PostgreSQL |
| demo-frontend | React frontend served by nginx |

## Publishing

Charts are published as OCI artifacts to GHCR on version tags (`v*`):

- `oci://ghcr.io/recmanj/charts/demo-backend`
- `oci://ghcr.io/recmanj/charts/demo-frontend`

## Usage

```bash
helm install my-backend oci://ghcr.io/recmanj/charts/demo-backend --version 0.1.0
helm install my-frontend oci://ghcr.io/recmanj/charts/demo-frontend --version 0.1.0
```

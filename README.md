# Demo Charts

Helm charts for demo-backend (FastAPI) and demo-frontend (React/nginx).

## Charts

| Chart | Description |
|-------|-------------|
| demo-backend | FastAPI backend with PostgreSQL |
| demo-frontend | React frontend served by nginx |

## Publishing

Charts are published to GitHub Pages via [chart-releaser-action](https://github.com/helm/chart-releaser-action) on push to main when a chart's `version` in `Chart.yaml` changes.

## Usage

```bash
helm repo add demo-charts https://recmanj.github.io/demo-charts
helm repo update
helm install my-backend demo-charts/demo-backend --version 0.1.0
helm install my-frontend demo-charts/demo-frontend --version 0.1.0
```

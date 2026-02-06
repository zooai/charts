# Zoo Charts

Helm charts for Zoo AI research infrastructure.

## Charts

| Chart | Description |
|-------|-------------|
| inference | AI inference service |
| training | ML training jobs |
| jupyter | JupyterHub deployment |
| mlflow | MLflow tracking server |

## Usage

```bash
helm repo add zooai https://zooai.github.io/charts/
helm repo update
helm install my-inference zooai/inference
```

## Development

```bash
# Lint charts
ct lint --all

# Test charts
ct install --all
```

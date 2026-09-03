# Zoo Charts

Helm charts for Zoo infrastructure.

## The node

Zoo's L1 runs the same node build as every other Lux network, so it deploys
from the shared chart rather than a copy kept here:

```bash
helm install zoo oci://ghcr.io/luxfi/charts/node \
  -f https://raw.githubusercontent.com/luxfi/charts/main/charts/node/values-zoo.yaml
```

`values-zoo.yaml` sets the only thing that differs — the network id, 200200,
which for a sovereign L1 is also its EVM id. The exact image is pinned by
digest there; environment-specific values live in `zoo/universe`.

## Charts here

None yet. Charts belong here when they deploy something Zoo builds and no
other network runs.

## Usage

```bash
helm repo add zooai https://zooai.github.io/charts/
helm repo update
```

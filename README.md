# kustomize

## Structure
```
├── base
│   ├── service.yaml
│   ├── deployment.yaml
│   ├── kustomization.yaml
└── overlays
    └── development
       ├── kustomization.yaml
        └── cpu_count.yaml
        └── replica_count.yaml
    └── production
        ├── kustomization.yaml
        └── cpu_count.yaml
        └── replica_count.yaml

```
## build
```sh
kustomize build overlay/dev/
```

## apply kubernetes
```sh
kustomize build overlay/dev/ | kubectl apply -f -
```

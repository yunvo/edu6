# kustomize

## Structure
```
├── base
│   ├── service.yaml
│   ├── deployment.yaml
│   ├── ingress.yaml
│   ├── kustomization.yaml
└── overlays
    └── dev
        ├── configmap.yaml
        ├── kustomization.yaml
        └── secret.yaml
```
## build
```sh
kustomize build overlay/dev/
```

## apply kubernetes
```sh
kustomize build overlay/dev/ | kubectl apply -f -
```

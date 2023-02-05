
# The Basics
```

kubectl apply -f kubernetes/kustomize/base/namespace.yaml
kubectl apply -f kubernetes/kustomize/base/configmap.yaml
kubectl apply -f kubernetes/kustomize/base/deployment.yaml
kubectl apply -f kubernetes/kustomize/base/service.yaml

# OR 

kubectl apply -f kubernetes/kustomize/base/

kubectl delete ns example

```

# Kustomize

## Build
```
kubectl kustomize .\kubernetes\kustomize\ | kubectl apply -f -
# OR
kubectl apply -k .\kubernetes\kustomize\

kubectl delete ns example
```

## Overlays

```
kubectl kustomize .\kubernetes\kustomize\environments\overlays | kubectl apply -f -
# OR
kubectl apply -k .\kubernetes\kustomize\environments\overlays

kubectl delete ns example
```




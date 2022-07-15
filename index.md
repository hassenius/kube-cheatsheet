## Kubernetes cheat sheet

Simple website to keep a cheat sheet of Kubernetes stuff

### Configmap stuff

- Nifty ways to manage configmaps and rekicking pods when configmaps are updated, using Kustomize

### Kubernetes service discovery

```yaml
apiVersion: v1
kind: Service
metadata:
  name: mygoogle
  namespace: default
spec:
  type: ExternalName
  externalName: google.ie
```
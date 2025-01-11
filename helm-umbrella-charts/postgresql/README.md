# Get first postgres pass

```sh
kubectl get secret -n postgresql postgresql -o jsonpath="{.data.postgres-password}" | base64 -d
```
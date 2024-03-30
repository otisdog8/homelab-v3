

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: harbor-secret
type: Opaque
stringData:
  HARBOR_ADMIN_PASSWORD: ""
  REGISTRY_PASSWD: ""
```
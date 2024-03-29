use the command, but put the output in templates

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: auth-generic-oauth-secret
type: Opaque
stringData:
  client_id: ""
  client_secret: ""
```
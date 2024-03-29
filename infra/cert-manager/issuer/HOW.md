Put the token and use this command
` kubeseal -f cloudflared-tunnel-credentials.secret.yaml -w cloudflared-tunnel-credentials.yaml`

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: cloudflare-api-token-secret
  namespace: cert-manager
type: Opaque
stringData:
  api-token: YOURAPITOKEN
```

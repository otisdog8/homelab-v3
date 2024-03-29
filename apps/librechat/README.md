Put the token and use this command
` kubeseal -f cloudflared-tunnel-credentials.secret.yaml -w cloudflared-tunnel-credentials.yaml --scope cluster-wide`

```yaml
apiVersion: v1
kind: Secret
metadata:
  name: librechat-secret
type: Opaque
stringData:
  OPENID_CLIENT_ID: ""
  OPENID_CLIENT_SECRET: ""
  OPENID_SESSION_SECRET: ""
  CREDS_KEY: ""
  CREDS_IV: ""
  JWT_SECRET: ""
  JWT_REFRESH_SECRET: ""
```

Generate a 50-character secret key, you might not need to set password and stuff in postgres I think it autogenerates.

Use the standard kubeseal command  `kubeseal -f cloudflared-tunnel-credentials.secret.yaml -w cloudflared-tunnel-credentials.yaml`

You need to set the postgres password when you first create the database

```yaml
apiVersion: v1
kind: Secret
type: Opaque
metadata:
  name: authentik-secret
stringData:
  AUTHENTIK_SECRET_KEY: ""
  POSTGRES_PASSWORD: ""
```
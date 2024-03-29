Put the token and use this command
` kubeseal -f cloudflared-tunnel-credentials.secret.yaml -w cloudflared-tunnel-credentials.yaml`

`kubectl create secret generic cloudflared-tunnel-credentials \                               
--from-file=credentials.json=~/file.json  --dry-run=client -o yaml > infra/cloudflared/cloudflared-tunnel-credentials.secret.yaml`

```yaml
apiVersion: v1
data:
  credentials.json: YOURJWTTOKEN
kind: Secret
metadata:
  creationTimestamp: null
  name: cloudflared-tunnel-credentials
  namespace: cloudflared
```

## References 
- https://github.com/aquasecurity/kube-hunter

### Need to set schedule time to run kube-hunter in ivari-sandbox-values.yaml
```yaml
image:
  registry: aquasec
  repository: kube-hunter
  tag: 0.6.8
  pullPolicy: IfNotPresent

imagePullSecrets: []
nameOverride: ""
fullnameOverride: ""

schedule: "*/5 * * * *"  # run at every 5 minuits
```

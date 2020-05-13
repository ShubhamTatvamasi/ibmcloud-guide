# ibmcloud-guide

get list on workers in a cluster
```bash
ibmcloud ks worker ls --cluster $(ibmcloud ks cluster ls --json | jq -r '.[0].id')
```

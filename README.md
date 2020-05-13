# ibmcloud-guide

get list on workers in a cluster
```bash
ibmcloud ks worker ls --cluster $(ibmcloud ks cluster ls --json | jq -r '.[0].name')
```

delete a cluster
```bash
ibmcloud ks cluster rm --cluster $(ibmcloud ks cluster ls --json | jq -r '.[0].name') -f
```


update ibmcloud cli
```bash
ibmcloud update
```


# ibmcloud-guide

get list on workers in a cluster
```bash
ibm_cluster=$(ibmcloud ks cluster ls --json) \
  ibmcloud ks worker ls --cluster $(echo ${ibm_cluster} | jq -r '.[0].name')
```

delete a cluster
```bash
ibm_cluster=$(ibmcloud ks cluster ls --json) \
  ibmcloud ks cluster rm --cluster $(echo ${ibm_cluster} | jq -r '.[0].name') -f
```

create a new cluster
```bash
ibmcloud ks cluster create classic --name cka
```

update ibmcloud cli
```bash
ibmcloud update
```


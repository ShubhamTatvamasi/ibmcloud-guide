# ibmcloud-guide


create a new cluster
```bash
ibmcloud ks cluster create classic --name cka
```

list clusters
```bash
ibmcloud ks cluster ls
```

get list on workers in a cluster
```bash
ibmcloud ks worker ls --cluster cka
```

get cluster state
```bash
ibmcloud ks cluster get --cluster cka
```

config cluster
```bash
ibmcloud ks cluster config --cluster cka
```

delete cluster
```bash
ibmcloud ks cluster rm --cluster cka -f
```

update ibmcloud cli
```bash
ibmcloud update
```

update your region to "India Chennai"
```bash
ibmcloud target -r in-che
```
> Just run `ibmcloud target` if you want to get current target.

List all locations:
```bash
ibmcloud ks locations
```

Check kubernetes versions on IBM Cloud:
```bash
ibmcloud ks versions
```

save cluster info in a variable
```bash
ibm_cluster=$(ibmcloud ks cluster ls --json)
ibm_cluster_name=$(echo ${ibm_cluster} | jq -r '.[0].name')
```
---

### plugins

Install kubernetes plugin:
```bash
ibmcloud plugin install container-service
```


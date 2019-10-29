# sensor-things-hackathon-19
PDOK - Geonovum SensorThings API Hackathon 2019 

Create a local cluster (using kind) and deploy all resources needed to run GOST 
on a local k8s cluster: 

```bash
docker-compose -f docker-compose.yml up
```

Config kubectl to connect to the local k8s cluster:

```bash
export INTEGRATIONTEST=`pwd`
export KUBECONFIG=$INTEGRATIONTEST/kubectl-config
curl http://localhost:10080/config > $KUBECONFIG
```

Schema to setup your GOST database can be found here:
https://github.com/gost/gost-db/blob/master/gost_init_db.sql
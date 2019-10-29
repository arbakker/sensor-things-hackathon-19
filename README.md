# sensor-things-hackathon-19
PDOK - Geonovum SensorThings API Hackathon 2019 

Create a local cluster (using kind) and deploy all resources to it which are needed to test the dkk-download applications: `docker-compose -f docker-compose.yml up`

```bash
export INTEGRATIONTEST=`pwd`
export KUBECONFIG=$INTEGRATIONTEST/kubectl-config
curl http://localhost:10080/config > $KUBECONFIG
```
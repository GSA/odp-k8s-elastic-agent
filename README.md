# odp-k8s-elastic-agent
Provides manifest to deploy elastic-agent on kubernetes

## How to deploy?
1. Clone this repo

2. Update the following values in the daemon-set.yaml file
    - `FLEET_URL` - URL of the remote Fleet server
    - `FLEET_ENROLLMENT_TOKEN` - API Token for the agent to entroll with the Fleet server

3. deploy using the following `kubectl` command from within the repo folder

```
kubectl apply -f .

```
4. Contact ELP admin to check if the agent with the specific API token has enrolled into the Fleet server

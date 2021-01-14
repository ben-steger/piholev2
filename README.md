# piholev2

1. `sudo microk8s apply -f 00-namespace.yaml`
2. `sudo microk8s apply -f 01-pihole-pvc.yaml`
3. `sudo microk8s apply -f 02-configmaps.yaml`
4. Change value of WEBPASSWORD in `03-deployment.yaml`
5. `sudo microk8s apply -f 03-deployment.yaml`
6. `sudo microk8s apply -f 04-service.yaml` (One service for the web UI, one for DNS.)

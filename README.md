kubectl apply -f keydb-deployment.yaml
kubectl apply -f keydb-service.yaml

kubectl exec -it <pod-name> -- /bin/sh
apt update
apt install redis-tools

SET k1 "v1"
GET k1
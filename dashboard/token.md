kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0-beta8/aio/deploy/recommended.yaml

kubectl apply -f dashboard-adminuser.yaml

kubectl apply -f clusterrolebinding.yaml

kubectl proxy

kubectl -n kubernetes-dashboard create token admin-user

http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/

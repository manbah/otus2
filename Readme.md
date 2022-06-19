**Otus 2 Home work**

**Run instruction**
1) To create postgres instance
run
   <code>helm install postgres ./postgres --set volumePermissions.enabled=true</code>

2) To create app instance run <code>helm install otus2-app ./otus2-app</code>

3) To use arch.homework as domain we need enable ingress controller. To enable run 
   <code>kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.2.0/deploy/static/provider/cloud/deploy.yaml </code>

4) To redirect to api run <code>kubectl apply -f ingress.yaml</code>

```
kubectl run pod1 --image nginx --dry-run=client -o yaml

kubectl api-resources
kubectl explain pods --recursive
kubectl explain pod.spec.affinity.podAffinity
kubectl explain pod.spec.affinity.nodeAffinity
kubectl explain pod.spec.containers.imagePullPolicy
kubectl apply -f pod.yml
kubectl logs hello-cat


# Running commands in Pods
kubectl apply -f https://raw.githubusercontent.com/nachikethmurthy/kubernetes-administrator-certification/main/1.pods/pod.yml
kubectl exec hello-cat -- ls 
kubectl exec hello-cat -- cat app.py
kubectl exec -it hello-cat -- python # start python inside the pod
kubectl get pods --show-labels

```
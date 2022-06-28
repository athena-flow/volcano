```shell
make images

helm install . --namespace volcano-trial --name volcano-trial
kubectl get pod -n volcano-trial

helm list  

helm delete --purge volcano-trial

kubectl delete crd commands.bus.volcano.sh
kubectl delete crd jobs.batch.volcano.sh
kubectl delete crd queues.scheduling.incubator.k8s.io
kubectl delete crd podgroups.scheduling.incubator.k8s.io
```
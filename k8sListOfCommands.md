# List Of Kubernetes Most Useful Commands

## 1. Pods
```
$ kubectl get pods
$ kubectl get pods — all-namespaces
$ kubectl get pod monkey -o wide
$ kubectl get pod monkey -o yaml
$ kubectl describe pod monkey
```

## 2. Create Deployments
Create single deployment:
`$ kubectl run monkey — image=monkey — record`

## 3. Scaling PODs
$ kubectl scale deployment/POD_NAME — replicas=N

##4. POD Upgrade and history
List history of deployments:
`$ kubectl rollout history deployment/DEPLOYMENT_NAME`

Jump to specific revision:
`$ kubectl rollout undo deployment/DEPLOYMENT_NAME — to-revision=N`

## 5. Services
List services:
`$ kubectl get services`

Expose PODs as services (creates endpoints)
`$ kubectl expose deployment/monkey — port=2001 — type=NodePort`

## 6. Volumes
List Persistent Volumes and Persistent Volumes Claims:
```
$ kubectl get pv
$ kubectl get pvc
```

## 7. Secrets
List Persistent Volumes and Persistent Volumes Claims:
```
$ kubectl get secrets
$ kubectl create secret generic — help
$ kubectl create secret generic mysql — from-literal=password=root
$ kubectl get secrets mysql -o yaml
```

## 8. ConfigMaps
List Persistent Volumes and Persistent Volumes Claims:
```
$ kubectl create configmap foobar — from-file=config.js
$ kubectl get configmap foobar -o yaml
```

## 10. Troubleshooting
```
$ kubectl describe
$ kubectl logs
$ kubectl exec
$ kubectl get nodes — show-labels
$ kubectl get events
```

 

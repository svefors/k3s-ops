Bindings created with:
```
kubectl create clusterrolebinding strimzi-cluster-operator-namespaced --clusterrole=strimzi-cluster-operator-namespaced --serviceaccount strimzi:strimzi-cluster-operator --dry-run-o yaml > binding-operator-namespaced.yaml

kubectl create clusterrolebinding strimzi-cluster-operator-entity-operator-delegation --clusterrole=strimzi-entity-operator --serviceaccount strimzi:strimzi-cluster-operator --dry-run=client -o yaml > binding-entity-operator.yaml

kubectl create clusterrolebinding strimzi-cluster-operator-topic-operator-delegation --clusterrole=strimzi-topic-operator --serviceaccount strimzi:strimzi-cluster-operator --dry-run=client -o yaml > binding-topic-operator.yaml
```

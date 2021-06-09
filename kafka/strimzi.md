kubectl create namespace ingestion
helm install kafka strimzi/strimzi-kafka-operator --namespace ingestion --version 0.21.0
kubectl apply -f ~/projects/bitbucket/minikube/2-repository/yamls/ingestion/broker/kafka-ephemeral.yaml -n ingestion

kubectl delete -f ~/projects/bitbucket/minikube/2-repository/yamls/ingestion/broker/kafka-ephemeral.yaml -n ingestion
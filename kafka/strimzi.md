kubectl create namespace ingestion
helm install kafka strimzi/strimzi-kafka-operator --namespace ingestion --version 0.21.0

# Strimzi
kubectl apply -f ~/projects/github/command-warehouse/kafka/kafka-ephemeral-single.yaml -n ingestion
kubectl delete -f ~/projects/github/command-warehouse/kafka/kafka-ephemeral-single.yaml -n ingestion
# OWS
kubectl apply -f ~/projects/bitbucket/minikube/2-repository/yamls/ingestion/broker/kafka-ephemeral.yaml -n ingestion
kubectl delete -f ~/projects/bitbucket/minikube/2-repository/yamls/ingestion/broker/kafka-ephemeral.yaml -n ingestion

# Create Topic
kubectl apply -f ~/projects/github/command-warehouse/kafka/py-kafka-skin-json.yaml -n ingestion
kubectl delete -f ~/projects/github/command-warehouse/kafka/py-kafka-skin-json.yaml -n ingestion
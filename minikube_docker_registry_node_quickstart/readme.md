Yaml recipes for the **failed part**/initial try of the Hands-on-kubernetes Playground

https://costica.dev/posts/hands-on-kubernetes-playground/

kubectl apply -f registry/deployment.yaml
kubectl apply -f registry/service.yaml

minikube -p PROFILE_NAME service docker-registry-service --url 

build Docker image & push it it to the exposed registry (mind the registry URL) // "great" UX! 

reference the repository in the node-quickstart/deployment recipe 

kubectl apply -f node-quickstart/deployment.yaml
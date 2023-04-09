[Node-quickstart](https://github.com/costicaaa/node-quickstart/tree/v2.0-dev_and_prod_ready_quickstart)
"What now?" part of the Kubernetes playground article https://costica.dev/posts/hands-on-kubernetes-playground/

1. Build the image (`node-quickstart` folder): `docker build -t node-quickstart .`
2. Start a brand-new cluster: `minikube -p easy-mode start`
3. Load the image: `minikube image load node-quickstart:latest`
4. Start the deployment of the container: `kubectl apply -f deployment.yaml`
5. Start the service: `kubectl apply -f service.yaml`
6. Expose the service to the outside world: `minikube -p easy-mode service node-quickstart-service --url`
7. Copy and paste the `url` returned by the previous command. `Hello world` is returned by the server.

# SEIP Assignment, Kyriaki Krimitza (8230066)

## Repository
GitHub: https://github.com/kyriakikrimitza/seip_assignment_1_2026

## Start Minikube
minikube start

## Apply Kubernetes files
kubectl apply -f k8s/

## Check cluster
kubectl get all
kubectl get configmap,secret

## Port forward
kubectl port-forward service/echo-api-service 8080:80

## Open in browser
http://localhost:8080
http://localhost:8080/secure-config

## AI Usage and Future Outlook

During this assignment, I used Generative AI tools, mainly ChatGPT, to guide the implementation of the Dockerfile, GitHub Actions workflow, Kubernetes manifests, and troubleshooting process.

The most useful parts of the AI assistance were understanding the correct structure of Kubernetes manifests, fixing YAML placement issues, explaining ConfigMaps and Secrets, generating Base64 values correctly, and debugging setup problems with Docker, Minikube, and kubectl.

Some friction points appeared during local setup, especially with Windows PATH configuration, Docker Desktop engine startup, WSL updates, and Minikube image downloads. These issues required manual troubleshooting through terminal outputs, restarting services, updating WSL, and re-running failed commands.

If I had more time, I would improve the system by replacing port-forwarding with an Ingress Controller, adding       Prometheus and Grafana monitoring, using ArgoCD for GitOps-based deployments, adding vulnerability scanning in the CI/CD pipeline, and introducing Helm charts for better deployment management.
# Ubuntu 24.04.3 Server Full-Stack & DevOps + UI Management Roadmap

This file shows which topics should be placed in which folders and under which filenames according to the project folder structure.

---

## 1. Basic Server and Linux Knowledge

📂 `01-Basics-Linux-Server/en/` and `01-Basics-Linux-Server/tr/`

- `ubuntu-commands.md` → Ubuntu basic commands
- `package-management.md` → Package management (APT)
- `netplan-static-ip.md` → Netplan static IP configuration
- `ufw-firewall.md` → UFW firewall management
- `ssh-remote.md` → Remote access via SSH
- `system-monitoring.md` → System resource monitoring

---

## 2. Development Environment Setup

📂 `02-Dev-Environment/en/` and `02-Dev-Environment/tr/`

- `git-setup.md` → Git installation and SSH key generation
- `vscode-remote-ssh.md` → VSCode Remote-SSH usage
- `dotnet-sdk-install.md` → .NET SDK installation
- `dotnet-basic-api.md` → Creating a basic .NET API

---

## 3. Docker Basics

📂 `03-Docker/en/` and `03-Docker/tr/`

- `docker-install.md` → Docker installation
- `docker-cli.md` → Docker CLI commands
- `dockerfile.md` → Creating a Dockerfile
- `docker-volumes-networks.md` → Volume and network concepts
- `docker-hub.md` → Docker Hub usage
- `docker-compose.md` → Multi-container setup with docker-compose

---

## 4. Database Systems (Containerized)

📂 `04-Databases/en/` and `04-Databases/tr/`

- `mssql.md` → MSSQL Server
- `postgresql.md` → PostgreSQL
- `mysql-mariadb.md` → MySQL / MariaDB
- `mongodb.md` → MongoDB
- `redis.md` → Redis
- `rabbitmq.md` → RabbitMQ
- `kafka.md` → Kafka

---

## 5. .NET + Database Integration

📂 `05-DotNet-Database-Integration/en/` and `05-DotNet-Database-Integration/tr/`

- `efcore-mssql.md` → EF Core with MSSQL
- `efcore-postgresql.md` → EF Core with PostgreSQL
- `mongodb-driver.md` → MongoDB driver usage
- `redis-cache.md` → Redis caching
- `rabbitmq-integration.md` → RabbitMQ integration

---

## 6. Kubernetes Basics

📂 `06-Kubernetes-Basics/en/` and `06-Kubernetes-Basics/tr/`

- `minikube-k3s-install.md` → Installing Minikube or K3s
- `kubectl-commands.md` → kubectl commands
- `deployment.md` → Deployment structure
- `service-types.md` → Types of services
- `configmap-secret.md` → Using ConfigMap and Secret
- `persistent-volume.md` → Persistent Volume and PVC
- `nodeport-access.md` → Access via NodePort
- `ingress-controller.md` → Ingress Controller installation

---

## 7. Kubernetes + .NET Applications

📂 `07-Kubernetes-DotNet-Apps/en/` and `07-Kubernetes-DotNet-Apps/tr/`

- `dotnet-deployment.md` → Kubernetes Deployment file for .NET app
- `statefulset-db.md` → StatefulSet for databases
- `secret-connection.md` → Managing connection strings with Secrets
- `hpa.md` → Horizontal Pod Autoscaler
- `rolling-update-rollback.md` → Rolling Update and Rollback

---

## 8. CI/CD Processes

📂 `08-CICD/en/` and `08-CICD/tr/`

- `github-actions.md` → GitHub Actions for automatic build
- `docker-registry-push.md` → Docker registry push
- `k8s-auto-deploy.md` → Automatic deployment to Kubernetes
- `semantic-versioning.md` → Semantic Versioning (SemVer)

---

## 9. Monitoring and Logging

📂 `09-Monitoring-Logging/en/` and `09-Monitoring-Logging/tr/`

- `prometheus-install.md` → Installing Prometheus
- `grafana-install.md` → Installing Grafana
- `loki-elk.md` → Installing Loki or ELK Stack
- `alertmanager.md` → Alertmanager setup

---

## 10. Advanced Tools and Services

📂 `10-Advanced-Tools/en/` and `10-Advanced-Tools/tr/`

- `nginx-reverse-proxy.md` → Nginx Reverse Proxy
- `traefik-ingress.md` → Traefik Ingress Controller
- `vault.md` → HashiCorp Vault
- `consul.md` → Consul service discovery
- `argocd-gitops.md` → ArgoCD GitOps
- `service-mesh.md` → Istio or Linkerd Service Mesh

---

## 11. Extra Lab Experiments

📂 `11-Extra-Labs/en/` and `11-Extra-Labs/tr/`

- `redis-sentinel.md` → Redis Sentinel
- `kafka-event-driven.md` → Event-driven architecture with Kafka
- `rabbitmq-microservices.md` → Microservices communication with RabbitMQ
- `minio.md` → MinIO object storage
- `keycloak.md` → Keycloak authentication
- `sonarqube.md` → SonarQube code analysis
- `load-testing.md` → Load testing with K6 or JMeter

---

## 12. Security and Optimization

📂 `12-Security-Optimization/en/` and `12-Security-Optimization/tr/`

- `ufw.md` → UFW firewall configuration
- `fail2ban.md` → Fail2Ban brute force prevention
- `ssl-letsencrypt.md` → SSL certificates with Let's Encrypt
- `docker-image-optimization.md` → Optimizing Docker images
- `k8s-rbac.md` → Kubernetes RBAC authorization
- `db-optimization.md` → Database optimization

---

## 13. UI Management Layer

📂 `13-UI-Management/en/` and `13-UI-Management/tr/`

- `portainer.md` → Portainer CE
- `rancher.md` → Rancher
- `lazydocker.md` → LazyDocker
- `pgadmin.md` → pgAdmin
- `ssms.md` → SQL Server Management Studio (SSMS)
- `adminer.md` → Adminer
- `mongo-express.md` → Mongo Express
- `lens.md` → Lens
- `k8s-dashboard.md` → Kubernetes Dashboard
- `octant.md` → Octant
- `grafana-ui.md` → Grafana
- `kibana-ui.md` → Kibana
- `loki-ui.md` → Loki UI
- `prometheus-ui.md` → Prometheus UI
- `jenkins.md` → Jenkins
- `gitlab-ci-cd.md` → GitLab CI/CD
- `argocd-ui.md` → ArgoCD UI
- `nginx-proxy-manager.md` → Nginx Proxy Manager
- `minio-console.md` → MinIO Console
- `filebrowser.md` → Filebrowser
- `nextcloud.md` → Nextcloud

---

## 14. Final Goal

📂 `14-Final-Goal/en/` and `14-Final-Goal/tr/`

- `final-architecture.md` → Achieving full UI-based management of infrastructure, databases, and applications
- `full-integration.md` → Fully integrated monitoring, logging, domain, SSL, and CI/CD processes with web-based control

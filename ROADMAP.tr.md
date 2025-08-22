# Ubuntu 22.04.5 Sunucu Üzerinde Full-Stack & DevOps + UI Yönetim Yol Haritası

Bu dosya, proje klasör yapısına göre hangi konuların hangi klasörlerde ve hangi dosya isimleri ile tutulacağını gösterir.

---

## 1. Temel Sunucu ve Linux Bilgisi

📂 `01-Basics-Linux-Server/en/` ve `01-Basics-Linux-Server/tr/`

- `ubuntu-commands.md` → Ubuntu temel komutları
- `package-management.md` → Paket yönetimi (APT)
- `netplan-static-ip.md` → Netplan ile sabit IP ayarı
- `ufw-firewall.md` → UFW firewall yönetimi
- `ssh-remote.md` → SSH ile uzaktan bağlanma
- `system-monitoring.md` → Sistem kaynak takibi

---

## 2. Geliştirme Ortamı Hazırlığı

📂 `02-Dev-Environment/en/` ve `02-Dev-Environment/tr/`

- `git-setup.md` → Git kurulumu ve SSH key oluşturma
- `vscode-remote-ssh.md` → VSCode Remote-SSH kullanımı
- `dotnet-sdk-install.md` → .NET SDK kurulumu
- `dotnet-basic-api.md` → Basit .NET API oluşturma

---

## 3. Docker Temelleri

📂 `03-Docker/en/` ve `03-Docker/tr/`

- `docker-install.md` → Docker kurulumu
- `docker-cli.md` → Docker CLI komutları
- `dockerfile.md` → Dockerfile oluşturma
- `docker-volumes-networks.md` → Volume ve network mantığı
- `docker-hub.md` → Docker Hub kullanımı
- `docker-compose.md` → docker-compose ile çoklu container

---

## 4. Veritabanı Sistemleri (Container)

📂 `04-Databases/en/` ve `04-Databases/tr/`

- `mssql.md` → MSSQL Server
- `postgresql.md` → PostgreSQL
- `mysql-mariadb.md` → MySQL / MariaDB
- `mongodb.md` → MongoDB
- `redis.md` → Redis
- `rabbitmq.md` → RabbitMQ
- `kafka.md` → Kafka

---

## 5. .NET + Veritabanı Entegrasyonu

📂 `05-DotNet-Database-Integration/en/` ve `05-DotNet-Database-Integration/tr/`

- `efcore-mssql.md` → EF Core ile MSSQL bağlantısı
- `efcore-postgresql.md` → EF Core ile PostgreSQL bağlantısı
- `mongodb-driver.md` → MongoDB driver kullanımı
- `redis-cache.md` → Redis cache kullanımı
- `rabbitmq-integration.md` → RabbitMQ ile mesajlaşma

---

## 6. Kubernetes Temelleri

📂 `06-Kubernetes-Basics/en/` ve `06-Kubernetes-Basics/tr/`

- `minikube-k3s-install.md` → Minikube veya K3s kurulumu
- `kubectl-commands.md` → kubectl komutları
- `deployment.md` → Deployment yapısı
- `service-types.md` → Service türleri
- `configmap-secret.md` → ConfigMap ve Secret kullanımı
- `persistent-volume.md` → Persistent Volume ve PVC
- `nodeport-access.md` → NodePort ile erişim
- `ingress-controller.md` → Ingress Controller kurulumu

---

## 7. Kubernetes + .NET Uygulaması

📂 `07-Kubernetes-DotNet-Apps/en/` ve `07-Kubernetes-DotNet-Apps/tr/`

- `dotnet-deployment.md` → Kubernetes Deployment dosyası
- `statefulset-db.md` → Veritabanı için StatefulSet
- `secret-connection.md` → Secret ile connection string yönetimi
- `hpa.md` → Horizontal Pod Autoscaler
- `rolling-update-rollback.md` → Rolling Update ve Rollback

---

## 8. CI/CD Süreçleri

📂 `08-CICD/en/` ve `08-CICD/tr/`

- `github-actions.md` → GitHub Actions ile otomatik build
- `docker-registry-push.md` → Docker registry push işlemi
- `k8s-auto-deploy.md` → Kubernetes’e otomatik deploy
- `semantic-versioning.md` → Versiyonlama (SemVer)

---

## 9. İzleme ve Loglama

📂 `09-Monitoring-Logging/en/` ve `09-Monitoring-Logging/tr/`

- `prometheus-install.md` → Prometheus kurulumu
- `grafana-install.md` → Grafana kurulumu
- `loki-elk.md` → Loki veya ELK Stack kurulumu
- `alertmanager.md` → Alertmanager ile uyarı sistemi

---

## 10. İleri Servisler ve Araçlar

📂 `10-Advanced-Tools/en/` ve `10-Advanced-Tools/tr/`

- `nginx-reverse-proxy.md` → Nginx Reverse Proxy
- `traefik-ingress.md` → Traefik Ingress Controller
- `vault.md` → HashiCorp Vault
- `consul.md` → Consul servis keşfi
- `argocd-gitops.md` → ArgoCD GitOps
- `service-mesh.md` → Istio veya Linkerd Service Mesh

---

## 11. Ekstra Deneme Alanları

📂 `11-Extra-Labs/en/` ve `11-Extra-Labs/tr/`

- `redis-sentinel.md` → Redis Sentinel
- `kafka-event-driven.md` → Kafka ile event-driven mimari
- `rabbitmq-microservices.md` → RabbitMQ ile mikroservis iletişimi
- `minio.md` → MinIO obje depolama
- `keycloak.md` → Keycloak kimlik doğrulama
- `sonarqube.md` → SonarQube kod analizi
- `load-testing.md` → K6 veya JMeter yük testi

---

## 12. Güvenlik ve Optimizasyon

📂 `12-Security-Optimization/en/` ve `12-Security-Optimization/tr/`

- `ufw.md` → UFW ile port güvenliği
- `fail2ban.md` → Fail2Ban brute force engelleme
- `ssl-letsencrypt.md` → SSL sertifikası (Let's Encrypt)
- `docker-image-optimization.md` → Docker image optimizasyonu
- `k8s-rbac.md` → Kubernetes RBAC yetkilendirme
- `db-optimization.md` → Veritabanı optimizasyonu

---

## 13. UI ile Yönetim Katmanı

📂 `13-UI-Management/en/` ve `13-UI-Management/tr/`

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

## 14. Nihai Hedef

📂 `14-Final-Goal/en/` ve `14-Final-Goal/tr/`

- `final-architecture.md` → Tüm altyapı, veritabanı ve uygulamaları UI üzerinden yönetebilir hale gelme
- `full-integration.md` → Tam entegre izleme, loglama, domain, SSL ve CI/CD süreçlerini web arayüzünden kontrol

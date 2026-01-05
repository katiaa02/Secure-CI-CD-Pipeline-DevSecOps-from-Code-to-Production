# Secure-CI-CD-Pipeline-DevSecOps-from-Code-to-Production

🔹 CI/CD

GitHub Actions

Pipeline en plusieurs stages

Gates de sécurité (fail si vulnérabilité critique)

🔹 Sécurité intégrée (clé du projet)
🧪 1. SAST – Analyse du code

Semgrep ou SonarCloud

Détection :

SQL Injection

Hardcoded secrets

Mauvaises pratiques

📦 2. SCA – Dépendances

OWASP Dependency-Check ou Snyk

Rapports CVE générés automatiquement

🔐 3. Secret Scanning

Gitleaks

Pipeline bloquée si clé AWS / token détecté

🐳 4. Sécurité des conteneurs

Docker

Trivy

Scan des images avant déploiement

☁️ 5. Infrastructure as Code sécurisée

Terraform

Checkov

Détection :

Buckets publics

Ports ouverts

Mauvaise config cloud

🔹 Déploiement

Kubernetes (kind ou minikube)

Déploiement automatique après validation sécurité

Manifests sécurisés :

Non-root container

Resource limits

Read-only filesystem

🔹 Monitoring & Security

Prometheus + Grafana

Falco (détection d’activités suspectes)

Alertes en cas d’événement critique

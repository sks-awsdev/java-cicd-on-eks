| Path                              | Purpose                                                                |
| --------------------------------- | ---------------------------------------------------------------------- |
| `jenkins/Jenkinsfile`             | Your CI/CD logic using Jenkins (build, test, sonar, docker build/push) |
| `sonar/sonar-project.properties`  | Required for SonarQube scan (project key, source dir etc.)             |
| `docker/Dockerfile`               | Build image for your Java application                                  |
| `k8s/`                            | Kubernetes manifests used by ArgoCD to deploy the app                  |
| `cloudformation/eks-cluster.yaml` | Provision EKS cluster (can be replaced with Terraform later)           |
| `src/`                            | Java source code (your app)                                            |
| `pom.xml`                         | Defines dependencies and build steps for Maven                         |
| `.gitignore`                      | Ignore IDE, target folders, etc.                                       |
| `README.md`                       | Project overview, instructions (write later)                           |

# sonarqube-kubernetes
Kubernetes sonarqube setup

# Once sonar server is set

Configure CI/CD 

```
- name: gcr.io/$PROJECT_ID/sonar-scanner:latest
  args:
    - '-Dsonar.host.url=https://sonar.ingress.url'
    - '-Dsonar.login=SONAR-PASSWORD'
    - '-Dsonar.projectKey=test-service'
    - '-Dsonar.sources=.'
```

here example step for GCP cloudbuild.yaml this will push details to sonar server

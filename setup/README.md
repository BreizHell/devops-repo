# Maybe necessary commands

- `docker compose exec -u root -it jenkins sh`
  - mkdir -p --mode=755 /var/jenkins_home/.m2/repository
  - chown -R jenkins:jenkins /var/jenkins_home/.m2/repository

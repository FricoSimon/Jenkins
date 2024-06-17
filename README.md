# Jenkins

Everything about [Jenkins!](https://jenkins.io/)

## Installation ([Downloads](https://www.jenkins.io/download/))

### Windows

1. Create a user (local)
2. Give access to logon as a service
3. Find a default password
4. Setup Jenkins (user, password, plugins)
5. Done

### Docker

1. Docker pull Jenkins/jenkins:latest
2. Run Docker container

   ```
   docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 --restart=on-failure jenkins/jenkins:latest
   ```

3. Get the initial password

   ```
   docker exec -it <container_id> cat /var/jenkins_home/secrets/initialAdminPassword
   ```

4. Open Jenkins in browser

   ```
   http://localhost:8080
   ```

5. Install suggested plugins
6. Done

## Use

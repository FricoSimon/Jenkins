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

1. Pull Docker image

   ```
   docker pull jenkins/jenkins:latest
   ```

2. Run Docker container

   ```
   docker run -d -v jenkins_home:/var/jenkins_home -p <YOUR_PORT>:8080 -p 50000:50000 --restart=on-failure jenkins/jenkins:latest
   ```

3. Get the initial password

   ```
   docker exec -it <CONTAINER_ID> cat /var/jenkins_home/secrets/initialAdminPassword
   ```

   or

   ```
   docker logs <CONTAINER_ID>
   ```

4. Open Jenkins in browser

   ```
   http://localhost:8080
   ```

5. Install suggested plugins
6. Done

## Use

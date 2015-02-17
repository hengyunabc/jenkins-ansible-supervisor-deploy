# jenkins-ansible-supervisor-deploy
Use jenkins, ansible, supervisor to deploy java application.

http://hengyunabc.github.io/deploy-system-build-with-jenkins-ansible-supervisor/

This playbook do these things:
- install python-pip, supervisor
- install jdk
- download tomcat and config
- tomcat control by supervisor
- deploy war to remote host
- wait for tomcat started

## Docker image showcase

```bash
docker run -it -p 8080:8080 -p 8101:8101 -p 9001:9001 --name='jenkins' hengyunabc/jenkins-ansible-supervisor
```

- jenkins: 
  [http://localhost:8080/](http://localhost:8080/)
- spring-mvc-showcase: 
  [http://localhost:8101/](http://localhost:8101/)
- supervisor: 
  [http://localhost:9001/](http://localhost:9001/)     admin/admin

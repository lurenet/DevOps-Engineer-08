Follow this simple instruction

1. Clone this project
  git clone https://github.com/lurenet/dve-08.git

2. Add to /etc/ansible/hosts two groups of nodes
  - build
  - prod

  Group "build" will be used to build docker image and push it to docker hub.
  Group "prod" will be used to download image and run container

3. Set up your authentification data for docker hub to config/dockerhub.yml

4. Run this playbook
  ansible-playbook tomcat.yml

5. Run this URL:
  http://IP_Prod_Group_Server/hello-1.0/

6. Get a result.
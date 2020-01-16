 1 - presentation de openshift 
 2 - connection web openshift and presentation interface
 3 - connection cli 
 4.1 - presentation pipeline devops
 4.2 - presentation example 
 5 - build docker
    docker build -t myapp-web-app .
 6 - push docker openshift 
    docker login docker.io
    docker tag myapp-web-app:latest zhamdaoui/myapp-web-app:v1
    docker push zhamdaoui/myapp-web-app:v1
 7 - create pod 
    oc apply -f pod.yaml
 8 - create service 
 9 - create route 
 10 - create deployment config
 11 - Rolling Back a Deployment
    oc rollout undo dc/myapp-dc
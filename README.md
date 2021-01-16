# Docker and Kubernetes Containers Demo Codes

## Docker Demo Codes

`INFO`
> docker run hello-world
<br> docker -v
<br> <br> nginx
<br> nginx -version

`DEMO`
> docker ps
<br> docker ps -a
<br> docker image ls
<br> docker rm ***(your_container_id)***
<br> docker image ls
<br> docker rmi ***(your_image-id)***
<br> docker run —-name myNginxServer -d -P nginx
<br> docker run —-name myNginxServer2 -d -P nginx
<br> docker run —-name myDocuments -v ***(your_path)***:/usr/share/nginx/html:ro -P -d nginx
<br> docker rm ***(your_container_id)*** -f
<br> docker kill ***(your_container_id)***

`FOR CREATE A HTML FILE`
> cd ***(your_path)***
<br> ls -la
<br> touch index.html
<br> nano index.html
<br> cat index.html

## Kurbernetes Demo Codes

`INFO`
> kubectl version

`DEMO`
> kubectl create deployment my-depl -—image=gcr.io/google_containers/echoserver:1.4 —-port=8080
<br> kubectl port-forward ***(pod_name)*** 8080:8080
<br> kubectl scale deployment.apps/my-depl —-replicas=2
<br> kubectl expose deployment my-depl —-type=NodePort
<br> <br> kubectl get deployments
<br> kubectl delete deployment my-depl
<br> kubectl get services
<br> kubectl delete service my-depl
<br> kubectl get pods
<br> kubectl delete pod ***(pod_name)***
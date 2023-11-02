# To create a docker image we have to make Dockerfile 
<br>
and build it using following command<br>

```sudo docker build -t anirudhabidave/kube-assignment```.<br>
# To push the image on docker hub first we have to login 
<br>
`sudo docker login`<br>

and put your username and password of docker hub<br>

# To push the image the command is

`sudo docker push anirudhabidave/kube-assignment`<br>

## To deploy the java app on kubernetes we have two ways<br>

###  By creating pod.yaml file and service.yaml file<br>

#### To create a pod <br>

`kubectl create -f mypod.yaml`<br>

#### To create a sirvice.yaml file <br>

`kubectl create -f service-definition.yaml`<br>

#### To get the link to access the web app<br>

`minikube service myapp-service --url`

### By creating deployment.yaml and service.yaml files

#### To create a deployment.yaml file

`kubectl create -f deployment.yaml`<br>

#### Then Create a service .

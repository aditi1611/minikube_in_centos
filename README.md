$ yum install docker -y

$ yum install socat -y

$ systemctl enable docker --now

$ curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

$ chmod +x ./kubectl

$ mv ./kubectl /usr/local/bin/kubectl

$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 && chmod +x minikube

$ install minikube /usr/local/bin

$ minikube start --vm-driver=none
 
to check --

$ kubectl get pods -n kube-system
-- you will get pods and all should be running!!!

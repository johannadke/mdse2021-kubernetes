# Download

`sudo apt install curl`
`curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64`
`sudo install minikube-linux-amd64 /usr/local/bin/minikube`

# minikube setup (wird nochmals gezeigt)

`minikube config set driver docker`
`sudo usermod -aG docker <user> && newgrp docker`
`minikube start`
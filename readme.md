# MDSE 2021 - Gruppe Kubernetes
17.12.2021

- Theorie:
  -   Johanna Deike     4940972
  -   Lisa Reß          3798263
  -   Nora Klemp        7979965
- Praxis:
  -   Aidan Zimmer      4803747
  -   Luca Chmielarski  3047210

---

<br>

## 1. Installation (Ubuntu)

```
sudo apt install curl
```

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
```

```
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

<br>

## 2. Minikube Setup

```
minikube config set driver docker
```
```
sudo usermod -aG docker $USER && newgrp docker
```
```
minikube start
```

<br>

## 3. Minikube + Kubectl Basic Commands

- Minikube Status anzeigen:

```
minikube status
```

- Bestimmte k8s-Komponente im Minikube anzeigen (ohne Klammern angeben!):

```
kubectl get (nodes/deployments/pods...)

kubectl get deployments     # z.B. alle Deployments anzeigen
```

- Deployments erstellen:

```
kubectl create deployment Name --image=image
```

- Bestimmte k8s-Komponente löschen:

```
kubectl delete (nodes/deployments/pods...)
```

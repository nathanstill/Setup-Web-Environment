# Setup-Web-Environment
1. Install Docker Desktop
2. Install Go
3. Install minikube (note - stop KIND first in Docker)
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
sudo install minikube-darwin-arm64 /usr/local/bin/minikube
minikube start
```
4. Check kubectl is working:
```
sudo kubectl get all --all-namespaces
```
5. Setup Wordpress in Kubernetes (some troubleshooting required):
```
https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume/
```

# Committing all files changed
```
cd ~
cd git
cd [name of repo - press tab to list]
git add .
git commit -m "My commit details here"
git push
```
# Cloning a repository
```
git clone [repo URL here]
```
# Creating a git folder
```
cd ~
mkdir git
cd git
```

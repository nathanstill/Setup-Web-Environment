# Setup-Web-Environment
1. Install Docker Desktop
2. Install Go
3. Install KIND
```
git clone https://github.com/kubernetes-sigs/kind.git
sudo apt install make
cd kind
make install
sudo ./bin/kind create cluster
```
4. Check KIND is working:
```
sudo kubectl get all --all-namespaces
```
5. Setup Wordpress in Kubernetes (some troubleshooting required):
```
https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume/
```

# Committing all files changed
```
cd git
cd [name of repo - press tab to list]
git add .
git commit -m "My commit details here"
git push

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

# Setup-Web-Environment
1. Install Docker Desktop
2. Install Go
3. Install KIND
```
git clone https://github.com/kubernetes-sigs/kind.git
sudo apt install make
cd kind
make install
sudo /home/ubuntu/go/bin/kind create cluster
```
4. Check KIND is working:
```
kubectl get all --all-namespaces
```
5. Setup Wordpress in Kubernetes (some troubleshooting required):
```
https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume/
```

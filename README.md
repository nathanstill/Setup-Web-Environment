# Adding a Custom Plugin
https://makitweb.com/how-to-create-simple-wordpress-plugin/

# Getting Visual Studio Code Setup

1. Press command+shift+p in Visual studio code.
2. Type 'shell install' and choose:
```
Install 'code' command in PATH
```
3. From the terminal, navigate to your www folder using the 'cd' (change directory) command and your Caveots page.
4. Join the assignment: https://classroom.github.com/a/3E9N1PfG
5. Create a new repository in this www folder.
```
git init
git add .
git commit -m "Initial Commit"
git remote add origin "[link to your wordpress repo created above]"
git push
```
Note: if there are suggested commands after the first git push command, run these.

# Setup-Web-Environment
1. Install apache, mysql and PHP
```
brew install apache2 mysql php
```
2. Create the httpd.conf configuration changes
```
nano /opt/homebrew/etc/httpd/httpd.conf
```

```
LoadModule php_module /opt/homebrew/opt/php/lib/httpd/modules/libphp.so

    <FilesMatch \.php$>
        SetHandler application/x-httpd-php
    </FilesMatch>
```
3. Restart apache
4. Download Wordpress and put in www folder
5. Delete the index.html file
6. Create the wordpress database
```
mysql -u root
```

```
CREATE DATABASE wpdb DEFAULT CHARACTER SET utf8 COLLATE utf8_unicode_ci;
```

#Old Instructions
1. Install Docker Desktop
2. Install Go
3. Install minikube (note - stop KIND first in Docker)

For Apple M1 (new lab computers)
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-arm64
sudo install minikube-darwin-arm64 /usr/local/bin/minikube
minikube start
```
For Intel only (older lab computers and some of your laptops):
```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64
sudo install minikube-darwin-amd64 /usr/local/bin/minikube
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

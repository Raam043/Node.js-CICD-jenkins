# Node.js-CICD-jenkins 

1. Release 2 instances
   1 for Jenkins
   1 for Node.js Application

2. Connect ssh to install jenkins with node js package

```sh
wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
yum upgrade
amazon-linux-extras install java-openjdk11 -y
yum install jenkins -y
systemctl enable jenkins
systemctl start jenkins
yum install git -y
```

Enable nodejs packages on Linux server
Install development tools.
Install nodejs
```sh
curl -sL https://rpm.nodesource.com/setup_15.x | bash -
yum groupinstall 'Development Tools'
yum -y install nodejs
```

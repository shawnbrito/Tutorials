## Instructions For Installing Tomcat 9

### Log into your Linux VM (Ubuntu / CentOS / Fedora)
#### Download Tomcat 9 for Linux from the internet  (google the tomcat 9 for linux)

- $workshop> wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.111/bin/apache-tomcat-9.0.111.tar.gz
- $workshop> wget https://download.oracle.com/java/17/archive/jdk-17.0.12_linux-x64_bin.tar.gz
- $workshop> tar xzf apache-tomcat-9.0.111.tar.gz

- $workshop> sudo mv apache-tomcat-9.0.111  /opt/tomcat
- $workshop> mv jdk-17.0.12  jdk
- $workshop> whoami    
- $workshop> sudo chown -R centos:centos  /opt/tomcat
- $workshop> sudo chmod –R  775  /opt/tomcat

## Edit the Startup Script
- $> sudo vi  /etc/systemd/system/tomcat.service

## Setup the Startup Service Files...
- $> sudo systemctl daemon-reload
- $> sudo systemctl restart tomcat.service
- $> sudo systemctl stop tomcat.service
- $> sudo systemctl start tomcat.service

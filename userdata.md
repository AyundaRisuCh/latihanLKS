#!/bin/bash
sudo yum -y update
sudo yum install httpd -y
sudo yum install php php-mysqli php-unzip php-xml php-common
sudo systemctl enable httpd
sudo systemctl start httpd
sudo yum install git unzip composer
sudo yum -y install ruby
sudo yum -y install wget
cd /home/ec2-user
wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto
sudo yum install -y python-pip
sudo pip install awscli

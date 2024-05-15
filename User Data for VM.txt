#!/bin/bash
sudo apt-get update
sudo apt-get -y install ruby
sudo apt-get install wget
cd /home/ubuntu
wget https://aws-codedeploy-us-east-2.s3.us-east-2.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto
sudo service codedeploy-agent start
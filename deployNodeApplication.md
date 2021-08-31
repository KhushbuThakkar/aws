# login to node using ssh

sudo apt update
sudo curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo yes | apt install nodejs
sudo apt install ruby-full
sudo apt install wget
cd /home/ubuntu

# codedeploy

wget https://aws-codedeploy-ap-south-1.s3.ap-south-1.amazonaws.com/latest/install
chmod +x ./install
sudo ./install auto > /tmp/logfile
sudo service codedeploy-agent status
sudo service codedeploy-agent start
sudo service codedeploy-agent status

#yarn 

sudo apt-get update && sudo apt-get install yarn

#caddy
apt update -y && apt upgrade -y
echo "deb [trusted=yes] https://apt.fury.io/caddy/ /" | sud

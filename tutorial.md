# Create EC2 instance
- Ubuntu 22.04 LTS
- t2.xlarge (4CPUs, 16GB)
- Ensure the security group expose port 5001 (or another port you want the service being reached on)

# Install Git
```
sudo apt-get update
sudo apt-get install git tree
```

# Install Docker and Docker Compose
```
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
apt-cache policy docker-ce
sudo apt install docker-ce
sudo systemctl status docker

# Adding docker-compose-plugin
sudo apt install python3-pip
pip install --upgrade pip
sudo pip install docker-compose
```
# Clone repo and checkout in the right branch 
```
git clone your_repo_url
git fetch --all
git checkout branchname
```

# Launch app with docker-compose
```
sudo docker-compose build
sudo docker-compose up -d
```





















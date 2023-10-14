# new-assignment
STEP 1
-create ubuntu server/Linux server on AWS cloud
STEP 2 
-- connect to MobaXtreme
-- update the server
$sudo apt-get update(ubuntu server)
$sudo yum update -y (linux server)
STEP 4  
--install jenkins in ubuntu server
  
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
    /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
# For linux server
--install jenkins in linux server
   sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
   sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key

    yum install fontconfig java-11-openjdk
    yum install jenkins



install git,docker.io,docker-compose

===============================
With Public IP and port 8080 open in new window broser 

In security group we have to enable port number 8080 and 8000 also for docker container

SET JENKINS USERNAME AND PASSWORD
Go to configure and add git url to fetch the code.
add plugin for Docker

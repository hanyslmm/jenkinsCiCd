# jenkinsCiCd

# Install Jenkins on Ubuntu steps:

1- Step 1 - Update existing packages
*sudo apt-get update

2- Step 2 - Install Java
*sudo apt install -y default-jdk

3- Download Jenkins package. 
* You can go to http://pkg.jenkins.io/debian/ to see the available commands
* First, add a key to your system
wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -

4- Add the following entry in your /etc/apt/sources.list:
* sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'

5- Update your local package index
* sudo apt-get update

6- Install Jenkins
* sudo apt-get install -y jenkins

7- Start the Jenkins server
* sudo systemctl start jenkins

8- Enable the service to load during boot
* sudo systemctl enable jenkins
* sudo systemctl status jenkins

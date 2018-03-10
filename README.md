# aws-ubuntu-jenkins

sudo apt-get install openjdk-8-jdk

wget -q -O — https://pkg.jenkins.io/debian/jenkins-ci.org.key | sudo apt-key add -

echo deb https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list

sudo apt-get update

sudo apt-get install jenkins -y

sudo systemctl start jenkins

sudo systemctl status jenkins

---

포트변경
sudo vi /etc/default/jenkins
HTTP_PORT=9999

# how to install docker on debian 12


* sudo apt remove docker docker-engine docker.io containerd runc
* sudo apt install apt-transport-https  ca-certificates  curl gnupg-agent software-properties-common iptables
* sudo update-alternatives --set iptables /usr/sbin/iptables-legacy
* /sbin/iptables --version
* curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
* sudo apt-key fingerprint 0EBFCD88
* sudo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/debian \
   $(lsb_release -cs) \
   stable"
* sudo apt update
* sudo apt install docker-ce docker-ce-cli containerd.io
* sudo service docker start
* sudo docker ps -a
* sudo docker run --rm hello-world

# how to install composer without errors

* composer install --ignore-platform-reqs

# Recusos do Windows: 

- Subsistema Windows para Linux
- Plataforma Máquina Virtual
  
# WslRegisterDistribution failed with error: 0x800701bc Error: 0x800701bc WSL 2 requer uma atualizaþÒo para seu componente kernel. Para obter mais informaþ§es, visite ...

resolve: install this https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi

# how to install docker on debian 12

* sudo apt-get update && upgrade
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
* sudo usermod -aG docker $USER
* newgrp docker
* groups $USER
* docker ps -a
* docker run --rm hello-world

# how to install docker on debian 12
  * sudo apt update && sudo apt upgrade -y
  * sudo apt install -y curl jq
  * sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
  * sudo chmod +x /usr/local/bin/docker-compose
  * docker-compose --version

# how to install composer without errors
* composer install --ignore-platform-reqs

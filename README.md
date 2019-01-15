# roger-skyline1

copy your ssh key to the server using : ssh-copy-id username@ip

Connect into ssh to root user then copy past :

echo -e "deb http://deb.debian.org/debian stretch main\ndeb-src http://deb.debian.org/debian stretch main\n\ndeb http://deb.debian.org/debian-security/ stretch/updates main\ndeb-src http://deb.debian.org/debian-security/ stretch/updates main\n\ndeb http://deb.debian.org/debian stretch-updates main\ndeb-src http://deb.debian.org/debian stretch-updates main" > /etc/apt/sources.list && apt-get update -y && apt-get upgrade -y && apt-get -y install sudo vim iptables-persistent fail2ban git nginx sendmail && git clone https://github.com/C1em/roger-skyline1.git /script

then run /script/deployment from the VM

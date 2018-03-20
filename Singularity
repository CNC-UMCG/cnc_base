Bootstrap: docker
From: ubuntu:latest

%environment
SINGULARITY_SHELL="/bin/bash"

%post
apt-get update
apt-get install -y wget

# add neurodebian repository
wget -O- http://neuro.debian.net/lists/xenial.de-md.libre | tee /etc/apt/sources.list.d/neurodebian.sources.list
apt-key adv --recv-keys --keyserver hkp://pool.sks-keyservers.net:80 0xA5D32F012649A5A9

# add irods icommands 
wget -qO - https://packages.irods.org/irods-signing-key.asc | apt-key add -
echo "deb [arch=amd64] https://packages.irods.org/apt/ $(lsb_release -sc) main" | tee /etc/apt/sources.list.d/renci-irods.list


apt-get update


# add datalad
apt-get install -y datalad

# install dependencies (cmake)
apt-get install -y cmake pkg-config

# install dcm2niix
apt-get install -y dcm2niix

# install icommands
apt-get install -y irods-icommands

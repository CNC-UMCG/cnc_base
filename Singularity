Bootstrap: docker
From: ubuntu:latest

%post

# add neurodebian repository

wget -O- http://neuro.debian.net/lists/xenial.de-md.libre | tee /etc/apt/sources.list.d/neurodebian.sources.list
apt-key adv --recv-keys --keyserver hkp://pool.sks-keyservers.net:80 0xA5D32F012649A5A9
apt-get update


# add datalad
apt-get -y install datalad

# install dependencies (cmake)
apt-get -y install cmake pkg-config

# install dcm2niix
apt-get -y install dcm2niix

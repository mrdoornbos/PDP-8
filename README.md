# PDP-8 

sudo apt update
sudo apt upgrade -y
sudo apt install build-essential libraspberrypi-dev \
     libncurses-dev perl python3-pip tcl neovim -y
pip3 install pexpect pyyaml

sudo ln -s /usr/sbin/udevadm /sbin/udevadm

cd ~/pidp8i
./configure && tools/mmake && sudo make install


make reconfig


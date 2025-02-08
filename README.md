# devstack-ironic
    $ sudo apt update
    $ sudo apt upgrade -y
    $ sudo apt-get update
    $ sudo apt-get upgrade -y
    $ sudo useradd -s /bin/bash -d /opt/stack -m stack
    $ sudo chmod +x /opt/stack
    $ echo "stack ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/stack
    $ sudo su - stack #
    $ sudo apt install git -y
    $ git clone https://opendev.org/openstack/devstack
    $ git clone https://github.com/svashu/devstack-ironic.git
    $ cp devstack-ironic/localrc devstack
    $ cd devstack
    $ sudo apt install -y vim
    $ sudo vim localrc
    
# Modify HOST_IP, PASSWORD
    $ ./stack.sh

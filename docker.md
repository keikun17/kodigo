# Docker

Login to central repo

    $ sudo docker login

Pull image

    $ docker pull <Name>
    // ex. docker pull centos

Commit container to a named image

    // sudo docker commit <container_id> <username>/<imagename>
    $ sudo docker commit $CONTAINER_ID keikun17/appname

Push

    // sudo docker commit <username>/<imagename>
    $ sudo docker push keikun17/appname

# boot2docker

install on OSX (follow instructions on [their github page](https://github.com/boot2docker/boot2docker)).

    $ brew update
    $ brew install boot2docker

Start VM and boot2docker dotfile things:

    $ boot2docker init

Start the VM

    $ boot2docker up

SSH into vm (username : docker, password : tcuser)

    $ boot2docker ssh

# Customization

You can customise the values of VM_NAME, DOCKER_PORT, SSH_HOST_PORT, VM_DISK, VM_DISK_SIZE, VM_MEM and BOOT2DOCKER_ISO by setting them in $HOME/.boot2docker/profile

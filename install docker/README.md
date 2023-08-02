Running this playbook will perform the following actions on your Ansible hosts:

    Install aptitude, which is preferred by Ansible as an alternative to the apt package manager.
    Install the required system packages.
    Install the Docker GPG APT key.
    Add the official Docker repository to the apt sources.
    Install Docker.
    Install the Python Docker module via pip.
    Pull the default image specified by default_container_image from Docker Hub.
    Create the number of containers defined by the container_count variable, each using the image defined by default_container_image, and execute the command defined in default_container_command in each new container.

Once the playbook has finished running, you will have a number of containers created based on the options you defined within your configuration variables.

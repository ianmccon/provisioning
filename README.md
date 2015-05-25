This project is designed to provision a vagrant box and install nginx web server
with a default web page

This project does not implement all the provisioning steps that I would normally make
I would normall copy ssh keys to the server for the deploy user and disable ssh password login
and disable root login

## Usage

1. Clone this repo on your local machine
2. Run `vagrant up`

3. Open 192.168.0.99 in your web browser to load the default web page.


## Testing

To run a syntax check and list the tasks that will be run type the following command
from the root of the project

    ansible-playbook --syntax-check --list-tasks -i tests/hosts ./provision.yml

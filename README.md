# Multi-Machine Vagrant with ansible

This project contains a simple app, which relies on a database and is an example of provisioning using Vagrant and Ansible.

To run:

- Clone this repo.
- In the root directory run `vagrant up`. This will provision two VMs, one for the app itself and one for the DB.
- To enter the app, run `vagrant ssh app`. This will put you into the app VM.
- Install npm by running `sudo npm install npm -g`
- Start the app with `DB_HOST=mongodb://192.168.10.150:27017/posts node app.js`
- Open development.local:3000 in your browser to view the home page. To view the posts, go to development.local:3000/posts

# Setting up Development Environment (using Vagrant)

To simplify contribution there is a [Vagrant box](https://vagrantcloud.com/redash/boxes/dev) available with all the needed software to run Redash for development (use it only for development).

To get started with this box:

1. Make sure you have recent version of [Vagrant](https://www.vagrantup.com/) installed.
2. Clone the Redash repository: `git clone https://github.com/getredash/redash.git`.
3. Change dir into the repository (`cd redash`)
4. To execute tests, run `./bin/vagrant_ctl.sh test`
5. To run the app, run `./bin/vagrant_ctl.sh start`. This might take some time the first time you run it, as it downloads the Vagrant virtual box. Now the server should be available on your host on port 9001 and you can login with username admin and password admin.

# Infrared tripleo inventory plugin

In order to use this plugin with infrared, the following command should be executed:

    infrared plugin add https://github.com/rhos-infra/tripleo-inventory.git --src-path infrared_inventory_plugin

## Usage example

Create new infrared workspace:

    infrared workspace checkout --create my_workspace

Run the plugin on your environment:

    infrared tripleo-inventory --host <HOST_NAME> --ssh-key /my/.ssh/id_rsa/path

Check Infrared commands work:

    infrared ssh controller-0 "whoami"

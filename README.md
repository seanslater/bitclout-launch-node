# deso-launch-node

Quick and dirty installation script to start a new DeSo node using Ubuntu - feedback, improvements, comments welcome.

Copy/paste the following commands to download the script, allow it to execute, then run it. The script will install Docker and download the DeSo installation packages.

The Nano text editor will open to edit dev.env - you can add your DeSo public key to ADMIN_PUBLIC_KEYS to lock admin access to your account and hide it from visitors to the node (or just leave it blank allowing open admin viewing access), Ctrl-X to close Nano and save/exit).

Tada!

Once installation has completed the server needs to be rebooted (to allow the open file limits to be refreshed).

Once rebooted, after a couple of minutes the node will start automatically. The node will then start to sync the blockchain - this will take a bit of time to complete. You can now open the IP address assigned to your server in your web browser and you should have a working read-only DeSo node online! Enjoy!

# Usage

sudo wget https://raw.githubusercontent.com/seanslater/deso-launch-node/main/deso-node.sh

sudo chmod 777 ./deso-node.sh

sudo ./deso-node.sh

sudo reboot

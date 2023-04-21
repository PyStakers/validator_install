# validator_install
Ethereum Validator - Automated Installation

# Summary
This script automates the installation and setup of an Ethereum validator node with Geth and Lighthouse. It performs the following tasks:

1) Prompts user to select Ethereum Network
2) Promtpts user for Ethereum address for validator tips. (optional)
3) Allows the user to set Checkpoint Sync. (optional)
4) Installs and configures Universal Firewall (ufw).
5) Creates necessary users, directories, and files.
6) Downloads and installs the latest Geth and Lighthouse binaries.
7) Sets up and writes service files for Geth, Lighthouse Beacon, and Lighthouse Validator.
8) Displays the final setup information, including firewall status and software versions.

To run the script, use these commands:

git clone https://github.com/PyStakers/validator_install.git

sudo pip install requests

python3 /validator_install/validator_install.py

# validator_install
Ethereum Validator - Automated Installation

# Summary
This script automates the installation and setup of an Ethereum validator node with Geth and Lighthouse. It performs the following tasks:
Prompts user to select Ethereum Network
Promtpts user for Ethereum address for validator tips. (optional)
Allows the user to set Checkpoint Sync. (optional)
Installs and configures Universal Firewall (ufw).
Creates necessary users, directories, and files.
Downloads and installs the latest Geth and Lighthouse binaries.
Sets up and writes service files for Geth, Lighthouse Beacon, and Lighthouse Validator.
Displays the final setup information, including firewall status and software versions.

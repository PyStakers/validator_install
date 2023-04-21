# validator_install
Ethereum Validator - Automated Installation and Confinguration

1 click, 1 minute, Ethereum Validator running Geth & Lighthouse

# Summary
This script automates the installation and setup of an Ethereum validator node using Geth and Lighthouse.

I used [Somer Esat's - Lighthouse/Geth](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-lighthouse-773f5d982e03) as a guide and created a single Python script to automate the entire setup and configuration.

Important Note: This script does not handle generating validator keys, keystores, mnemonics, or any security related items. It simply prepares the computer for staking by installing the binaries, creating users, writing service files etc. 

After the 1 minute installation, Execution (Geth) and Consensus (Lighthouse) clients are properly configured and can begin syncing.

If you want to run a full validator, you'll also need to generate a mnemonic and keystores to run the validator. Please refer to [Somer's guide](https://someresat.medium.com/guide-to-staking-on-ethereum-ubuntu-lighthouse-773f5d982e03) or this [Ubuntu - Key Generation Guide](https://app.gitbook.com/s/-MMPsvIEM2fJY_8ygWws/) to learn more.

# Validator Install Script
The `validator_install.py` script performs the following tasks:

1) Prompts user to select Ethereum Network (mainnet / testnet)
2) Prompts user for Ethereum address for validator tips. (optional)
3) Prompts user to set Checkpoint Sync. (optional)
4) Installs and configures Universal Firewall (ufw).
5) Creates necessary users, directories, and files.
6) Downloads and installs the latest Geth and Lighthouse binaries.
7) Sets up and writes service files for Geth, Lighthouse Beacon, and Lighthouse Validator.
8) Displays the final setup information, including firewall status and installed software versions.

**To run the script, use these commands:**

`sudo apt-get update`

`sudo apt-get install git`

`git clone https://github.com/PyStakers/validator_install.git`

`sudo pip install requests`

`python3 validator_install/validator_install.py`


**Disclaimer:** This script is for testing purposes only. Do not use it on mainnet Validators. Test using a VM or bootable USB.

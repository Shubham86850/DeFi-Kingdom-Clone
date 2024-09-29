# A Simple DeFI Kingdom Clone

## Description

This project is a basic replica of a blockchain-based game. Players can collect, build, and battle with their digital assets on a custom EVM subnet on Avalanche.

## Getting Started

### Executing Program

To run this project, follow these steps:

1. Download and install [Oracle VM VirtualBox](https://www.virtualbox.org/). Configure it as needed.
2. Download a Microsoft Windows Subsystem for Linux (WSL) distribution like [Ubuntu](https://ubuntu.com/desktop/wsl) or [Parrot](https://parrotsec.org/download/). Install and set it up on VirtualBox.
3. After opening WSL, launch its terminal and install Avalanche-CLI. [Refer to the official documentation for installation instructions](https://docs.avax.network/tooling/cli-guides/install-avalanche-cli).
4. With Avalanche CLI installed, create a new subnet by running the command `avalanche subnet create mySubnet` in your terminal. This will set up a subnet named "mySubnet" on your local machine. Here I have named the Subnet as "Shubham".
5. During the subnet creation, you will need to select a subnet type. Choose the SubnetEVM option to create an EVM Subnet on your local machine, then proceed to step 6.
6. Run `avalanche subnet create Shubham` <br>
   Attempted to check if a new version is available, but couldn't find the currently running version information <br>
   Ensure to follow official instructions, or automatic updates won't be available for you <br>
   ✔ Subnet-EVM <br>
   creating subnet Shubham <br>
   Enter your subnet's ChainId. It can be any positive integer. <br>
   ChainId: 5678 <br>
   Select a symbol for your subnet's native token <br>
   Token symbol: SHUBHAM <br>
   ✔ Use latest version <br>
   ✔ Low disk use / Low Throughput 1.5 mil gas/s (C-Chain's setting) <br>
   ✔ Airdrop 1 million tokens to the default address (do not use in production) <br>
   ✔ No <br>
7. After selecting the EVM Subnet option, deploy the subnet by running `avalanche subnet deploy Shubham` and choose to deploy on your local network. This will set up your new EVM Subnet.
8. Once deployed, the console will display all details regarding the subnet you just created.
9. Set up a local network in your wallet using the subnet details.
10. Navigate to [Remix IDE](https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.26+commit.8a97fa7a.js) and create two files named `ERC20.sol` and `vault.sol`. Copy and paste the code.
11. Compile both contracts under the Compiler tab.
12. Connect Remix to your MetaMask wallet using Injected Provider.
13. First, deploy the `ERC20.sol` contract, then copy its address to deploy the `vault.sol` contract.
14. After deploying the contracts, you can interact with them by calling their functions through the Remix interface.
15. You can mint tokens, approve transactions made by the vault contract, and perform deposit and withdrawal actions using the vault contract.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Authors

Shubham  
[@Shubham](sksingh94166@gmail.com)

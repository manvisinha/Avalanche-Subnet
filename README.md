# Cherry Token and Vault

## Overview

This project implements a basic ERC-20 token named Cherry (CHY) with additional functionalities such as minting, burning, and a Vault contract for handling deposits and withdrawals.

## Contracts

### ERC20

The ERC20 token handles actions like sending tokens, giving permission for spending, and managing the creation and removal of tokens. Additionally, it provides information about the total supply, individual balances, and allowed transactions.

#### Functions

- `transfer`: Transfer tokens from the sender to a recipient.
- `approve`: Approve another address to spend tokens on behalf of the sender.
- `transferFrom`: Transfer tokens from one address to another using the approved spender.
- `mint`: Make new tokens, adding to the total amount available.
- `burn`: Remove tokens from circulation, reducing the total amount available.

### IERC20 Interface

The IERC20 Interface lists the actions and events required for the ERC-20 standard. The ERC20 contract follows and carries out these guidelines.

### Vault

The Vault contract simplifies the safe deposit and withdrawal of tokens. Users deposit tokens into the Vault, getting shares in exchange. Later, these shares can be traded back for the initially deposited tokens.

#### Functions

- `deposit`: Deposit tokens into the Vault and receive shares in proportion to the total supply.
- `withdraw`: Withdraw tokens from the Vault by redeeming a specified number of shares.

## Subnet

A subnet refers to a subset or partition of the overall network that operates semi-independently. Subnets allow for the customization of parameters, consensus mechanisms, and virtual machines within a specific subset of the blockchain network.

Key characteristics of subnets include:

- **Tailoring to Specific Needs**: Each subnet has the flexibility to establish unique rules, validators, and virtual machines, making it suitable for specific uses or applications.
- **Consensus Mechanism:** Subnets can use different consensus mechanisms, providing flexibility in how transactions are confirmed.
- **Interoperability:** Subnets can interact with each other, enabling seamless movement of assets and data between different parts of the network.
- **Security Isolation:** Subnets provide security isolation, containing potential issues or attacks within a specific subnet.
- **Scalability:** Subnets contribute to the overall scalability of the network by handling a larger number of transactions concurrently.

## Getting Started

1. Clone the repository: `git clone [repository_url]`
2. Install dependencies: `npm install`
3. Deploy the contracts and subnets on your preferred Ethereum or Avalanche development network.

## Example Usage

1. Deploy the ERC20 contract with the desired parameters.
2. Deploy the Vault contract, specifying the ERC20 token's address.
3. Interact with the contracts and subnets using the provided functions.

## Author

 Manvi Sinha
 [@sinhamanvi17@gmail.com]

## License

This project is licensed under the MIT License.

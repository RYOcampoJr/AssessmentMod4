# Smart Contract Management
## Project: Function Frontend

This project demonstrates a simple smart contract and a React frontend for interacting with it. The smart contract allows the owner to deposit, withdraw, wipe, and double the balance. 

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract allows an account owner to deposit and withdraw funds, wipe the balance, and double the balance, while ensuring that only the owner can perform these actions. Events are emitted for each operation to provide transparency and traceability.

## Getting Started

Follow the instructions below to get the project running on your local machine.

### Installation

1. Clone the repository to your local machine:
    ```bash
    git clone <repository-url>
    ```

2. Navigate to the project directory:
    ```bash
    cd <project-directory>
    ```

3. Install the project dependencies:
    ```bash
    npm install
    ```

### Running the Project

1. Open two additional terminals in your VS Code, so you have a total of three terminals open.

2. In the second terminal, start a local Ethereum network using Hardhat:
    ```bash
    npx hardhat node
    ```

3. In the third terminal, deploy the smart contract to the local network:
    ```bash
    npx hardhat run --network localhost scripts/deploy.js
    ```

4. Back in the first terminal, start the React frontend:
    ```bash
    npm run dev
    ```

### Accessing the Project

Once everything is set up and running, you can access the project in your web browser at:

http://localhost:3000/


### Smart Contract

The smart contract includes the following functions:
- **`getBalance()`**: Returns the current balance.
- **`deposit(uint256 _amount)`**: Allows the owner to deposit a specified amount.
- **`withdraw(uint256 _withdrawAmount)`**: Allows the owner to withdraw a specified amount.
- **`wipeBalance()`**: Resets the balance to zero.
- **`doubleBalance()`**: Doubles the current balance.

### Frontend

The React frontend provides a simple interface for interacting with the smart contract. You can connect your MetaMask wallet, view your account balance, and perform the following actions:
- Deposit 1 ETH
- Withdraw 1 ETH
- Wipe Balance
- Double Balance

### Forked From
[MetacrafterChris/SCM-Starter](https://github.com/MetacrafterChris/SCM-Starter)

### Author
Adrian Oraya

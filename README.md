# Particle Testnet Bot

This repository contains a Node.js application that automates transactions on the Ethereum testnet (Ropsten) using multiple private keys.

## Requirements

- Node.js
- npm (Node Package Manager)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/dante4rt/particle-testnet-bot.git
   cd particle-testnet-bot
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Define the RPC URL:**

   Create a file named `rpc.txt` in the root directory of the project and paste your Ethereum RPC URL (e.g., `https://eth-sepolia.g.alchemy.com/v2/xxxx`) into it. This URL specifies the Ethereum network endpoint to connect to.

4. **Prepare private keys:**

   - Create or edit `privateKeys.json` to include your Ethereum private keys as an array of strings. Each private key should be enclosed in double quotes.

   **Example `privateKeys.json` (correct format):**
   ```json
   [
       "private_key_1_here",
       "private_key_2_here"
   ]
   ```

   Ensure each private key string is correctly formatted as shown above.

## Usage

- **Run the application:**

  ```bash
  node index.js
  ```

- Follow the prompts to enter the number of transactions to send per private key.
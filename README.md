# Centic Bot Network

This repository contains a Centic bot network tool utilizing Node.js. The tool can perform automated tasks such as auto check-in, creating wallets, and buffing referrals with both proxy and non-proxy support.

🌐 [Centic Quests Link](https://centic.io/quests/daily?refferalCode=eJwNxskRACAIBLCWOERmywHcHixf84pcxDibMohKNujGtMJPaxJrhzZPPghYDA8=)

## Features

- 🌐 Auto task completion
- 🌐 Auto check-in
- 🌐 Auto create wallets and buff referrals
- 🌐 Multi-threading support
- 🌐 Auto Claim Quest
- 🌐 Auto Claim Daily Reward
- 🌐 Support multiple accounts
- 🌐 Support Proxy usage

## Requirements

- Node.js

## Instructions

Follow these steps to set up and run the Centic bot network tool:

1. **Install dependencies**:

   ```bash
   npm install
   ```

2. **Configure environment**:

   - Reconfigure the `.env` file according to your needs.

3. **Prepare necessary files**:

   - Save the private key of your EVM wallet in `privateKeys.txt` (format: 0x...).
   - Save the `apiKey` in `tokens.txt`. You can manually get the `apiKey` from the web (application => storage => apiKey) or the tool will automatically retrieve it using the private key.
   - Save proxies in `proxy.txt` in the format: `proxy: http://user:pass@ip:port`.

4. **Buff referrals**:

   - To buff referrals for the main account, run the following command:

     ```bash
     node autoRef
     ```

   - Detailed information of the created wallets will be saved in `wallets.json` (you should save this file). The `privateKeys.txt` file will automatically update with the private keys of the new wallets.

5. **Get wallet address**:

   - Run the following command to get the wallet address through the private key:

     ```bash
     node setup
     ```

   - The wallet address will be saved in `wallets.txt`.

6. **Run the tool**:

   - Run the main tool with the following command:

     ```bash
     node main
     ```

   - Alternatively, you can run the tool with proxy support:

     ```bash
     node main-proxy
     ```

## Centic Auto Claim Tasks

This script automates claim tasks to earn the Centic Points (CTP).

## Additional Features

- 🌐 Auto Claim Quest
- 🌐 Auto Claim Daily Reward
- 🌐 Support multiple accounts
- 🌐 Support Proxy usage

## Prerequisites

- Node.js installed on your machine.
- `tokens.txt` file containing token `apiKey` from Centic platform. Follow the instructions below to get it:
  1. Open the Centic platform: [Centic Quests](https://centic.io/quests/daily?refferalCode=eJwNxskRACAIBLCWOERmywHcHixf84pcxDibMohKNujGtMJPaxJrhzZPPghYDA8=)
  2. Login with your wallet.
  3. Inspect or press `F12`, and find Application.
  4. In local storage, find `apiKey_` and copy all values.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Hunga9k50doker/Centic.git
   cd centicBot
   ```

2. Install the required dependencies:

   ```bash
   npm install
   ```

3. Input your Centic `apiKey` in the `tokens.txt` file, one user per line:

   ```bash
   nano tokens.txt
   ```

4. Optionally, you can use a proxy. Paste the proxy in `proxy.txt` in the format `http://username:password@ip:port`:

   ```bash
   nano proxy.txt
   ```

5. Run the script:

   ```bash
   npm run start
   ```

## License

This project is licensed under the MIT License.

---

Feel free to customize this README to match your specific needs! If you have any other questions or need further assistance, let me know.

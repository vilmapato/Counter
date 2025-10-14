# 📦 Base Project Day 1 – Counter Contract

This is a simple **Solidity counter contract** deployed to the **Base Sepolia testnet** as part of the Day 1 assignment of the Base Bootcamp.

---

## 🛠 Deployment Details

- **Deployer Address:**  
  `0xCd123a950B03401937906fC53C49CF65B4868ed8`

- **Contract Address (Base Sepolia):**  
  `0x08Ad79edAb7B5F0E4dd9B8fE39979d05e04F74d2`

- **Transaction Hash:**  
  [`0xff721260e6500527454ee4653d082c135007e35d59dcf0a51e05ce488978b768`](https://sepolia.basescan.org/tx/0xff721260e6500527454ee4653d082c135007e35d59dcf0a51e05ce488978b768)

---

## ⚙️ Tooling Used

- **Framework:** [Foundry](https://book.getfoundry.sh/)
- **RPC Provider:** [Alchemy Base Sepolia Endpoint](https://www.alchemy.com/faucets/base-sepolia)
- **Network:** `Base Sepolia Testnet`

---

## 📝 Notes

- ✅ Contract compiled and deployed successfully on first attempt.
- 🔍 Verified using Basescan for deployment confirmation.

## 🧰 Installation

First, install [Foundry](https://book.getfoundry.sh/getting-started/installation):

in your bash:
curl -L https://foundry.paradigm.xyz | bash
foundryup

forge install

Then, Set your RPC and private key as environment variables in the root create .env file:
BASE_SEPOLIA_RPC_URL="https://base-sepolia.g.alchemy.com/v2/YOUR_API_KEY"
PRIVATE_KEY="your_private_key_here"
BASESCAN_API_KEY ="YOUR_KEY_HERE"

## 📦 Compile the Contract

forge build

## 🚀 Deploy the Contract

forge create src/Counter.sol:Counter --rpc-url $BASE_SEPOLIA_RPC_URL --private-key $PRIVATE_KEY --broadcast

# dApp_FileShare

This project facilitates decentralized image upload and sharing on the blockchain using **Solidity** for the smart contract and **React** for the front-end interface. It enables users to securely upload images to **IPFS (InterPlanetary File System)** and share access with specified users through smart contract functionality.

---

## ✨ Features
- **Decentralized Storage**: Images are uploaded to IPFS, ensuring decentralized and immutable storage.
- **Smart Contract**: Utilizes Solidity smart contracts on the Ethereum blockchain for access control and ownership management.
- **Access Control**: Users can grant or revoke access to their uploaded images to specific individuals through the smart contract.

---

## 🚀 Technologies Used
- **Solidity**: Smart contract development for ownership and access control.
- **React**: Front-end interface for uploading images and managing access.
- **IPFS**: Decentralized storage protocol for hosting uploaded images.

---

## 🛠️ Installation and Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/dApp_FileShare.git

### 2. Install Dependencies for Hardhat
Navigate to the root directory:
```bash
Copy code
cd client
npm install

### 3. Compile the Smart Contract
```bash
Copy code
npx hardhat compile
4. Deploy the Smart Contract
Deploy the Solidity smart contract to an Ethereum testnet or a local development environment:
```bash
Copy code
npx hardhat run scripts/deploy.js --network <network-name>
5. Install Dependencies for the React Front-End
Navigate to the React client directory:
```bash
Copy code
cd client
npm install
6. Run the React Application
Start the React application:

```bash
Copy code
npm start
⚙️ Configuration
Set up Environment Variables:

Obtain API keys from Pinata to interact with IPFS.
Update the React component (FileUpload.js) with your Pinata API keys.
Update Contract Address:

After deploying the smart contract, update the contract address in App.js within the React application.
📖 Usage
Install Metamask:

Ensure Metamask is installed and configured in your browser for Ethereum interactions.
Upload Image Before "Get Data":

Click "Get Data" only after uploading an image on Pinata. Otherwise, an error stating "You don't have access" will occur.
Access Other Users' Images:

Use the "Get Data" button to access other users' images by inputting their Ethereum address. You can only access their images if they've granted you access via the smart contract. Otherwise, an error saying "You don't have access" will occur.
🛑 Important Notes
Ensure that Pinata API keys are correctly set up to enable smooth image uploads to IPFS.
Access control is strictly managed through the Solidity smart contract, ensuring user privacy and ownership.
📂 Project Structure
bash
Copy code
Dgdrive3.0/
├── contracts/          # Solidity smart contracts
├── scripts/            # Deployment scripts
├── client/             # React front-end application
├── hardhat.config.js   # Hardhat configuration
└── README.md           # Project documentation
🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

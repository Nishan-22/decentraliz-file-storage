# Decentralized File Storage System (Web3 DApp)

A decentralized file storage system built using **React**, **Solidity**, **Ethers.js**, and **IPFS**.  
It allows users to upload files to IPFS and store file metadata securely on the Ethereum blockchain.

---

# 🚀 Project Overview

This project is a Web3-based file storage system that removes dependency on centralized cloud storage providers.

Instead of storing files in a central database:
- Files are stored on **IPFS (InterPlanetary File System)**
- File metadata is stored on **Ethereum blockchain**
- Ownership is managed using wallet authentication (MetaMask)

---

# 🎯 Problem Statement

Traditional cloud storage systems suffer from:

- Centralized control over user data
- Risk of censorship or deletion
- Single point of failure
- Lack of transparency in ownership
- Security vulnerabilities in centralized databases

This project solves these issues using blockchain and decentralized storage.

---

# 🏗️ System Architecture
  +------------------------------------------------------+
|                        USER                          |
|                (MetaMask Wallet)                    |
+---------------------------+--------------------------+
                            |
                            v
+------------------------------------------------------+
|                  React Frontend (DApp)              |
|            UI Layer + User Interaction              |
+---------------------------+--------------------------+
                            |
                            v
+------------------------------------------------------+
|                     Ethers.js                       |
|              Blockchain Interaction Layer           |
+---------------------------+--------------------------+
                            |
            +---------------+----------------+
            |                                |
            v                                v
+--------------------------+     +--------------------------+
|  Ethereum Blockchain     |     |           IPFS           |
|  (Smart Contracts)       |     |  (Decentralized Storage) |
|--------------------------|     |--------------------------|
| - File metadata          |     | - Stores actual files    |
| - Ownership records      |     | - Returns CID            |
| - Access logic           |     | - Distributed network    |
+--------------------------+     +--------------------------+

## Frontend
- React.js
- Tailwind CSS
- Ethers.js

## Blockchain
- Solidity
- Ethereum (Sepolia / Local Ganache)
- MetaMask

## Storage
- IPFS (Pinata / Node)

## Tools
- Hardhat
- Node.js
- npm

---

# 📦 System Design

## 1. Frontend Layer (React)
- User interface for uploading and viewing files
- Wallet connection using MetaMask
- Sends transactions via Ethers.js

---

## 2. Blockchain Layer (Solidity)
- Stores file metadata (CID, owner, timestamp)
- Ensures immutable ownership tracking
- Executes smart contract logic

---

## 3. Storage Layer (IPFS)
- Stores actual file data
- Returns unique CID (Content Identifier)
- Distributed and decentralized storage

---

# 🔑 Core Features

- Upload files to IPFS
- Store CID on blockchain
- Wallet-based authentication
- View all uploaded files
- Retrieve file metadata
- Ownership tracking

---

# 📂 Smart Contract Design

## Data Stored:
- File ID
- IPFS CID
- File name
- Owner address
- Timestamp

## Core Functions:
- uploadFile()
- getFile()
- getAllFiles()
- getMyFiles()
- getFileCount()

---

# 🔄 Workflow
User connects MetaMask wallet
User selects file in frontend
File is uploaded to IPFS
IPFS returns CID
CID is sent to smart contract
Blockchain stores metadata
User retrieves file anytime using CID



---

# 🔐 Security Features

- Wallet-based authentication
- Immutable blockchain storage
- Decentralized file system (IPFS)
- No centralized server dependency

---

# 📌 Use Cases

- Decentralized cloud storage
- Academic certificate verification
- Secure document sharing
- NFT metadata storage
- Web3 portfolio project

---



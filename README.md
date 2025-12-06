# MyToken (MTK)

## Overview
**MyToken (MTK)** is a simple ERC-20 compatible token built on Ethereum for learning and experimentation purposes.  
It demonstrates core ERC-20 functionalities including token transfer, delegated transfers, and event emission.

---

## Token Details
- **Name**: MyToken  
- **Symbol**: MTK  
- **Decimals**: 18  
- **Total Supply**: 1,000,000 MTK  

---

## Features
- ✅ Standard ERC-20 implementation  
- ✅ Transfer tokens between addresses  
- ✅ Approve and transferFrom functionality (delegated transfer)  
- ✅ Event emission for transparency (`Transfer`, `Approval`)  
- ✅ Balance tracking for each address  

---

## How to Deploy
1. Open **[Remix IDE](https://remix.ethereum.org/)**  
2. Create a new file named `MyToken.sol`  
3. Paste your ERC-20 contract code into the file  
4. Compile the contract using **Solidity version 0.8.x**  
5. Deploy the contract:  
   - Set the **total supply** (e.g., `1000000 * 10^18` for 1,000,000 MTK with 18 decimals)  
   - Choose the deploying account  

---

## How to Use

### 1. Check Balance
```
balanceOf(0x5B38Da6a701c568545dCfcB03FcB875f56beddC4 ) → returns 999999000000000000000000
```
### 2. Transfer Tokens
```
transfer(0xAb8483F64d9C6d1EcF9b849Ae677dD3315835cb2, 1000000000000000000) → returns true
```
### 3.Approve Token Spending
```
approve(0xAb8483F64d9C6d1EcF9b849Ae677dD3315835cb2, 5000000000000000000) → returns true
```
### 4.Transfer Tokens on Behalf of Owner
```
transferFrom(0x5B38Da6a701c568545dCfcB03FcB875f56beddC4, 0x4B20993Bc481177ec7E8f571ceCaE8A9e22C02db, 5000000000000000000) → returns true
```
### 5. Check Allowance
```
allowance("0x5B38Da6a701c568545dCfcB03FcB875f56beddC4", "0xAb8483F64d9C6d1EcF9b849Ae677dD3315835cb2") → returns 0
```

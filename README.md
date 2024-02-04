![_adbbfce4-9f37-44cf-8c7a-381d279183f1](https://github.com/GustavoLSantos/Ethereum-Testament/assets/28766048/e455cf32-2b62-4263-958a-34188d609e4e)
# Overview
The Ethereum Testament Smart Contract facilitates the execution of a testamentary distribution of Ether (ETH) upon the demise of the contract owner. This decentralized application allows the contract owner (Person X) to specify family members and their respective Ethereum wallet addresses along with the allocated amounts. Upon triggering the testament function, the specified Ether amounts are automatically transferred to the designated family wallets.

## 1. Introduction
#### 1.1 Purpose

* The Ethereum Testament Smart Contract aims to provide a decentralized and secure solution for the automated distribution of Ether to specified family members in the unfortunate event of the contract owner's passing.

#### 1.2 Features

* Testament registration for family members
* Automated testament execution
* Allocation updates for family members

## 2. Getting Started
#### 2.1 Prerequisites

* Ethereum wallet with sufficient ETH for deployment and transactions
* Solidity development environment

#### 2.2 Deployment

* Deploy the smart contract to the Ethereum network of your choice.
* Fund the contract owner's wallet with the desired amount of Ether.

## 3. Usage
#### 3.1 Registering Family Members

* Use the registerFamilyMember function to add family members and specify their Ethereum wallet addresses and allocated amounts.
  
#### 3.2 Testament Execution

* Execute the testament by calling the executeTestament function, which transfers the allocated Ether to the designated family wallets.
  
#### 3.3 Updating Testamentary Allocations

* Adjust family members' allocations by calling the updateAllocation function.
  
## 4. Smart Contract Functions
#### 4.1 registerFamilyMember(address _familyMember, uint256 _allocation)

* Registers a family member with their Ethereum address and allocated Ether.
  
#### 4.2 executeTestament()

* Triggers the testament, transferring allocated Ether to the designated family wallets.
  
#### 4.3 updateAllocation(address _familyMember, uint256 _newAllocation)

* Updates the allocation for a specific family member.
  
## 5. Example Workflow
#### 5.1 Registering Family Members

// Solidity code snippet for registering family members
~~~solidity
testamentContract.registerFamilyMember(0xFamilyMember1, 5 ether);
testamentContract.registerFamilyMember(0xFamilyMember2, 3 ether);
~~~

#### 5.2 Executing Testament

// Solidity code snippet for executing the testament
~~~solidity
testamentContract.executeTestament();
~~~

#### 5.3 Updating Allocations

// Solidity code snippet for updating allocations
~~~solidity
testamentContract.updateAllocation(0xFamilyMember1, 2 ether);
~~~

# Unit 20 - "Joint Savings Account"  

![alt=“”](https://github.com/tiyub/unit-20-joint-savings-account/blob/main/Instructions/Images/20-5-challenge-image.png)  

A Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. This smart contract uses management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.  

### Solution

Smart contract complied successfully.  

![alt=“”](Execution_Results/001-compile.png)  

Making sure that “JavaScript VM” is selected as the environment, “Deploy & Run Transactions” was applied to the Smart contract.  

![alt=“”](Execution_Results/002-deploy.png)  

Using the Dummy Accounts - below - the `setAccounts` function defined the authorized Ethereum address that was able to withdraw funds from deployed contract.  
* Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb  
* Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0  

![alt=“”](Execution_Results/003-setAcc.png)  

Smart contract deposits were tested by sending the following amounts of ether. After each transaction, use the `contractBalance` function to verify that the funds were added to your contract:

* Transaction 1: Send 1 ether as wei
* Transaction 2: Send 10 ether as wei
* Transaction 3: Send 5 ether.

![alt=“”](Execution_Results/004-1EthAsWei.png)  
![alt=“”](Execution_Results/005-10EthAsWei.png)  
![alt=“”](Execution_Results/006-5Eth.png)  

Having successfully deposited funds into the contract, the contract’s withdrawal functionality was test by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`.

![alt=“”](Execution_Results/007-1Acc5Eth.png)  
![alt=“”](Execution_Results/008-2Acc10Eth.png)  

After each transaction, the `contractBalance` function was used to verify that the funds were withdrawn from the contract. The `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

![alt=“”](Execution_Results/009-verify5Eth.png)  
![alt=“”](Execution_Results/010-verify10Eth.png)  

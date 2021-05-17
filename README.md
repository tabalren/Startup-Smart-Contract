# Startup-Smart-Contract

![](Images/SmartContracts_handshake.png)

This code will create an Ethereum-compatible blockchain to build smart contracts. This will enable your company to automate finances for increased transparency and to make accounting and auditing practically automatic!

I have created 2 'Profit Splitter' contracts designed to:

1. Pay employees quickly and easily.
2. Distribute profits to different tiers of employees.

## Contract 1 - Associate Splitter

This contract is designed to accept Ether into the contract and divide the Ether evenly among three associate-level employees. This will allow your company's Human Resources department to pay employees quickly and efficiently.

Refer to the below screenshots for the detailed code.

When deploying the contract in Remix, deploy the contract to your local Ganache chain by connecting to Injected Web3 and ensuring MetaMask is pointed to localhost:8545. See screenshot below with code in Remix and Metamask window open on the right.

You will need to fill in the constructor parameters with your designated employee addresses.

![Screen Shot 2021-05-17 at 3 52 46 PM](https://user-images.githubusercontent.com/74678703/118548142-f364a900-b727-11eb-9e75-2a41646c5ad4.png)

Test the deposit function by sending various values. Keep an eye on the employee balances as you send different amounts of Ether to the contract and ensure the logic is executing properly.


In testing the deposit function, we can see proof of the transaction taking place looking at the resulting balances in Ganache:

Ganache balance before depositing 3 ETH (Balance of 92.80): 

<img width="940" alt="beforedeposit" src="https://user-images.githubusercontent.com/74678703/118548177-feb7d480-b727-11eb-9568-2b8669b2ee80.png">

Ganache balances after deposting 3 ETH (Balance of 89.80 in main account and profits split across 3 employee addresses):

<img width="928" alt="afterdeposit" src="https://user-images.githubusercontent.com/74678703/118548362-36268100-b728-11eb-8980-03aa34f91153.png">


## Contract 2 - Tiered Profit Splitter

This contract will distribute different percentages of incoming Ether to employees at different tiers/levels. For example in this contract, the CEO gets paid 60%, CTO 25%, and Bob the Associate gets 15%.

Refer to the screenshot below of the solidity code with the environment, contract inputs and MetaMask setup required to execute the contract.

<img width="1619" alt="Screen Shot 2021-05-17 at 3 38 48 PM" src="https://user-images.githubusercontent.com/74678703/118547414-4853ef80-b727-11eb-9219-ec136ce0a4c7.png">

In testing the deposit function, we can see proof of the transaction taking place looking at the resulting balances in Ganache:

Ganache balance before depositing 3 ETH (Balance of 86.79):
<img width="908" alt="Screen Shot 2021-05-17 at 3 39 05 PM" src="https://user-images.githubusercontent.com/74678703/118547507-66b9eb00-b727-11eb-9f16-6ee6d1cca24a.png">

Ganache balance after depositing 3 ETH (Balance of 83.79 and profits split across 3 tiered employee addresses): 
<img width="912" alt="Screen Shot 2021-05-17 at 3 39 41 PM" src="https://user-images.githubusercontent.com/74678703/118547515-691c4500-b727-11eb-8f65-e449196565b3.png">



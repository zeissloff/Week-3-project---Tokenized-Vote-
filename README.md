# Week-3-project---Tokenized-Vote-

### Instructions :

1. Write smart contract
2. Deploy contract
3. Run scripts:
    + giveVotingTokens 
    + delegateVotingPower 
    + castingVote 
    + checkingVotePower
    + queryingResults 

### Prerequisites for the Project:

Environment Configuration: create a .env file and add your Alchemy API key and Private key.

Compilation: be able to "run npx hardhat compile" to compile the MyToken.sol contract and the TestMyToken.ts script.

Network configuration: Use the Sepolia Testnet for deployment and testing. 

# Deployment of the contract and minting token : 
+ GiveTokens.ts 
+ Command used with the following accounts :
  + Acc1 = 0x0aCA03DA72A643f5403d07d7657C17B6E3ED575D
  + Acc2 = 0x98dd07d88aFE0E5C318747AabC360E8E3A741767

```bash
npx ts-node --files ./scripts/GiveTokens.ts 0x0aCA03DA72A643f5403d07d7657C17B6E3ED575D 0x98dd07d88aFE0E5C318747AabC360E8E3A741767npx ts-node --files ./scripts/DK_DeployMyERC20Token.ts <ACCT1_ADDRESS> <ACCT2_ADDRESS>
```
![2024-08-31 01 07 10](https://github.com/user-attachments/assets/c35538be-0b17-4a49-8206-12d1716a00b7)

+ TokenizedBallot.ts

```bash
npx ts-node --files ./scripts/DelegateVote.ts "Proposal1" "Proposal2" "Proposal3" 0x5fa2b9098f5dce19c6c19cc27e4feef22df30797
```
+ The contract address : 0x798fe65fefb58e2da6b25e24423f86869360113d
(https://sepolia.etherscan.io/address/0x798fe65fefb58e2da6b25e24423f86869360113d)

# Run scripts : 

+ GiveVotingTokens - ./scripts/GiveToken
+ As seen above 
```bash
npx ts-node --files ./scripts/DK_DeployMyERC20Token.ts <ACCT1_ADDRESS> <ACCT2_ADDRESS>
```

+ DelegateVotingPower - ./scripts/DelegateVote
```bash
npx ts-node --files ./scripts/DelegateVote.ts "Proposal1" "Proposal2" "Proposal3" 0x798fe65fefb58e2da6b25e24423f86869360113d
```
<img width="598" alt="Capture d’écran 2024-09-01 à 22 55 10" src="https://github.com/user-attachments/assets/9fe5ade0-5cf0-4070-880d-deec0dcafee5">


+ CastingVote - ./scripts/CastingVote
```bash
npx ts-node --files ./scripts/CastingVote.ts 0x0aCA03DA72A643f5403d07d7657C17B6E3ED575D
```
+ CheckingVotePower - ./scripts/CheckVoting
```bash
npx ts-node --files ./scripts/checkVotingRights.ts
```
<img width="1429" alt="Capture d’écran 2024-09-01 à 22 23 31" src="https://github.com/user-attachments/assets/1e841a7e-f217-48a0-816f-d5c452a6f9d7">

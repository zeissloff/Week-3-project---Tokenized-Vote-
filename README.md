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

Environment Configuration: Create a .env file and add your Alchemy API key and Private key.

Compilation: Be able to "run npx hardhat compile" to compile the MyToken.sol contract and the TestMyToken.ts script.

Network Configuration: Use the Sepolia Testnet for deployment and testing. :

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
+ The contract address : 0x5Fa2B9098f5dCe19C6c19cC27e4feEF22DF30797
https://sepolia.etherscan.io/address/0x5fa2b9098f5dce19c6c19cc27e4feef22df30797

# Run scripts : 

+ GiveVotingTokens - ./scripts/GiveToken
```bash

```

+ DelegateVotingPower - ./scripts/DelegateVote
```bash

```

+ CastingVote - ./scripts/CastingVote
```bash

```
+ CheckingVotePower - ./scripts/CheckVoting
```bash

```

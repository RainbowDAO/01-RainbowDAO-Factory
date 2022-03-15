# Documentation on how to run the project

## Contract introduction
- DaoFactory: Users can create their own DAO through factory contracts,displays a list of dao information,It's a collection of all the contracts.
- Authority: Used to manage permissions between accounts or contracts, which can be changed by proposal.
- DaoBaseInfo: It is used to save the basic information and types of dao.
- DaoManage: The dao's main logical management contract can manage funds or change contract parameters or contract permissions by requesting proposals.
- DaoMembers: Management contract for DAO members.
- ERC20Factory: This contract allows you to create your own ERC20 tokens.
- RouteManage: Routing contracts, record the addresses of all contracts.
- Vault: Token management contracts manage the expenditure and income of various tokens.
- Vote: The ability to initiate proposals for voting is the primary way to manage dao functionality.
## Dependencies

- Linux or Mac
- node ≥ 14

## Network & Contract
- Network Name: Rinkeby Test Network
- RPC URL: https://rinkeby.infura.io/v3/9aa3d95b3bc440fa88ea12eaa4456161

### contract address

#### DaoFactory
0x3cf33889A31666BBD75946e5650CF6e643B2C0B2
#### Authority
0x8bBef131a546d8151297e96C68AE614E5a80037d
#### DaoBaseInfo
0xb8Fda38562bd77dD8D2A0335e539D4188DF030a3
#### DaoManage
0xDEf7188Bd888e230E7258410EF8a4e6Bee8AaaFF
#### DaoMembers
0xe1240c60f37ae1CdeC036591C9814c1Fce8d986c
#### ERC20Factory
0x2697c5DAC9c13D9EA97F097ee5E7702d195E28dc
#### RouteManage
0x90E7F2c414a066C0995dccDADCd095d3e057cdE4
#### Vault
0x466Dc7d36085e981A7Ec5cb773e9b159f88CFF23
#### Vote
0xf9A3f8eb156B49Ae50ebe0A9e45A46aa22766795

## Installing

```bash
git clone https://github.com/RainbowDAO/01-ETHDenver2022-RainbowDAO-Factory.git
npm install
```

**Note**: Only the Metamask wallet is available for this demo


## Deploy Contracts
Open a local node or complete the information in the ```truffle-config.js``` and add the mnemonic to the ```secret```

```bash
npm install -g @truffle/hdwallet-provider
truffle compile && truffle migrate
```
You will deploy contracts
- DaoFactory

## Create a DAO
The creatDao in the DaoMain contract creates a DAO of its own, defining names, logos, and symbols

```creatDaoWithNewToken()``` or ```creatDao()```


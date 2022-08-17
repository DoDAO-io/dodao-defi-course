## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Smart Contratcs
 
 
---

##### What does a Transaction mean in DeFi?  

- [ ]  Transferring tokens via courier.
- [ ]  Transferring fiat currency from one crypto wallet to another.
- [x]  Transactions are an action initiated by an externally owned account.
- [ ]  Transferring tokens from one bank account to another.
  
Hint: NoHint
         
Explanation: A transaction in DeFi refers to any action initiated by an externally owned account that brings about a change in the state of blockchain.

Sub Topics: ethereum-transactions-working
 

---

##### What are the different types of accounts owned by Ethereum users?  

- [ ]  Ethereum Trading account
- [x]  Externally owned account
- [ ]  Ethereum Transfer account
- [x]  Smart Contract account
  
Hint: NoHint
         
Explanation: Externally owned accounts (EOA) and Smart Contract account are the two types of accounts owned by Ethereum users.

Sub Topics: ethereum-transactions-working
 

---

##### Which of the following accounts have no code associated with them?  

- [ ]  Smart Contract account
- [x]  Externally owned account
- [ ]  Ethereum Transfer account
- [ ]  Ethereum Trading account
  
Hint: NoHint
         
Explanation: Externally owned accounts have no code associated with them.

Sub Topics: ethereum-transactions-working
 

---

##### How does a transaction occur in a Smart Contract Account?  

- [ ]  The transaction involves interaction with many dApps during execution.
- [x]  Execution of a code in the smart contract helps in transactions.
- [ ]  Smart contracts cannot be used to conduct transaction.
  
Hint: Smart Contracts have clauses written in code.
         
Explanation: Transaction in smart contracts are executed when the code in them runs successfully.

Sub Topics: ethereum-transactions-working
 

---

##### What does it mean by Atomicity of Ethereum transaction?  

- [ ]  Transaction steps occur one by one in a sequence.
- [ ]  Transactions need to be of a small amount.
- [x]  Transactions are reversed if a clause fails in a smart contract.
- [x]  Transactions cannot overlapp, divide or interrupt.
  
Hint: NoHint
         
Explanation: Atomicity is a property of Ethereum transaction which means that when a clause in a smart contract is not met or remains unsatisfied then the transaction fails and returns to the pre-transaction stage. These transactions cannot divide into smaller units. Moreover, they cannot overlapp or interrupt other transactions.

Sub Topics: ethereum-transactions-working
 

---

##### What are the properties of  Ethereum Transactions?  

- [x]  Peer to Peer
- [x]  Irreversible once executed
- [x]  Atomic
- [ ]  Involves middlemen
  
Hint: NoHint
         
Explanation: Ethereum transactions occur on P2P (Peer-to-Peer) basis. These transactions are irreversible once executed and they are atomic in nature.

Sub Topics: ethereum-transactions-working
 

---

##### An Externally owned account can be used to transfer......  

- [ ]  Bitcoin
- [ ]  Ethereum
- [ ]  DogeCoin
- [x]  All of the above
  
Hint: NoHint
         
Explanation: An EOA can be used to send any tokens within the Ethereum Network.

Sub Topics: ethereum-transactions-working
 

---

##### Which of the following is not part of account field?  

- [ ]  nonce
- [x]  wallet address
- [ ]  codeHash
- [ ]  storageRoot
  
Hint: NoHint
         
Explanation: An Ethereum account composes of majorly 4 fields. Those are nonce, balance, codeHash and storageRoot.

Sub Topics: ethereum-transactions-working
 

---

##### How is the transaction data stored in the blockchain?  

- [x]  Blocks
- [ ]  Smart contracts
- [ ]  Cryptographic hashes
- [ ]  None of the above
  
Hint: Working of transactions in the blockchain
         
Explanation: The transaction data is stored in the form of a block in the blockchain.

Sub Topics: ethereum-transactions-working
 

---

##### Ethereum accommodates which of the below types of transactions?  

- [ ]  Regular Transactions
- [ ]  Contract Deployment Transactions
- [ ]  Execution of a contract
- [x]  All of the above
  
Hint: NoHint
         
Explanation: The 3 types of Ethereum Transactions are - Regular Transactions, Contract Deployment Transactions, Execution of a contract.

Sub Topics: ethereum-transactions-working
 

---

##### Where are pending and unconfirmed transactions stored?  

- [ ]  Blocks
- [ ]  Sender’s Wallet
- [x]  Mempool
- [ ]  Miner’s Wallet
  
Hint: NoHint
         
Explanation: The place where pending or unconfirmed transactions are stored is known as mempool.

Sub Topics: miner-extractable-value
 

---

##### What happens when mempool is overloaded with transactions?  

- [x]  Delayed confirmation of transactions
- [ ]  Reduction in backlog.
- [x]  Increase in transaction fees.
- [ ]  Low traffic in the pool
  
Hint: Overcrowded Mempool creates more time in successful transaction.
         
Explanation: When the mempool becomes overloaded with transactions, it resutls in delayed confirmations of these transactions and increase in the gas fees as well.

Sub Topics: miner-extractable-value
 

---

##### What users can do if there is an overload in the mempool?  

- [ ]  Cancel the transaction
- [x]  Switch to paid speed network
- [x]  Pay more transaction fees
- [x]  Wait for confirmation
  
Hint: NoHint
         
Explanation: When there is too much traffic in the mempool, users might switch to a paid speed network which would lead to more transaction fees. Otherwise users can just wait to get a confirmation.

Sub Topics: miner-extractable-value
 

---

##### How can miners tamper the blockchain?  

- [ ]  Excluding transaction
- [ ]  Including transaction
- [ ]  Re-ordering transactions
- [x]  All of the above
  
Hint: NoHint
         
Explanation: Miners have access to the mempool. So, they can exclude a transaction, include a transaction or re-ordering any transaction in the pool.

Sub Topics: miner-extractable-value
 

---

##### What does Miners Extractable Value refer to?  

- [ ]  Standard block reward
- [ ]  Gas fees
- [ ]  Interest on large order
- [x]  Extra source of income from transactions
  
Hint: NoHint
         
Explanation: Miner Extractable Value is the extra income other than standard block reward and gas fees which the miners get by tampering with the transaction orders (front-running).

Sub Topics: miner-extractable-value
 

---

##### How do “searchers” execute gas golfing? Gas golfing refers to programming transactions using the least amount of gas.  

- [x]  Using addresses which have long string of zeros.
- [x]  Leaving some amount of ERC-20 tokens in contracts.
- [ ]  Reducing transactions into smaller parts.
- [ ]  Use more efficient systems to execute transactions.
  
Hint: Decrease the storage of a block
         
Explanation: Addresses which have a long string of zeros reduce the size of the block and hence the gas required to mine it. Moreover, the contract must not be kept empty it should have some amount of ERC-20 to remove the gas required for initialising the contract.

Sub Topics: miner-extractable-value
 

---

##### Which of the following are examples of MEV?  

- [x]  DEX Arbitrage
- [ ]  Selling of NFTs
- [x]  Sandwich trading
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: DEX Arbitrage and Sandwich trading are the examples of MEV.

Sub Topics: miner-extractable-value
 

---

##### What are the ill-effects of increasing MEV?  

- [ ]  Miners get more money-minded
- [ ]  More transactions occur on blockchain creating traffic.
- [ ]  High gas fees
- [x]  Alteration in exchange rates
  
Hint: Effets of MEV crowding
         
Explanation: Increase in the MEV can result in alteration in exchange rates due to front-running.

Sub Topics: miner-extractable-value
 

---

##### What are the benefits of MEV?  

- [x]  DEX arbitrage offers competitive pricing to users.
- [x]  Speedy liquidations help lenders get paid back
- [ ]  Increase in the rate of transaction
- [ ]  None of the above
  
Hint: Miner Extractabe Value benefits
         
Explanation: DEX arbitrage helps the user get competitive pricing for a coin and speedy liquidation help lenders get paid back.

Sub Topics: miner-extractable-value
 

---

##### What was the amount collected (in million $) via MEV in 2021?  

- [ ]  500
- [x]  780
- [ ]  650
- [ ]  200
  
Hint: NoHint
         
Explanation: The amount collected via MEV in 2021 is around $780 Million.

Sub Topics: miner-extractable-value
 

---

##### What is a famous example of a non-fungible token?  

- [x]  Cryptokitties
- [ ]  Zcash
- [ ]  Augur
- [ ]  US Dollar
  
Hint: NoHint
         
Explanation: Cryptokitties is a famous non-fungible token.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Which of the following are two most important languages for coding the smart contract on ethereum?  

- [ ]  Rust and Solidity
- [ ]  Python and Rust
- [x]  Solidity and Vyper
- [ ]  Solidity and Python
  
Hint: NoHint
         
Explanation: Solidity and Vyper are the coding languages used for coding the smart contract.

Sub Topics: smartcontracts-gas-oracles
 

---

##### A smart contract can be used in which of the following fields?  

- [ ]  Trading
- [ ]  Real Estate
- [ ]  Supply chain management
- [x]  All of the above
  
Hint: Functions of Smart Contracts
         
Explanation: Smart contracts can be used in any field which uses the interpretation and transfer of data.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What is the maximum limit of the size of smart contract on ethereum?  

- [ ]  ~1.2 Gb
- [ ]  ~30 Mb
- [x]  ~24 Kb
- [ ]  No such fixed limit
  
Hint: NoHint
         
Explanation: The current maximum limit of the amount of data that can be stored by a smart contractis 24 Kb.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What are the features of smart contracts?  

- [x]  Composability
- [x]  Irreversible
- [x]  Permissionless
- [ ]  Easily Editable
  
Hint: Features of Blockchain combined with smart contracts
         
Explanation: Smart contracts are composable, the clauses are irreversible and they do not require any permission to be executed.

Sub Topics: smartcontracts-gas-oracles
 

---

##### Why smart contracts cannot interact with “real–world” events?  

- [ ]  When needed, these details can be coded in the contract.
- [ ]  The information is already coded
- [x]  They cannot send HTTP requests
- [ ]  They do not need external information
  
Hint: Smart contract is plane code of agreements
         
Explanation: Smart contract are not capable enough to send HTTP Requests such as GET, POST etc.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What are the benefits of Multisig contracts over regular contracts?  

- [x]  Avoid single point of failure
- [x]  Divide responsibility for contract execution and management
- [x]  Prevents loss of funds due to a single private key
- [ ]  Defaulters can be caught easily
  
Hint: Multisig contracts have many validators
         
Explanation: Multisig contracts have many validators, this prevents single point of failue. Moreover, responsibilty for contract execution and management is distributed. Many contributors help in preventing the loss of funds due to a single private key.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What is the unit to measure the amount of computational effort in Ethereum?  

- [ ]  Ethereum Energy
- [x]  Gas
- [ ]  Coal
- [ ]  Fuel
  
Hint: NoHint
         
Explanation: Gas is the unit to measure the amount of computational effort in Ethereum.

Sub Topics: smartcontracts-gas-oracles
 

---

##### Suppose Ga is the gas required to include a regular transaction and Gb is the gas required to execute a smart contract the which of the following will be true?  

- [ ]  Ga = Gb
- [x]  Ga < Gb
- [ ]  Ga > Gb
- [ ]  Data insufficient to determine a relation
  
Hint: Complexity of a transaction
         
Explanation: Gb will be greater than Ga because regular transactions consume less gas compared to a smart contract which is far more complex during execution .

Sub Topics: smartcontracts-gas-oracles
 

---

##### How are gas prices denoted?  

- [x]  Gwei
- [ ]  Bitcoin
- [ ]  DAOs
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: gwei is the unit used to denote gas price. 1 gwei = one billionth of an ETH.

Sub Topics: smartcontracts-gas-oracles
 

---

##### ___A___ requires gas whereas ___B___  requires no gas.  

- [ ]  A = Transaction  B= Smart Contract
- [x]  A = Transaction  B= Check Balance
- [ ]  A = Smart Contract  B = Transaction
- [ ]  A =  Check Balance  B = Transaction
  
Hint: Regular Transaction and read only functions
         
Explanation: Regular transaction requires gas whereas checking balance (read-only) requires no gas.

Sub Topics: smartcontracts-gas-oracles
 

---

##### Determine what happens - You execute a transaction which requires 21 units of gas but you supplied only 20 units of gas.  

- [ ]  Transaction is successful and 1 unit of gas added as a debt
- [x]  Transaction unsuccessful and gas consumed
- [ ]  Transaction unsuccessful and gas returned
- [ ]  Transaction waits for the addition of 1 unit of gas.
  
Hint: Consumption of gas
         
Explanation: Transaction is unsuccessful and the gas has already been consumed and provided to the miner who processed the transaction.

Sub Topics: smartcontracts-gas-oracles
 

---

##### 1 gwei represents......  

- [ ]  10-6  of ETH
- [x]  10-9  of ETH
- [ ]  10-7  of ETH
- [ ]  10-8  of ETH
  
Hint: NoHint
         
Explanation: 1 gwei represents one billionth of a ETH.

Sub Topics: smartcontracts-gas-oracles
 

---

##### Why is gas necessary in the Ethereum network?  

- [ ]  Reward the miners
- [x]  Prevent spamming in the network
- [x]  Avoid infinite loop
- [ ]  Gas can be removed to make network better
  
Hint: Features of Gas
         
Explanation: High Gas prevents spamming in the network and smart contract having an infinite loop will terminate when it runs out of gas.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What are the reasons behind high gas fees?  

- [ ]  Increasing popularity of the Ethereum network.
- [ ]  Higher tip to outbid other transactions
- [ ]  Smart contracts consume a lot of gas
- [x]  All of the above
  
Hint: Increasing gas demand
         
Explanation: All the three listed reasons are responsible for high gas fees.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What are Oracles?  

- [ ]  People who update network about real-world
- [x]  On-chain APIs
- [ ]  To check if a smart contract is mined and confirmed
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: Oracles are on-chain APIs which help a smart contract get realtime data.

Sub Topics: smartcontracts-gas-oracles
 

---

##### What is/are the oracle problem?  

- [ ]  Oracle does not interact effectively with smart contract
- [x]  A single source of truth is unreliable and insecure
- [ ]  Oracles fail during the time of congestion
- [ ]  All of the above
  
Hint: Trust issues on single oracle
         
Explanation: A single oracle cannot be relied upon for accurate and trustworthy information. In DeFi there can be many oracle which would have been programmed to interfere wrongly with the smart contract.

Sub Topics: smartcontracts-gas-oracles
 

---

##### Who introduced ERC 20?  

- [ ]  Vitalik Buterin
- [x]  Fabian Vogelstellar
- [ ]  option 3
- [ ]  option 4
  
Hint: NoHint
         
Explanation: Fabian Vogelstellar introduced ERC-20 for fungible tokens.

Sub Topics: fungible-non-fungible-tokens
 

---

##### How does ERC 20 empower DeFi?  

- [x]  Transfer tokens from one account to another
- [x]  Get the current token balance of an account
- [ ]  Forgery of assets increases.
- [x]  Get the total supply of token available in the network
  
Hint: Advantages of ERC-20
         
Explanation: ERC-20 enbales transferring of tokens, get current token balance and also get the total supply of token that is available in the market.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Which of the following token is used to represent the ownership of an asset?  

- [ ]  Utility Tokens
- [x]  Equity Token
- [ ]  Governance token
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: Equity token which is a type of Fungible token is used to represent the ownership of an asset or in a pool.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Which of the following tokens have an intrinsic value proposition?  

- [ ]  Equity Token
- [x]  Utility Tokens
- [ ]  Governance token
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: Utility tokens have an intrinsic value proposition.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Which of the following acts as a governance token?  

- [x]  UNI token
- [ ]  Bitcoin
- [ ]  Ethereum
- [ ]  SHIBA coin
  
Hint: NoHint
         
Explanation: UNI token acts as a governance token for the UNISWAP decentralised exchange.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Who introduced ERC -721?  

- [ ]  Vitalik Buterin
- [x]  Dieter Shirley
- [ ]  Fabian Vogelstellar
- [ ]  Changpen Zao
  
Hint: NoHint
         
Explanation: Dieter Shirley along with her team was responsible for introduction of ERC-721.

Sub Topics: fungible-non-fungible-tokens
 

---

##### What differentiates ERC 721 (NFTs) from ERC 20 (FTs)?  

- [ ]  Deployment on the Ethereum network
- [x]  Unique Identity to each token
- [ ]  Size of the token
- [ ]  They are identical
  
Hint: NoHint
         
Explanation: ERC-721 (NFTs) are unique tokens that is no two NFTs can have the same token id whereas Fungible tokens are not unique.

Sub Topics: fungible-non-fungible-tokens
 

---

##### Which of the following is a multi-token standard?  

- [ ]  ERC 20
- [ ]  ERC 721
- [x]  ERC 1155
- [ ]  option 4
  
Hint: NoHint
         
Explanation: ERC-1155 is a multitoken standard which is used to handle Fungible and Non-fungible tokens simultaneously.

Sub Topics: fungible-non-fungible-tokens
 

---

##### For a web application we use web server, for mobile application we use mobile server, so for the decentralised applications we use......  

- [ ]  Distributed communication server
- [x]  Blockchain server
- [ ]  Distributed application server
- [ ]  Centralised server
  
Hint: NoHint
         
Explanation: A blockchain server is used to handle decentralised applications.

Sub Topics: dapps
 

---

##### What does the web3 library do to help dApps communicate with the Ethereum Network?  

- [ ]  Soap Requests
- [ ]  RPC calls
- [x]  REST requests
- [ ]  POST Requests
  
Hint: NoHint
         
Explanation: web3 enables REST requests in the Ethereum Network.

Sub Topics: dapps
 

---

##### What does ERC stand for?  

- [ ]  Ethereum Replacement of code
- [ ]  Ethereum Requisite for code
- [x]  Ethereum Request for Comments
- [ ]  Ethereum Revision Comments
  
Hint: NoHint
         
Explanation: ERC stands for Ethereum Request for Comments

Sub Topics: fungible-non-fungible-tokens
 

---

##### Explain the importance of standardization to dApps?  

- [x]  So that they follow certain convention
- [x]  So that they can implement certain methods
- [ ]  So that they all can be the same
- [ ]  All of the above
  
Hint: Features of dapps
         
Explanation: dApps are standardised so that they can follow certain conventions and all follow certain common methods.

Sub Topics: dapps
 

---

##### What kind of dApp did bitcoin enable?  

- [x]  P2P payment system
- [ ]  Anonymous Payment system
- [ ]  Private Payment system
- [ ]  Dysfunctional payment system
  
Hint: NoHint
         
Explanation: Bitcoin works on the P2P payment system.

Sub Topics: dapps
 

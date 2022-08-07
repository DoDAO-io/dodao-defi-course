## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Smart Contratcs
 
 **Working of Ethereum Transactions**        
- How Ethereum Transaction work?
  * Transactions involve sending data and/or ETH (or other tokens)
  from one address to another.
  * An Ethereum user can control addresses through an externally
  owned account (EOA) or by using smart contract code (contract
  account).
  * When sending data to a contract account, the data are used to
  execute code in that contract.
  * Transactions sent to an EOA can only transfer ETH.
  * A single transaction starts with an end user from an EOA, but it can pass through many dApps (decentralised Applications) before completing.
  * Transaction begins with a single smart contract and continues to carry on all the intermediate steps within the contract body.

- Atomicity
  * This is one of the most important property of Ethereum Transaction Mechanism which makes DeFi different from CeFi.
  * The transactions in Ethereum are atomic which means the clauses in a smart contract can lead to failure of transaction and thus all the steps of the transaction are reversed.
  * Atomicity is a critical feature of transactions because funds can
  move between many contracts (i.e., “exchange hands”) with the
  knowledge and security that if one of the conditions is not met,
  the contract terms reset as if the money never left the starting
  point.
 
 **Miner Extractable Value**        
- Mempool
  * Transactions are posted to a memory pool, or mempool, before
  they are added to a block. 
  * Miners monitor these posted transactions, add them to their own
  mempool, and share the transaction with other miners to be
  included in the next available block.

- Miner Extractable Value
  * Any actor can see transactions in the mempool by running or
  communicating with mining nodes.
  * This observation allows for front-running (legal in the DeFi space) to miners. If miner encounters a large order, they can plave their order before that, hence the miners are incentivised to do so.
  * Miner extractable value (MEV) is a measure of the profit that the
  miner could make by including, excluding or re-ordering
  transactions. 
  * This is one of the drawback of the Proof of work consensus mechanism. Obfuscating transactions can mitigate MEV, thus hiding from miners how they might profit from transactions.
 
 **Smart Contracts, Gas and Oracles**        
- Smart Contracts
  * Ethereum is the example of most popular smart contract platform.
  * A smart contract is code that can create and transform arbitrary data or
  tokens on top of the blockchain of which it is a part.
  * These are extremely powerful because it allows users to trustlessly encode
  rules for any type of transaction and even create scarce assets with
  specialized functionality.
  * Many standard business contracts can be algorithmically encoded and
  algorithmically enforced. These contracts run on the Ethereum blockchain and are run on every node.
  * This is not just useful for finance. For example, supply chains are another
  good example.

- Gas 
  * Transactions have a gas fee that is the fee received by the miners for conducting transactions.
  * Transactions have a gas fee, which varies based on the complexity
  of the transaction. E.g., low gas fee is used to compensate a miner
  for including and executing a transaction, and high gas fee for
  more data-intensive transactions.
  * If a transaction reverts due to any failure or runs out of gas the
  miner forfeits all gas used until that point. This helps miners earn even if large volumes of failed transactions occur.

  - Gas fees
    * The gas price is determined by the market and effectively creates
    an auction for inclusion in the next Ethereum block.
    * Higher gas fees signal higher demand and therefore generally
    receive higher priority for inclusion.
  
  - Gas Price 
    * Every operation on the Ethereum blockchain requires gas.
    * Each unit of gas has a gas price, which is denoted in gwei. 1 gwei = 1
      billionth of an ETH. Gas prices increase as users outbid one another
      during times of higher network congestion.
  
  - Gas Limit
    * The gas limit is the maximum amount of gas a user is willing to use for a
    transaction. A transaction can include multiple operations.
    * If there is residual amount of gas after the transaction is complete, then the user gets back the remaining gas.

  - Turing Complete
    * Gas plays a very important role. If a malicious attack is planned then it would be extremely expensive to carry out.
    * Ethereum is turing complete whereas Bitcoin is not.

- Oracles
  * Ethereum blockchain nows only of what happens inside the Blockchain. But how does it get the information needed from the outside world? Here Oracles come into play.
  * An oracle, in the context of smart contract platforms, is any data source for reporting information external to the blockchain. 

  - Oracle Problem
    * This refers to the correctness of the off-chain information that is provided by the oracle.
    * One Ethereum-based platform known as Chainlink is designed to solve the
    oracle problem by using an aggregation of data sources. The Chainlink
    whitepaper includes a reputation-based system that is decentralized.

  
 
 **Fungible and Non fungible Tokens**        
- ERC 20 (Ethereum Request for Comment 20)
  * ERC 20 is implemented standard for fungible tokens created using the Ethereum blockchain network.
  * When a token implements the ERC-20 interface, any application
  that generically handles the defined functionality can instantly
  and seamlessly integrate with the token.
  * Hence, fungible tokens can be of many types as discussed below.

- Types of Fungible Tokens
  - Equity Tokens
    * An equity token (not traditional stocks) is simply a token that
    represents ownership of an underlying asset or pool of assets. 
    * The units must be fungible so that each corresponds to an
    identical share in the pool.

  - Utility Tokens
    * Utility tokens are fungible tokens that are required to utilize some
    functionality of a smart contract system or that have an intrinsic
    value proposition defined by its respective smart contract system.
    * Some example of utility tokens include:
      - To be collateral (e.g., SNX)
      - To represent reputation or stake (e.g., REP, LINK)
      - To maintain stable value relative to underlying or peg (e.g., DAI, Synthetix Synth)
      - To pay application-specific fees (e.g., ZRX, DAI, LINK)

  - Governance Tokens 
    * Governance tokens are similar to equity tokens in the sense they
    represent percentage ownership. Instead of asset ownership,
    governance token ownership applies to voting rights.
    * Any platform with admin-controlled functionality is not truly DeFi
    because of the admins’ centralized control. For this reason, many platforms strive for a decentralized upgrade process, often mediated by a governance token.
    * UNI token introduced by Uniswap DEX, is a type of governance token which used, as voting rights whenever there is a need to incorporate an upgrade in the existing mechanism of exchange.
  
 
 **Decentralised Applications**        
- Decentralised Applications
  * dApps are similar to traditional software applications except they live on a
  decentralized smart contract platform.
  * The primary benefit of these applications is their permissionlessness and
  censorship-resistance. Anyone can use them, and no single body controls
  them.
  * A decentralized autonomous organization (DAO) has its rules of operation
  encoded in smart contracts that determine who can execute what behavior
  or upgrade.   
  * It is common for a DAO to have some kind of governance token, which gives
  an owner some percentage of the vote on future outcomes.
 
 

## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Decentralised Exchanges
 
 **Introduction to Decentralised Exchanges**        
- What is an Exchange?
  * An exchange is a marketplace or platform where securities (such as stocks, bonds, preferred shares, ETFs, etc.), commodities, derivatives, and other financial instruments are traded (i.e buying and selling among customers). Eg:- New York Stock Exchange(US), National Stock Exchange(India), Shanghai Stock Exchange(China)

- What is a Crypto Exchange?
  * Crypto or cryptocurrency or digital-currency exchange is a marketplace or platform which allows customers to trade cryptocurrencies for other assets, such as conventional fiat money(eg: U.S. Dollar, Japanese Yen, Euro, etc.) or other digital currencies.
  * Types of Crypto Exchange:-
    * Traditional or Centralized Exchange ( CEX )
    * Decentralized Exchange ( DEX )
 
 **Types of Crypto Exchange**        
- Traditional or Centralized Exchange (CEX):
  * A centralized crypto exchange is one that's created and run by a company. These exchanges are considered centralized because one company oversees all the transactions and sets the exchange's rules and fees.
  * Transactions are done using traditional “Order Book” models that are officiated by banks, brokers, or any other intermediary.
  * Customer data(such as KYC) and transactional data are stored by a company.
  * For example, Coinbase, Crypto.com and FTX create and run popular CEXes for a profit.
  * Now, What is an “Order Book”?
    * An order book is a list of orders that presents different offers from buyers and sellers for a specific security.
    * It also shows the prices and volumes that people in the market are willing to buy and sell the security for.
  * There are two types of CEX based on the order book model:
    - CEX with Server Order Book model:
      * All the customers’ trading data, prices, and volumes of securities are stored in a Centralized Server.
      * Trade matching and settlement are faster.
      * No fees are deducted for canceled orders.
      * No censorship resistance as all data are stored on a centralized server.
      * Exchange operators can front-run customers.

    - CEX with Onchain Order Book model
      * All the customers’ trading data, prices, and volumes of securities are stored on a Blockchain.
      * Provide censorship resistance, as all data are stored on a distributed, and decentralized ledger in the form of immutable data blocks on the blockchain which are publicly shared among all its network nodes.
      * Trade matching and settlement might be slow due to blockchain scalability issues.
      * Fees are deducted in the form of Gas Fees for both successful and canceled orders.
      * Miner/Trader/Exchange Operator can front-run users.
 
 **Decentralized Exchange (DEX)**        
- Decentralized Exchange (DEX)
  * A peer-to-peer marketplace where transactions between crypto traders are done mostly using Automated Market Maker (AMM) without banks, brokers, or any other intermediary intervention.
  * Customer, transactional, and all other forms of data are stored on Blockchain. 
  * Eg: Uniswap, dYdX (which runs on Ethereum Blockchain)

  - Pros
    * No KYC is required as trades are done in terms of account address 
    * No fees are paid to the exchange.
    * No impermanent loss (this will be discussed later in this course)
    * Censorship resistance is governed by Smart Contracts and not by any central authority

  - Cons
    * Fees (i.e Gas Fee) are deducted as an additional charge for a deposit, withdrawal, or trade creation/cancelation.
    * Trade settlement might be slow due to blockchain scalability issues. 
    * Sometimes, not fully decentralized due to mediating server for speeding the process of trade execution.
 
 **Automated Market Maker (AMM)**        
- Automated Market Maker (AMM):
  * AMM is a type of DEX protocol that relies on a mathematical formula that allows digital assets to be traded without permission, automatically by using liquidity pools instead of the traditional order book pricing model. This formula can vary with each protocol. For example, Uniswap uses the Constant Product AMM protocol which is as follows:-
    * Asset X quantity * Asset Y quantity = K (a constant)  simply  X*Y=K
      * Properties of popular Constant Product AMM protocol:
        * Instant liquidity, irrespective of the trade size (assuming that trade size is always less than pool size).
        * Purchase of asset X increases the price of X and decreases the price of Y
        * The ratio of assets X and Y sets the price
    * Now, What is a Protocol?
      * Protocols are basic sets of rules that allow data and cryptocurrencies to be shared securely between different nodes (i.e computers) in the blockchain network.
    - Pros of an AMM:
        * No Order Book Maintenance for traders but arbitrage is required for them.
        * A simple implementation of Constant Product AMM causes less computation which results in Low gas costs.
    - Cons of an AMM:
        * The danger of Impermanent loss/Coin De-Pegg may cause a total possible loss of funds in Liquidity Pools.
        * High slippage for low liquidity markets. So, please do observe and set your slippage tolerance threshold level while trading.
 
 **Liquidity Pool**        
- Liquidity Pool and its Working:-
  * A Liquidity Pool is a collection of two asset pairs X and Y (Let’s say for example in the case of Constant Product AMM), funded by Liquidity Providers(LP), that are locked in a smart contract, to facilitate trading, borrowing, lending, yielding, etc.
  * It ensures that buy and sell orders are carried out no matter the time of the day and at whatever price you want to trade without looking for any direct counterpart(as in the case of Order Book) as AMM ensures this. Hence, we won’t need to find a seller to buy a token. All that is needed is sufficient liquidity in the pool.
  * When a token swap occurs, the AMM ensures that the price adjusts based on its algorithm. The algorithm ensures that there is always liquidity in the pool, no matter the trade size. 
  * For eg., A liquidity pool is, by default, a 50:50 ratio of 2 coins. Let's say 50% dai (DAI) and 50% ether (ETH). When you buy DAI with ETH, the pools will start to lose DAI and get more ETH. The algorithm increases the price of dai and lowers the price of ether to keep the ratio regulated. The process is a self-regulated automated reaction to the market's needs.  
 
 **Profit and Loss incurr by Liquidity Providers(LP) on AMM DEXs**        
- Types of rewards that Liquidity Providers get on funding Liquidity Pools are:
  - Trading Fees reward: that are paid by traders on each trade( eg, 0.03% in Curve.fi )
  - Liquidity Mining reward:
    * It is an incentive/reward given to the Liquidity Providers(LP) proportional to the amount of liquidity provided by the LP
    * It can also be provided to the LPs in terms of “Airdrops”.
    * Airdrops are tokens that are given to the traders and LPs for free or in exchange for minimal promotional work.
- Types of losses for Liquidity Providers:
  - Impermanent loss == Not Permanent Loss
    * Impermanent Loss arises when the price ratio of an asset and liquidity pool changes. So, Liquidity Providers (LPs) who have deposited funds in affected pools automatically incur this loss. The larger the shift in the price ratio the larger the loss.
    * However, this loss is called impermanent for a reason as long as we do not withdraw deposited tokens at a time that the pool is experiencing a shift in price ratio it is still possible to mitigate the loss.
    * This loss disappears when the prices of the tokens revert to the original value at which they were deposited.
    * Those who withdraw funds before the prices revert suffer permanent losses.
    - Nonetheless, it is possible to negate the losses through income received by liquidity providers via:
      * Trading fees (i.e fees taken from traders during each trading transaction).
      * Liquidity mining reward (i.e reward given by the DEX in the form of its governance tokens or some other asset as interests).
  - Coin de-peg:
    * De-pegging refers to the phenomenon of a stablecoin deviating or any asset deviating from its intended peg. For example: In the case of a stablecoin pegged to USD, if its value reduces below $1, then the coin is said to be “de-pegged” which indirectly reduces the valuation of investment to a Liquidity Pool by a Liquidity Provider.
 
 **Profit and Loss incurr by Traders on AMM DEXs**        
* How traders are making profits using AMM?
  - Arbitrage:
    * It is an investment strategy in which an investor (a.k.a. Arbitrageurs) simultaneously buys and sells the same asset in different markets(either AMM or some other market) to profit from tiny differences in the asset's listed price.
  - Flash Swaps or Capital Free Arbitrage (used in Uniswap):
    * It allows us to withdraw up to the full reserves of any ERC20 token on Uniswap and execute arbitrary logic at no upfront cost, provided that by the end of the transaction you either:
      * Pay for the withdrawn ERC20 tokens with the corresponding pair tokens
      * Return the withdrawn ERC20 tokens along with a small fee
* One thing that causes the most loss to traders:-
  - Slippage:
    * The featured price of a cryptocurrency on a marketplace is the most recent price at which that cryptocurrency was bought by the buyer or sold by the seller. So in some cases where there are not enough counter-parties to trade with, then the market is said to be illiquid or prone to slippage.
    * It occurs when the processing of large order volumes drives the prices of an asset up or down to mitigate this occurrence and this fluctuation of price is called volatility.
    * In other words, Slippage is the difference between the expected price of an order and the price when the order executes. ( due to the volatility of cryptocurrency prices )
    * For solving this illiquidity or slippage problem of the market we need liquidity which is provided by Liquidity Providers (or Market Makers) to make Liquidity Pools liquid again and this whole process is called Market Making.
      
 
 **DEX Aggregator**        
- DEX Aggregators:
  DEX Aggregators are financial protocols that enable cryptocurrency traders to access a range of trading pools from a single dashboard (i.e Aggregates different Liquidity Pool prices at one Place).
  - Types of Aggregators:-
    - Off-chain Aggregator ( like 1inch, paraswap )
      * (+) Can swap multiple chains flexibly present over 4+ exchanges
      * (-) An operator can front-run users
    - On-chain Aggregator ( like swapswap )
      * (+) used for arbitrage findings
      * (-) unlikely to efficiently cover 4+ exchanges
 
 

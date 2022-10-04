## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Decentralised Exchanges
 
 **Introduction**        
### What is an Exchange?
  An exchange is a marketplace or platform where securities (such as stocks, bonds, preferred shares, ETFs, etc.), commodities, derivatives, and other financial instruments are traded (i.e buying and selling among customers). 
  An exchange's primary duty is to ensure fair and orderly trading as well as the efficient broadcast of price information for any securities traded on that exchange. Exchanges provide a forum for firms, governments, and other organizations to offer securities to the investing public. 
  An exchange can be either a physical facility where traders gather to do business or an electronic platform. Most countries throughout the world have their own exchanges. The New York Stock Exchange (NYSE), Nasdaq, National Stock Exchange(India), London Stock Exchange (LSE), and Tokyo Stock Exchange are among the more notable exchanges (TSE).
  Exchanges can be subdivided: 
  - By objects sold or traded: Stock exchange, Crypto exchange, Commodities exchange, or Foreign exchange market. 
  - By type of trade: Classical exchange, Future & Options exchange.

  Let us dive into crypto exchanges.

### What is a Crypto Exchange?
  Crypto or cryptocurrency or digital-currency exchange is a marketplace or platform which allows customers to trade cryptocurrencies for other assets, such as conventional fiat money(eg: U.S. Dollar, Japanese Yen, Euro, etc.) or other digital currencies.
  On a crypto exchange, you can use ordinary fiat currency to buy crypto, or you may be able to trade one crypto for another. You may be able to convert your crypto back into regular currency, leave it in your account for future trades, or withdraw it as cash. They display the current market value of the cryptocurrencies they provide. Available services can vary, depending on the exchange or app you use. For example, some services don't allow you to move your crypto off platform to your own crypto wallet. Unlike traditional exchanges that have set trading hours, cryptocurrency exchanges are active 24 hours a day, 7 days a week.
  
  In addition to trading services, crypto exchanges provide price discovery through trading activity and crypto storage. Prior to crypto exchanges, consumers could only obtain cryptocurrency through mining or organizing transactions in various online and offline communities.

  There are Centralized and Decentralized Cryptocurrency Exchanges, and each offers advantages and disadvantages.
 
 **Types of Crypto Exchange**        
### Traditional or Centralized Exchange (CEX):
  A centralized exchange is a peer-to-exchange-to-peer marketplace where transactions between crypto traders are done using traditional “Order Book” models that are officiated by banks, brokers, or any other intermediary. Centralized cryptocurrency exchanges serve as a middleman between buyers and sellers and generate revenue through commissions and transaction fees. You may think of a CEX as a stock exchange for digital assets.
  Coinbase, Crypto.com, Gemini, and Binance are well-known cryptocurrency exchanges. These exchanges let cryptocurrency investors buy and sell digital assets at the current price, known as spot, or leave orders that get executed when the asset reaches the investor's preferred price objective, known as limit orders, in a manner similar to stock trading websites or applications.
  Exchanges choose which digital assets to allow trading in, providing some reassurance that dishonest digital assets may be barred. They also set exchange rules and fees as well as store customer data (such as KYC) and transactional data.
  Since one of the core principles of cryptocurrencies is that they are decentralized, or not issued or regulated by a government or other central body, this may seem nonsensical. However, a centralized cryptocurrency exchange might make it simpler to purchase the cryptocurrency you want using fiat money.
  Some centralized exchanges may be more susceptible to assault because they are held by a single party, which poses a potential risk.

### What is an Order Book?
  An order book is a price-level-organized electronic list of purchase and sell orders for a given asset or financial instrument. An order book records the number of shares bid or offered at each price point, often known as market depth. As a result, the price of a digital asset will be determined by the supply and demand for that asset in comparison to another, whether it be a fiat currency or cryptocurrency.
  It also reveals the market participants responsible for the purchase and sell orders, while some prefer to remain anonymous. Because they give valuable trading information, these listings benefit traders and increase market transparency. This data can provide valuable information about potential support and resistance levels.
  Almost every exchange uses order books to list orders for various assets such as equities, bonds, currencies, and even cryptocurrencies such as Bitcoin. These orders might be either manual or digital in nature.
  Some exchanges, called dark pools, have order books that aren't visible to the public.

  ![Order Book](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/1inch.png?raw=true)
  `Reference: https://medium.com/stabletrade/understanding-order-books-orders-b297ea51acff`
  There are two types of CEX based on the order book model, there might be further ones but let's just discuss the two basic components here:

### Server Order Book model
  In centralized exchanges which use the server order book model, all the customers' trading data, prices, and volumes of securities are stored in a Centralized Server. 
  The server order book model has its own advantages such as it supports faster trade matching and settlements which is great as speed is very important in financial settlements.
  In the case of canceled orders, no fees are deducted from the user's account which increases the ease of use as the user can place as many orders and cancel them at will.
  There are also a few drawbacks to this model.
  Since all data is stored on a centralized server and this centralized server is totally controlled by the exchange, there is no censorship resistance. The exchange operators can front-run customers due to low transparency. Suppose you have placed an order but the exchange decides to put some other orders before your order to profit from them, you as a user can do nothing about it as you will never know what happened and might even suffer losses in such a case.

### Onchain Order Book model
  In an on-chain order book model, all the customers' trading data, prices, and volumes of securities are stored on a Blockchain. Thus, there is no central server is involved in this case which results in a high level of transparency. It provides censorship resistance, as all data are stored on a distributed, and decentralized ledger in the form of immutable data blocks on the blockchain which are publicly shared among all its network nodes. The smart contract is written in a way that nobody else can censor the protocol, there are no admin keys, and so on.
  Since the blockchain is running much more reliably than a server, this model is relatively robust, so obviously you will have to pay more fees in exchange for that.
  This leads us to a few drawbacks which are, presumably, slow trade matching and settlement due to blockchain scalability issues. So, the slower your blockchain confirmation latency, the slower the entire system works.
  Naturally, for any blockchain transaction, you must pay a fee, even if you just want to cancel your order. Thus, fees are deducted in the form of Gas Fees for both successful and canceled orders so you might end up paying double the fees in case of cancellation (once for creating the order and again for canceling it).
  Even in this model, there is a slight risk of front-running the users by miner/trader/exchange operator.
 
 **Decentralized Exchange (DEX)**        
A decentralized exchange is another sort of exchange that permits peer-to-peer transactions straight from your digital wallet without the use of an intermediary. Uniswap, PancakeSwap, dYdX, and Kyber are a few DEXs. These decentralized exchanges are powered by blockchain-based smart contracts, which are self-executing bits of code. Compared to a centralized exchange, these smart contracts provide better privacy and less slippage (another term for transaction charges). However, even though smart contracts are based on regulations, the lack of a middleman leaves the user on their own, making DEXs appropriate only for experienced investors. In a way, they increase complexity for users as users must remember their crypto wallet keys and passwords, or their funds will be lost permanently and cannot be recovered. In contrast to centralized exchanges, which provide a more convenient and user-friendly process, they require the user to understand and become acquainted with the platform and the process. Also, these exchanges are best suited for investors wishing to transition from one digital asset to another, but not for those looking to purchase or sell digital assets with fiat currency, a process known as on and off-ramping. It makes them less appealing to users who do not already own cryptocurrency.
Decentralized exchange users are not required to transfer their assets to a third party. As a result, there is no possibility of a firm or organization being hacked, and users are guaranteed enhanced protection against hacking, failure, fraud, or theft. Customer, transactional, and all other forms of data are stored on Blockchain. Thus DEXs reduce market manipulation by enabling peer-to-peer cryptocurrency exchange, protecting customers against false trading and wash trading. Users benefit from privacy and anonymity since decentralized exchanges do not need clients to fill out know-your-customer (KYC) forms. Because DEXs are not censored, more cryptocurrencies and digital assets are available than through a CEX. In fact, several Altcoins are exclusively available on DEXs.
Centralized exchanges facilitate almost 99% of crypto transactions, implying that they are responsible for the majority of trade volume, making it challenging to locate buyers and sellers on decentralized exchanges due to frequent liquidity issues and low trading volumes.

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
Now we'll be discussing automated market maker (amm). These are the most popular form of decentralized exchanges on DeFi and they've really helped DeFi to grow significantly in size due to their ideal design for the low throughput blockchains as well as for the higher throughput blockchains.
AMM is basically a type of DEX protocol that relies on a mathematical formula that allows digital assets to be traded without permission, automatically by using liquidity pools instead of the traditional order book pricing model. This formula can vary with each protocol. For example, Uniswap uses the Constant Product AMM protocol which is as follows:
Asset X quantity * Asset Y quantity = K (a constant)  simply  X*Y=K
Properties of popular Constant Product AMM protocol:
  * Instant liquidity, irrespective of the trade size (assuming that trade size is always less than pool size).
  * Purchase of asset X increases the price of X and decreases the price of Y
  * The ratio of assets X and Y sets the price
![Automated Market Maker](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/amm.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`
Now, What is a Protocol?
Protocols are basic sets of rules that allow data and cryptocurrencies to be shared securely between different nodes (i.e computers) in the blockchain network.
- Pros of an AMM:
  * No Order Book Maintenance for traders but arbitrage is required for them.
  * A simple implementation of Constant Product AMM causes less computation which results in Low gas costs.
- Cons of an AMM:
  * The danger of Impermanent loss/Coin De-Pegg may cause a total possible loss of funds in Liquidity Pools.
  * High slippage for low liquidity markets. So, please do observe and set your slippage tolerance threshold level while trading.
 
 **Liquidity Pool**        
A Liquidity Pool is a collection of two asset pairs X and Y (Let’s say for example in the case of Constant Product AMM), funded by Liquidity Providers(LP), that are locked in a smart contract, to facilitate trading, borrowing, lending, yielding, etc.
It ensures that buy and sell orders are carried out no matter the time of the day and at whatever price you want to trade without looking for any direct counterparty(as in the case of Order Book) as AMM ensures this. Hence, we won’t need to find a seller to buy a token. All that is needed is sufficient liquidity in the pool.
When a token swap occurs, the AMM ensures that the price adjusts based on its algorithm. The algorithm ensures that there is always liquidity in the pool, no matter the trade size. 
For eg: A liquidity pool is, by default, a 50:50 ratio of 2 coins. Let's say 50% dai (DAI) and 50% ether (ETH). When you buy DAI with ETH, the pools will start to lose DAI and get more ETH. The algorithm increases the price of dai and lowers the price of ether to keep the ratio regulated. The process is a self-regulated automated reaction to the market's needs.

![Liquidity Pool](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/liquidity-pool.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`
 
 **Profit and Loss incurr by Liquidity Providers(LP) on AMM DEXs**        
Types of rewards that Liquidity Providers get on funding Liquidity Pools are:
### Trading Fees
Incentive or reward in terms of trading fees that are paid by traders to the Liquidity Providers on each trade they undertake.
The way that this works is the trading fees value is directly added into the pool so as such the liquidity providers they have an LP coin which represents the share of the allocation in this pool and because this pool is growing through trading fees the share of the pool remains the same, relatively speaking. But the absolute value of the of the pool obviously grows and therefore the LP coins grow in value through the addition of trading fees. An example in Curve.fi is that the LPs they get 0.03 of the trading fees from the users. So in essence you if you're participating as a liquidity provider in a pool you are gaining interest on based on the user behavior so the more users trade the more financial value you will receive.
### Liquidity Mining
Liquidity mining can be seen as being equal to an incentive that's created for participants to participate in a particular defi protocol. It is a reward given to the Liquidity Providers(LP) proportional to the amount of liquidity provided by them.
It can also be provided to the LPs in terms of “Airdrops”. Airdrops are tokens that are given to traders and LPs for free or in exchange for minimal promotional work.
These are rewards that any DeFi protocol can manually specify so they can for example say if you provide a certain amount of liquidity to a pool then the protocol (this is actually the the DeFi protocol i.e. instructors or developers) will basically give some token as a reward. So this is a liquidity mining reward and this incentive exists in order to incentivize liquidity providers to deposit more and more assets into a pool, hence attracting more liquidity and thud attracting more traders because the slippage becomes lower because the trading volume grows and volume attracts volume in the exchange businesses.

Now, Let's discuss the types of losses for Liquidity Providers :
### Impermanent loss
Impermanent loss is an often overlooked risk when providing liquidity to an amm but it's rather simple let's dive into it.
Impermanent loss basically means Not Permanent Loss. Impermanent Loss arises when the price ratio of an asset and liquidity pool changes. So, Liquidity Providers (LPs) who have deposited funds in affected pools automatically incur this loss. The larger the shift in the price ratio the larger the loss. However, this loss is called impermanent for a reason. As long as we do not withdraw deposited tokens at a time that the pool is experiencing a shift in price ratio it is still possible to mitigate the loss. This loss disappears when the prices of the tokens revert to the original value at which they were deposited. Those who withdraw funds before the prices revert suffer permanent losses. Nonetheless, it is possible to compensate the losses through income received by liquidity providers via Trading fees (i.e fees taken from traders during each trading transaction) and Liquidity mining reward (i.e reward given by the DEX in the form of its governance tokens or some other asset as interests).
Finding a solution to impermanent loss is not simple but quite challenging. A potential solution is to change to bonding cuve (the curve that governs the amm liquidity).
The image below provides an example of impermanent loss.
![Impermanent Loss](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/impermanent-loss.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`

### Coin de-peg:
De-pegging refers to the phenomenon of a stablecoin deviating or any asset deviating from its intended peg. For example: In the case of a stablecoin pegged to USD, if its value reduces below $1, then the coin is said to be “de-pegged” which indirectly reduces the valuation of investment to a Liquidity Pool by a Liquidity Provider.
 
 **Profit and Loss incurr by Traders on AMM DEXs**        
Now, Let us discuss how traders make profits using AMM?:-
### Arbitrage
Arbitrage is an investment strategy in which an investor (a.k.a. Arbitrageurs) simultaneously buys and sells the same asset in different markets to profit from tiny differences in the asset's listed price. Arbitrage is the practice by which different prices on various exchanges or markets become synchronized. These markets could be either AMM or some other market.
Naturally this requires to perform at least one transaction. So either you could only want to perform an arbitrage transaction on a single market but this is under the assumption that you already own some of the coins (Let’s say x and y) which you will swap and maybe you want to replenish your portfolio. But typically an arbitrage is done by having one transaction that either purchases an asset on one market and other sells the asset on another. These two actions are swap actions and they can be all done in a single transaction ideally. 

Below is an pictorial example of arbitrage.
![Arbitrage](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/arbitrage.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`
### Flash Swaps or Capital Free Arbitrage 
Used in Uniswap, It allows us to withdraw up to the full reserves of any ERC20 token on Uniswap and execute arbitrary logic at no upfront cost, provided that by the end of the transaction you either:
* Pay for the withdrawn ERC20 tokens with the corresponding pair tokens
* Return the withdrawn ERC20 tokens along with a small fee

One thing that causes the most loss to traders:
### Slippage
The featured price of a cryptocurrency on a marketplace is the most recent price at which that cryptocurrency was bought by the buyer or sold by the seller. So in some cases where there are not enough counter-parties to trade with, then the market is said to be illiquid or prone to slippage.
It occurs when the processing of large order volumes drives the prices of an asset up or down to mitigate this occurrence and this fluctuation of price is called volatility.
In other words, Slippage is the difference between the expected price of an order and the price when the order executes. ( due to the volatility of cryptocurrency prices )
For solving this illiquidity or slippage problem of the market we need liquidity which is provided by Liquidity Providers (or Market Makers) to make Liquidity Pools liquid again and this whole process is called Market Making.
![Slippage](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/slippage.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`
      
 
 **DEX Aggregator**        
We have looked at decentralized exchanges in isolation, but now we we're going to look at how to aggregate or merge them together.
DEX Aggregators are financial protocols that enable cryptocurrency traders to access a range of trading pools from a single dashboard. Users really are interested in the deepest liquidity in order to pay the lowest slippage on their trades. So the exchange aggregators source liquidity from all the different exchanges and merge them so that the user only has to access a single dashboard to exchange their assets and then the exchange aggregator find the best liquidity, the lowest prices, lowest commissions etc as per user’s interest. 

There are overall two types of aggregators that are currently prevalent they're so-called off-chain aggregators and on-chain aggregators. 
### Off-chain Aggregators
Off-chain Aggregators like 1inch, paraswap are websites where you can go and you have your browser wallet or your crypto wallet activated perform trades. They are quite flexible, that means you can perform trades across multiple chains efficiently instead of just a single chain. They are also very quick in determining the optimal trade. The disadvantage of such aggregators is that operators can front run users because the operator is a trusted third person here which is in the middle between the exchange and the user. The off chain aggregation is typically performed off-chain as the name suggests so the computation of the trait with the optimal parameters is not performed on chain and can therefore not always be optimal.

Let's discuss about 1inch. The UI of of one inch is really beautifully verbose, you can see a lot of data, you can analyze which markets might be better, also choose to go directly to these websites right if you want to pay a less gas price for instance. So it's quite intuitive and flexible. For example to exchange Ether and DAI you input the amount that you would like to exchange so it will also show you a list of the various exchanges where you can perform this trade right. It actually explains you which route is taken for your swap. There might be more complicated routes that emerge depending on the swap that you're enacting. Your trade might also open up an arbitrage opportunity since you're you're swapping assets and you're changing liquidity on one exchange so there will be another market where there's an arbitrage opportunity created due to your swap.
![1inch](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/1inch.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`
### On-chain Aggregators
Then there are on-chain aggregators like swapswap is an example of this. They are much less famous at the moment than than off-chain aggregators but they do have some key advantages, for example, they allow you to perform atomic routing and arbitrage which is provably optimal on-chain. The smart contract basically does everything for the user and there is no middleman. There is basically a very small likelihood of being front run so it's technically a little bit safer however they don't scale as much as the off-chain variants so they're unlikely to efficiently cover many more exchanges in parallel like the off-chain aggregators.

SwapSwap is a recent emerging on-chain aggregator which aggregates two DEXs so that's not much but it's a beginning so you have UniSwap and SushiSwap that's being aggregated. There's no particular UI change for the user so you have here a standard Uniswap UI. You do not really see at the moment like what financial advantages you get out of this aggregator but in theory you should get better prices than on Uniswap and Sushiswap since you're aggregating the liquidity together. The beautiful thing is that it basically routes a swap if the smart contract deems this to be profitable. So the smart contract will decide at execution time whether this should be now routed or not and it does perform arbitrage with flash loans so it does not leave money on the table. So if profitable it will create even a flash loan for you on the fly ,transparently, in the background and perform all this in the smart contract.
![SwapSwap](https://github.com/DoDAO-io/dodao-defi-course/blob/89865af46df4e3e877a8c216dd04b63c48ba23a2/images/swapswap.png?raw=true)
`Reference: https://berkeley-defi.github.io/assets/material/Updated%20Lecture%205%20Slides.pdf`

So next time you hit an exchange think about maybe visiting some aggregators, checking the prices there maybe they are cheaper maybe not and just try around a little bit too especially if you want to exchange larger amounts.
 
 

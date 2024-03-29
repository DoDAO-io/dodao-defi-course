## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Lending and Borrowing
 
 **Lending**        
- What is Lending(also known as “financing”)?
  * Lending occurs when someone(here lender) allows another person to borrow something (such as Money, property, or another asset) with the expectation that the borrower will either return the asset or repay the lender with some interest.
  * We all are currently learning DeFi, so let’s see On-Chain Lending and Borrowing(i.e Credit):-      
  - Entities of Lending and Borrowing:-
    * Lender: Deposit Principal in the Liquidity Pool(or Vault) and gets back Principal with interest.
    * Borrower: Collateralize Assets and get back the borrowed amount
    * Liquidator: Liquidates the crypto collateral assets when a borrower defaults or when the Loans become unsafe due to the volatility in token prices.
    * Price Oracle: Report prices or send exact prices of assets from different sources(either centralized or decentralized) to the Protocol.
 
 **Lending Terminology**        
- Collateral: 
  * An asset that serves as a security deposit on the debt taken.

- Over-collateralization:
  * When the value of collateral assets exceeds the value of the granted loan then it is called an Over-collateralized loan. 

- Under-collateralization:
  * When the value of collateral assets is below the value of the granted loan then it is called an Under-collateralized loan.

- Liquidation: 
  * Selling collateral assets of a borrower is called Liquidation.
  
- Health Factor (In detail):
  * Health Factor = Borrowing Capacity / Total Value of Debts
  * Borrowing capacity is the summation of all the values of the collateral we have, times a `liquidation threshold`
    0 < liquidation threshold < 1 (Range)
  * The liquidation threshold provides a “secure” margin
  * When the health factor declines below 1, a borrowing position becomes liquidatable
 
 **Collateralization**        
- Collateralization:
  * It is the process of securing a loan with a valuable asset(a.k.a Collateral) by the loan borrower. There are two types of Collateraliztion:-

  - Over-collateralization:
    - In this, the borrower has to provide:
      * value(collateral assets) > value(debt or granted loan) 
      * It means they allow to borrow less than the collateralize amount
      * But allows the borrower to freely use their funds which they get as a loan
    - Let's say a borrower collateralizes ETH and borrows DAI
      * The value of ETH (collateral) exceeds the value of DAI (debt)
      * Now, the borrower can use the borrowed DAI arbitrarily/freely

  - Under-collateralization:
    - In this, the borrower has to provide
      * value(collateral assests) < value(debt or granted loan)
      * It means they allow to borrow more than the collateralize amount
      * But they highly restrict the borrower to use their funds as they don't get their borrowed funds immediately as smart contracts manage how a borrower can use money
    - Let's say a borrower collateralizes ETH and borrows DAI
      * The value of DAI (debt) can exceed the value of ETH (collateral)
      * The collateralized ETH and borrowed DAI are restricted to be used with pre-designed smart contracts. Those are typically farming contracts.
      * The vault remains in control of all assets.
 
 **Liquidation**        
-Liquidation:
  * Liquidation == Selling collateral from the borrower
  * Liquidators/Anyone can liquidate the collateralized asset in return for an incentive (in the form of an opportunity to purchase the collateralize asset at a lower value than the market)
    * If value(collateral assets) <= 150% * value(debt or granted loan)   (...for example)
  * There may also be auctions for liquidating the collateralized asset whose value is degraded.
  - Liquidation Insights:
    - Health Factor:
      * A Fixed Spread liquidation does not necessarily increase the health factor
    - Close Factor (CF): 
      * The maximum proportion of the debt that is allowed to be repaid in a fixed spread liquidation
      * Value of Debt to Repay < ( Close Factor * Total Value of Debt )
    - Over-liquidation:
      * Liquidations sell excessive amounts of borrower's collateral
    - Optimal Liquidation Strategy:
      * Liquidating up to the close factor is not necessarily the best strategy.
      * Instead, two successive liquidations might offer more profits.
    - Data suggests:
      * Auction liquidations might be more borrower-friendly
 
 **Liquidation Spread (LS)**        
- Liquidation Spread (LS):
  * It is the spread/range of bonus, or discount, that a liquidator can collect when liquidating collateral.
  * Value of Collateral to Claim = Value of Debt to Repay * (1 + LS)
  * Two types of Liquidation based on Liquidation Spread:-
  - Fixed Spread:
    * With fixed spread liquidation, a liquidatable loan can be instantly liquidated at a pre-determined discount.
    * This discount, or liquidation spread incase of Fixed Spread model, is known upfront, which allows liquidators 
      to locally decide whether to engage in a liquidation opportunity.
    * This avoids hour-long liquidation auctions, which cost time and transaction fees.
    * Different protocols follow different liquidation models. MakerDAO, for example, uses an auction-based system, while Aave, Compound, and dYdX have fixed spread models.
    * In this, the Liquidator does both settlements in one Blockchain transaction such as:
      * Repays the debt of a borrowing position to Vault
      * And Acquires the collateral at a discounted price from the position in return. 
        * Eg. Typical discounts can lie between 5-15% in the case of Aave.
  - Variable (or Auction Based) Spread:
    * In this, various liquidators bid over time until the auction terminates and this process requires multiple blockchain transactions.
    * Types of Auction Liquidation:
      - English Auction:
        * In this, Bidders outbid each other increasingly
      - Dutch Auction:
        * This, Auction begins with a high asking price and the price lowers until the auction terminates 
        * Eg, MakerDAO Dutch Auction:-
          - Instant Settlement:
            * Unlike the English auction which is operated in multiple transactions, the MAkerDAO Dutch auction is settled instantly in one atomic transaction.
          - Flash Lending of Collateral:
            * No upfront DAI (i.e, the debt or granted loan) is required (i.e., a flash loan used specifically for MakerDAO liquidations).
          - Price as a Function of Time:
            * Collateral price decreases over time and nobody can get the collateral for free by accident.
 
 **Flash Loans**        
- Definition:
  * Take loans(in a flash) —> Use them —> Repay loan + interest all in one single atomic blockchain transaction(eg, It takes 12-14 sec in the case of Ethereum Blockchain).
- Flash Loan Use Cases:
  - DeFi attacks:
    - Price Oracle Manipulation using an example:
      * Let's say an attacker takes out a flash loan on the incoming asset A and the relevant Uniswap pool, swap asset A for asset B with a large volume. Then, this trade will increase the price of asset B (increased demand) and reduce the cost of asset A (increased supply).
    - Pump and Dump: 
      * In this, an attacker takes a flash loan from one platform to split the loan between the other two lending platforms to pump the price of an asset in one and dump the price of an asset in another before returning the loan to the first lending platform in a single transaction.
  - (Risk-free) Arbitrage using flash loans.
  - Wash-trading:
    * In this, the borrower takes out a flash loan of Y tokens on DEX A, then execute two trades by swapping Y tokens for Z tokens on DEX B and vice-versa again on DEX B. This increases the trading volume for the Y tokens, creating an artificial level of interest and opportunity for profit. 
  - Flash Minting:
    * In this, attackers can mint an arbitrary number of new Flash-mintable tokens (a.k.a FMTs or ERC20-compliant tokens) into their account, as long as they also burn the same number of tokens from their account before the end of the same transaction to generate profits.
  - Collateral swapping:
    * It enables DeFi users to swap or switch the collateral asset that they used to take out a flash loan on a lending app. 
- Flash Loan Based Liquidation works:
  * When a liquidator does not have the cryptocurrency upfront to repay and has to complete liquidation in one transaction.
 
 **Over-colleteralized borrowing use cases**        
- Over-colleteralized borrowing seems to be not relevant initially as the amount of collateral needed to borrow the 
  tokens can be quite high. But there are many use cases for it.
  * **Yield Farming** - The process involves leveraging DeFi protocols to lend cryptocurrencies for high returns that can 
    go up to 100% APY (Annual Percentage Yield). Yield farming originates from banks’ process in lending your deposits; the difference 
    is that DeFi yield farming compounds the interest earned.
  * **Arbitrage** - Arbitrage takes advantage of the fact that an asset may be worth more in one market than another. While 
    this usually happens because of market inefficiencies, it can also be used to exploit differences in rates between 
    different platforms.
  * **Margin Trading (Leverage)** - Taking out a loan with extra collateral can help you gain leverage, and you can repeat 
    the process until you reach the limit.
  * **Liquidation** - Liquidations can be quite profitable, especially for tech-savvy traders. Usually, a liquidator has to 
    compete against other people for the same job, so he uses bots. They work by "sniping" the loans that are under the 
    collateralization ratio. This way, they can liquidate the collateral and reimburse the lender. In turn, the liquidator 
    receives a reward fee for his services.
  * **Risk-reduction/Hedging** - No matter how well you think you know the markets, there will always be bumps in the road. As 
    a trader, you need to find ways to protect your investment from risk, and this is where crypto hedging strategies come in. 
    Hedging encompasses opening positions in opposing market directions to reduce the risks and impacts of market swings. By doing this, 
    you can help to offset any potential losses that might occur.
 
 

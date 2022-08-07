## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Lending and Credit
 
 **Lending**        
- What is Lending(also known as “financing”)?
  * Lending occurs when someone(here lender) allows another person to borrow something (such as Money, property, or another asset) with the expectation that the borrower will either return the asset or repay the lender with some interest.
  * We all currently learning Decentralized Finance i.e Finance on a distributed, decentralized, and immutable ledger or data block. So, let's discuss On-Chain or Blockchain-based Lending and Borrowing:-
  - Entities of Lending and Borrowing:-
    * Lender: Deposit Principal in the Liquidity Pool(or Vault) and gets back Principal with interest.
    * Borrower: Collateralize Assets and get the back borrowed amount
    * Liquidator: Liquidates the Liquidity pool
    * Price Oracle: Report prices or send exact prices of assets from different sources(either centralized or decentralized) to the Protocol.
 
 **Lending Terminology**        

- Collateral: 
  * An asset that serves as a security deposit on the debt taken.

- Over-collateralization: 
  - The borrower has to provide
    * value(collateral assets) > value(granted loan) 
    * It means they allow to borrow less than the collateralize amount
    * But allows the borrower to freely use their funds which they get as a loan
    - Let's say a borrower collateralizes ETH and borrows DAI
      * The value of ETH (collateral) exceeds the value of DAI (debt)
      * Now, the borrower can use the borrowed DAI arbitrarily/freely

- Under-collateralization:
  - The borrower has to provide
    * value(collateral) < value(debt)
    * It means they allow to borrow more than the collateralize amount
    * But they highly restrict the borrower to use their funds as they don’t get their borrowed funds immediately as smart contracts manage how a borrower can use money
    - Let's say a borrower collateralizes ETH and borrows DAI
      * The value of DAI (debt) can exceed the value of ETH (collateral)
      * The collateralized ETH and borrowed DAI are restricted to be used with pre-designed smart contracts. Those are typically farming contracts.
      * The vault remains in control of all assets.


- Liquidation: 
  * Liquidation == Selling collateral from the borrower
  * Liquidators/Anyone can liquidate the collateralized asset in return for an incentive (in the form of an opportunity to purchase the collateralize asset at a lower value than the market)
    * If value(collateral) <= 150% * value(debt)   (...for example)
  * There may also be auctions for liquidating the collateralized asset whose value degraded.
  - Liquidation Insights:
    - Health Factor:
      * A Fixed Spread liquidation does not necessarily increase the health factor
    - Over-liquidation:
      * Liquidations sell excessive amounts of borrower’s collateral
    - Optimal Liquidation Strategy:
      * Liquidating up to the close factor is not necessarily the best strategy.
      * Instead, two successive liquidations might offer more profits.
    - Data suggests:
      * Auction liquidations might be more borrower-friendly


- Health Factor (In detail):
  * Health Factor = Borrowing Capacity / Total Value of Debts
  * Borrowing is the summation of all the values of the collateral we have, times a `liquidation threshold`
    0 < liquidation threshold < 1 (Range)
  * The liquidation threshold provides a “secure” margin
  * When the health factor declines below 1, a borrowing position becomes liquidatable

- Liquidation Spread (LS): bonus, or discount, that a liquidator can collect when liquidating collateral.
  * Value of Collateral to Claim = Value of Debt to Repay * (1 + LS)
  * Two types of Liquidation based on Liquidation Spread:-
  - Fixed Spread:
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
            * No upfront DAI (i.e, the debt) is required (i.e., a flash loan used specifically for MakerDAO liquidations).
          - Price as a Function of Time:
            * Collateral price decreases over time and nobody can get the collateral for free by accident.


- Close Factor (CF): the maximum proportion of the debt that is allowed to be repaid in a fixed spread liquidation
  * Value of Debt to Repay < CF * Total Value of Debt
 
 **Flash Loans**        
- Definition:
  * Take loans(in a flash)—> Use them—> Repay loan + interest all in one single atomic blockchain transaction(eg, It takes 12-14 sec in the case of Ethereum Blockchain).
- Flash Loan Use Cases:
  * DeFi attacks
  * Price Oracle Manipulation
  * Pump and Dump
  * (Risk-free) Arbitrage
  * Wash-trading
  * Flash Minting
  * Collateral swapping
- Flash Loan Based Liquidation works:
  * When a liquidator does not have the cryptocurrency upfront to repay and has to complete liquidation in one transaction.
 
 

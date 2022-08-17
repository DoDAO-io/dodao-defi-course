## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Lending and Credit
 
 
---

##### Who deposits Principal in the Liquidity Pool(or Vault) to get back the Principal with interest as profit?  

- [x]  Lender
- [ ]  Borrower
- [ ]  Liquidator
- [ ]  Price Oracle
  
Hint: Lending
         
Explanation: Lender deposits Principal in the Liquidity Pool(or Vault) and gets back Principal with interest.

Sub Topics: lending-intro
 

---

##### What is the role of Price Oracle?  

- [ ]  Change prices of assets from different sources(only decentralized) to the Protocol.
- [ ]  Report prices of assets from different sources(only decentralized) to the Protocol.
- [x]  Report prices of assets from different sources(either centralized or decentralized) to the Protocol.
- [ ]  Change prices of assets from different sources(either centralized or decentralized) to the Protocol.
  
Hint: Reports the prices
         
Explanation: Price Oracle reports the prices or send exact prices of assets from different sources(either centralized or decentralized) to the Protocol.

Sub Topics: lending-intro
 

---

##### Who liquidates the Liquidity pool?  

- [ ]  Lender
- [ ]  Borrower
- [x]  Liquidator
- [ ]  Price Oracle
  
Hint: NoHint
         
Explanation: Liquidator liquidates the Liquidity pool

Sub Topics: lending-intro
 

---

##### Lending is also known as?  

- [ ]  Liquidation
- [x]  Financing
- [ ]  Price Oracle
- [ ]  Vaulting
  
Hint: NoHint
         
Explanation: explanation

Sub Topics: lending-intro
 

---

##### What is a collateral?  

- [ ]  Reported price of an asset
- [x]  An asset that serves as a security deposit on the debt taken
- [ ]  Interest amount gained on the Principal
- [ ]  Total value of debts
  
Hint: Asset
         
Explanation: Collateral is an asset that serves as a security deposit on the debt taken.

Sub Topics: terminology
 

---

##### Selling collateral assets of a borrower is known as?  

- [ ]  Collateralization
- [ ]  Under-collateralization
- [ ]  Over-collateralization
- [x]  Liquidation
  
Hint: NoHint
         
Explanation: Selling collateral assets of a borrower is called Liquidation.

Sub Topics: terminology
 

---

##### When is a loan considered Under-collateralized?  

- [ ]  When the value of collateral assets exceeds the value of the granted loan
- [x]  When the value of collateral assets is below the value of the granted loan
- [ ]  When the value of collateral assets is equal to the value of the granted loan
- [ ]  When the value of collateral assets is double the value of the granted loan
  
Hint: Under is similar to ...
         
Explanation: When the value of collateral assets is below the value of the granted loan then it is called an Under-collateralized loan.

Sub Topics: terminology
 

---

##### Which of the following is equal to Health Factor?  

- [x]  Borrowing Capacity / Total Value of Debts
- [ ]  Borrowing Capacity * Total Value of Debts
- [ ]  Borrowing Capacity + Total Value of Debts
- [ ]  Borrowing Capacity - Total Value of Debts
  
Hint: NoHint
         
Explanation: Health Factor = Borrowing Capacity / Total Value of Debts

Sub Topics: terminology
 

---

##### Which of the following is the correct range of liquidation threshold?  

- [ ]  0 < Liquidation Threshold < 10
- [ ]  -1 < Liquidation Threshold < 1
- [ ]  -1 < Liquidation Threshold < 0
- [x]  0 < Liquidation Threshold < 1
  
Hint: Can not be negative
         
Explanation: Range of Liquidation threshold is (0,1).

Sub Topics: terminology
 

---

##### When does a borrowing position become liquidatable?  

- [x]  When the health factor declines below 1
- [ ]  When the health factor increases above 1
- [ ]  When the liquidation threshold declines below 1
- [ ]  When the liquidation threshold increase above 1
  
Hint: Health Factor
         
Explanation: When the health factor declines below 1, a borrowing position becomes liquidatable

Sub Topics: terminology
 

---

##### The process of securing a loan with a valuable asset by the loan borrower is known as  

- [ ]  Under-collateralization
- [x]  Collateralization
- [ ]  Over-collateralization
- [ ]  Liquidation
  
Hint: NoHint
         
Explanation: Collateralization is the process of securing a loan with a valuable asset (a.k.a Collateral) by the loan borrower

Sub Topics: collateralization
 

---

##### The summation of all the values of the collateral we have, times a `liquidation threshold` is known as?  

- [ ]  Liquidation
- [ ]  Collateralization
- [x]  Borrowing capacity
- [ ]  Health Factor
  
Hint: NoHint
         
Explanation: Borrowing capacity is the summation of all the values of the collateral we have, times a `liquidation threshold`.

Sub Topics: terminology
 

---

##### Let's suppose a borrower collateralizes ETH and borrows DAI. Which of the following statements is true for Over-collateralization?  

- [x]  The value of ETH (collateral) exceeds the value of DAI (debt)
- [ ]  The value of DAI (debt) can exceed the value of ETH (collateral)
- [x]  The borrower can use the borrowed DAI arbitrarily/freely
- [ ]  The borrower can not use the borrowed DAI arbitrarily/freely
  
Hint: Not strict
         
Explanation: In Over-collateralization, the borrower has to provide value(collateral assets) > value(debt or granted loan). It means they allow to borrow less than the collateralize amount. But allows the borrower to freely use their funds which they get as a loan

Sub Topics: collateralization
 

---

##### The vault remains in control of all assets in case of  

- [ ]  Over-collateralization
- [ ]  Over-Liquidation
- [ ]  Under-Liquidation
- [x]  Under-collateralization
  
Hint: Restricted
         
Explanation: In Under-collateralization, the borrower is highly restricted to use their funds. The vault remains in control of all assets.

Sub Topics: collateralization
 

---

##### Pick the correct statement.  

- [ ]  Value of Debt to Repay = (Close Factor * Total Value of Debt)
- [x]  Value of Debt to Repay < (Close Factor * Total Value of Debt)
- [ ]  Value of Debt to Repay > (Close Factor * Total Value of Debt)
- [ ]  Value of Debt to Repay >= (Close Factor * Total Value of Debt)
  
Hint: NoHint
         
Explanation: Value of Debt to Repay is always less than the product of Close Factor and Total Value of Debt.

Sub Topics: collateralization
 

---

##### What do you mean by Close Factor?  

- [ ]  The minimum proportion of the debt that is allowed to be repaid in a fixed spread liquidation
- [ ]  The minimum proportion of the debt that does not need to be repaid.
- [ ]  The maximum proportion of the debt that does not need to be repaid.
- [x]  The maximum proportion of the debt that is allowed to be repaid in a fixed spread liquidation
  
Hint: Maximum
         
Explanation: The maximum proportion of the debt that is allowed to be repaid in a fixed spread liquidation.

Sub Topics: liquidation
 

---

##### Choose the Optimal Liquidation Strategy.  

- [ ]  Liquidating up to the close factor
- [x]  Two successive liquidations
- [ ]  Both of the above
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: Liquidating up to the close factor is not necessarily the best strategy. Instead, two successive liquidations might offer more profits.

Sub Topics: liquidation
 

---

##### Select the one word substitute for - "Selling collateral from the borrower"  

- [x]  Liquidation
- [ ]  Collateralization
- [ ]  Lending
- [ ]  Factorization
  
Hint: NoHint
         
Explanation: Liquidation == Selling collateral from the borrower

Sub Topics: liquidation
 

---

##### Select the correct option.  

- [ ]  A Fixed Spread liquidation necessarily increases the health factor
- [x]  A Fixed Spread liquidation does not necessarily increase the health factor
- [ ]  A Fixed Spread liquidation necessarily decreases the health factor
- [ ]  A Fixed Spread liquidation doubles the health factor
  
Hint: NoHint
         
Explanation: A Fixed Spread liquidation does not necessarily increase the health factor.

Sub Topics: liquidation
 

---

##### Data suggests that Auction liquidations might be more lender-friendly. True or False?  

- [ ]  true
- [x]  false
  
Hint: Borrower
         
Explanation: Data suggests that Auction liquidations might be more borrower-friendly.

Sub Topics: liquidation
 

---

##### What is Liquidation Spread?  

- [ ]  It is the process of securing a loan with a valuable asset by the loan borrower
- [ ]  It is the process of selling collateral assets of a borrower
- [x]  It is the spread/range of bonus, or discount, that a liquidator can collect when liquidating collateral
- [ ]  It is the spread/range of bonus, or discount, that a liquidator can not collect when liquidating collateral
  
Hint: Definition of Liquidation Spread
         
Explanation: Liquidation Spread (LS) is the spread/range of bonus, or discount, that a liquidator can collect when liquidating collateral.

Sub Topics: liquidation-spread
 

---

##### Select the incorrect option(s).  

- [x]  Value of Collateral to Claim = Value of Debt to Repay * (1 - LS)
- [ ]  Value of Collateral to Claim = Value of Debt to Repay * (1 + LS)
- [ ]  Value of Debt to Repay = Value of Collateral to Claim / (1 + LS)
- [x]  Value of Debt to Repay = Value of Collateral to Claim * (1 + LS)
  
Hint: NoHint
         
Explanation: Value of Collateral to Claim = Value of Debt to Repay * (1 + LS).

Sub Topics: liquidation-spread
 

---

##### Two types of Liquidation based on Liquidation Spread are-  

- [x]  Fixed Spread
- [ ]  Over Spread
- [ ]  Under Spread
- [x]  Variable Spread
  
Hint: NoHint
         
Explanation: Fixed Spread and Variable Spread are the two types of Liquidation based on Liquidation spread.

Sub Topics: liquidation-spread
 

---

##### Liquidator does both settlements in one Blockchain transaction. This refers to which of the following Liquidation spread?  

- [x]  Fixed Spread
- [ ]  Variable Spread
- [ ]  Auction Spread
- [ ]  Dutch Spread
  
Hint: Auction or Variable spread are the same
         
Explanation: In Fixed Spread, the Liquidator does both settlements in one Blockchain transaction such as, repays the debt of a borrowing position to Vault and acquires the collateral at a discounted price from the position in return.

Sub Topics: liquidation-spread
 

---

##### Which of the following is not a type of Auction Liquidation?  

- [x]  Fixed Auction
- [x]  Variable Auction
- [ ]  English Auction
- [ ]  Dutch Auction
  
Hint: Languages
         
Explanation: English Auction and Dutch Auction are the two types of Auction Liquidation.

Sub Topics: liquidation-spread
 

---

##### Bidders outbid each other increasingly in which type of Auction Liquidation?  

- [ ]  Fixed Auction
- [ ]  Variable Auction
- [x]  English Auction
- [ ]  Dutch Auction
  
Hint: NoHint
         
Explanation: Bidders outbid each other increasingly in English Auction

Sub Topics: liquidation-spread
 

---

##### What happens in Dutch Auction Liquidation?  

- [ ]  Bidders outbid each other increasingly
- [x]  Auction begins with a high asking price
- [x]  The price lowers until the auction terminates
- [ ]  The price keeps increasing until the auction terminates
  
Hint: NoHint
         
Explanation: In Dutch Auction, Auction begins with a high asking price and the price lowers until the auction terminates

Sub Topics: liquidation-spread
 

---

##### What are the properties of MakerDAO Dutch Auction?  

- [x]  It is settled instantly in one atomic transaction
- [ ]  It is operated in multiple transactions
- [x]  Collateral price decreases over time
- [ ]  Collateral price increases over time
  
Hint: Instant Settlement
         
Explanation: MakerDAO Dutch Auction comprises of Instant Settlement, Flash Lending of Collateral and the Collateral price decreases over time and nobody can get the collateral for free by accident.

Sub Topics: liquidation-spread
 

---

##### What do you mean by Flash Loans?  

- [ ]  Borrow and settle loans instantaneously in multiple transactions
- [x]  Borrow and settle loans instantaneously in a single transaction
- [x]  No collateral required
- [ ]  Collateral is required
  
Hint: Instant processing
         
Explanation: Take loans(in a flash)—> Use them—> Repay loan + interest all in one single atomic blockchain transaction

Sub Topics: flash-loans
 

---

##### Approximate average time required for flash loans on Ethereum Blockchain?  

- [x]  12-14 secs
- [ ]  12-14 hours
- [ ]  12-14 days
- [ ]  12-14 weeks
  
Hint: Instant processing
         
Explanation: It takes 12-14 sec in the case of Ethereum Blockchain.

Sub Topics: flash-loans
 

---

##### Some use cases of Flash Loans are-  

- [x]  Price Oracle Manipulation
- [x]  Pump and Dump
- [x]  Flash Minting
- [ ]  None of the above
  
Hint: all
         
Explanation: Price Oracle Manipulation, Pump and Dump, Flash Minting are some of the use cases of flash loans.

Sub Topics: flash-loans
 

---

##### Pick the odd one out.  

- [ ]  Flash Minting
- [ ]  Collateral swapping
- [x]  Slow loan processing
- [ ]  Wash-trading
  
Hint: Others are use cases of Flash Loans
         
Explanation: Collateral swapping, Wash-trading, Flash Minting are some of the use cases of flash loans.

Sub Topics: flash-loans
 

---

##### Collateral Factor is also know as?  

- [x]  loan-to-value ratio
- [ ]  value-to-loan ratio
- [ ]  loan ratio
- [ ]  value ratio
  
Hint: NoHint
         
Explanation: Collateral Factor is also know as loan-to-value ratio.

Sub Topics: use-cases
 

---

##### In the case of DAI and ETH, Compound has a Collateral Factor of 75%. What does it mean?  

- [x]  Only the 75% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.
- [ ]  Only the 25% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.
- [ ]  100% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.
- [ ]  Only the 7.5% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.
  
Hint: loan-to-value ratio
         
Explanation: In the case of DAI and ETH, Compound has a Collateral Factor(a.k.a loan-to-value ratio) of 75% which means only the 75% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.

Sub Topics: use-cases
 

---

##### Which of the following DeFi platforms have a use case for Over-collateralization?  

- [x]  Compound
- [x]  Alchemix
- [x]  Aave
- [ ]  None of the above
  
Hint: Over-collateralization use cases
         
Explanation: All the following platforms use Over-collateralization.

Sub Topics: use-cases
 

---

##### When does the Flash Loan based liquidation work?  

- [x]  When a liquidator does not have the cryptocurrency upfront to repay and has to complete liquidation in one transaction
- [ ]  When a liquidator does not have the cryptocurrency upfront to repay and does not have to complete liquidation in one transaction
- [ ]  When a liquidator has the cryptocurrency upfront to repay and has to complete liquidation in one transaction
- [ ]  When a liquidator has the cryptocurrency upfront to repay and does not have to complete liquidation in one transaction
  
Hint: Instant processing
         
Explanation: Flash Loan Based Liquidation works When a liquidator does not have the cryptocurrency upfront to repay and has to complete liquidation in one transaction.

Sub Topics: flash-loans
 

---

##### Which of the following DeFi platforms have a collateral factor of 50%?  

- [ ]  Compound
- [x]  Alchemix
- [ ]  Aave
- [ ]  Maker
  
Hint: Borrowing use case
         
Explanation: Alchemix has a Collateral Factor(a.k.a loan-to-value ratio) of 50%  which means only the 50% of supplied(or collateralized valued) DAI or ETH can be used to borrow other tokens.

Sub Topics: use-cases
 

---

##### In case of MakerDAO Dutch Auction, Collateral price decreases over time and anybody can get the collateral for free by accident. True of False?  

- [ ]  true
- [x]  false
  
Hint: liquidation spread
         
Explanation: Collateral price decreases over time but nobody can get the collateral for free by accident.

Sub Topics: liquidation-spread
 

---

##### Range of typical discounts in the case of Aave when the Liquidator does both settlements in one Blockchain transaction?  

- [ ]  50-55%
- [ ]  0.5-0.15%
- [ ]  15-50%
- [x]  5-15%
  
Hint: Close to 5%
         
Explanation: Typical discounts can lie between 5-15% in the case of Aave.

Sub Topics: liquidation-spread
 

---

##### Choose the correct statements.  

- [x]  There may be auctions for liquidating the collateralized asset whose value is degraded.
- [x]  Over-liquidation is when liquidations sell excessive amounts of borrower's collateral
- [ ]  A Fixed Spread liquidation necessarily increases the health factor
- [ ]  Value of Debt to Repay > (Close Factor * Total Value of Debt)
  
Hint: Liquidation
         
Explanation: Value of Debt to Repay > (Close Factor * Total Value of Debt). A Fixed Spread liquidation does not necessarily increase the health factor. Over-liquidation is when liquidations sell excessive amounts of borrower's collateral. There may be auctions for liquidating the collateralized asset whose value is degraded.

Sub Topics: liquidation
 

---

##### Which use case of flash loans enables DeFi users to switch the collateral asset that they used to take out a flash loan on a lending app?  

- [ ]  Price Oracle Manipulation
- [ ]  Flash Minting
- [x]  Collateral swapping
- [ ]  Wash-trading
  
Hint: switch or swap
         
Explanation: Collateral swapping enables DeFi users to swap or switch the collateral asset that they used to take out a flash loan on a lending app

Sub Topics: flash-loans
 

---

##### Which of the following flash loan use cases are DeFi attacks?  

- [ ]  Price Oracle Manipulation
- [ ]  Pump and Dump
- [x]  Both A and B
- [ ]  None of the above
  
Hint: NoHint
         
Explanation: Price Oracle Manipulation & Pump and Dump both are DeFi attacks.

Sub Topics: flash-loans
 

---

##### What happens when a borrower takes out a flash loan of Y tokens on DEX A, then execute two trades by swapping Y tokens for Z tokens on DEX B and vice-versa again on DEX B?  

- [x]  An artificial level of interest is generated which creates an opportunity for profit.
- [ ]  Profit opportunity is not created in such a case
- [x]  The trading volume for the Y tokens increases
- [ ]  The trading volume for the Y tokens decreases
  
Hint: Wash-trading
         
Explanation: This is a scenario for Wash-trading. In such a case the trading volume for the Y tokens increases, creating an artificial level of interest and opportunity for profit.

Sub Topics: flash-loans
 

---

##### What do you mean by Flash Minting?  

- [x]  Attackers can mint an arbitrary number of new Flash-mintable tokens into their account, as long as they also burn the same number of tokens from their account
- [ ]  Attackers can only mint a pre-decided number of new Flash-mintable tokens into their account
- [x]  It is completed in a single transaction
- [ ]  It can be completed using multiple transactions
  
Hint: NoHint
         
Explanation: In Flash Minting, attackers can mint an arbitrary number of new Flash-mintable tokens (a.k.a FMTs or ERC20-compliant tokens) into their account, as long as they also burn the same number of tokens from their account before the end of the same transaction to generate profits.

Sub Topics: flash-loans
 

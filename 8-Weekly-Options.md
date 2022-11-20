<details>
<summary>Weekly Options</summary>
<br>

  <img width="723" alt="image" src="https://user-images.githubusercontent.com/75510135/202854326-1dfa0514-98df-4301-8e02-44ca0f2e226e.png">
 
  
  - Analysis of the **Calendar** trade using Weekly Options
  - ATM options
  - **Sell** 12 days later call option
  - **Buy next month** (40 days) same date call option
  - Example - APPLE trading at 560 currently
  - buy a calenday spread
       - sell june 12 @560 PUT
       - buy july 12 @560 PUT
       
  - check Delta and Theta Value
 
  
  - profit / time chart
  
  
</details>


<details>
<summary>Iron Condor</summary>
<br>

  - 2 spreads
  - directional neutral strategy but purely time decay
  - look for delta 20
  - suppose Apple is trading at 560 then
    - PUT Sell
     - Sell June 530 PUT
     - Buy June 520 PUT
   - CALL Sell
    - Sell June 590 CALL
    - Buy June 600 CALL
  - Adjust the strategy , in case stock goes down then buy a put of next month
  
- look for IV Rank/Percentile above 50
- optimal days to expiration = 45 days(30- 60 days)
  
</details>


<details>
<summary>Short Strangle</summary>
<br>

  - Sell 1 Call and 1 Put, both OTM
  - Look for below 10 delta option
  - say Apple is trading at 560 in June b4 weekly expiry ,then 
     - Sell June 590 CALL (OTM)
     - Sell June 530 PUT  (OTM)
  - Good place on Friday morning and square of on Monday morning to take the advantage of weekend time
  
  - Theoritical price will tell what price gonna look like 
  - SUPPOSE APPLE moved to 585 on the day of expiry then, you will collect all the premium ie total premium will be PRoFIT
   - All the PUT below 585 => 0
   - All the Call above 585 => 0
  
  
</details>

<details>
<summary>Bear Spread</summary>
<br>

   <img width="615" alt="image" src="https://user-images.githubusercontent.com/75510135/202860366-aec372b6-0138-46f1-8a9d-161d095751b6.png">

   - more theta , more profit daily
  <img width="912" alt="image" src="https://user-images.githubusercontent.com/75510135/202862868-fa11b226-5be3-4c95-bbc3-2d107ec75fcc.png">

  
</details>

<details>
<summary>Setting up the Trage</summary>
<br>
  
  
 => Sell at Higher price , buy at lower price
- Select the stocks
    - look for IV Rank/Percentile above 50
    - optimal days to expiration = 45 days(30- 60 days)
    - chose the strike
     * short PUT ITM ( near 20%)
     * long PUT lower strike price
     * short CALL ITM ( near 20%)
     * long CALL at higher strike price

  ***** Note - look at wing width in console  
  
- Eg share , iwm, is currently trading at 109 then
   - Sell IRON Condor at 
     - Sell CALL 114  (lower)
     - Buy CALL 117  (higher)
  
     - Sell PUT 103 (higher)
     - Buy PUT 100  (lower)
  
- Analyze the trade
  - Determine Risk / Reward
  - max Loss should not > 3*Max Profit
  - set price for break-even( to determine the probability of profit)
  - POP should be around 60%
  - in above example its 102 - 115
  - calculate RoC ( return on capital)
  - Exit the trade when profit is 40% of the target max Profit, that is 15% of ROC
  
  
- in case if Stock moved 1 side , say upside
  - close the PUT (both)
  - exit the remaining trade( CALL) , 5 days before expiry
  
- Normal distribution of market moves
  
  
  
</details>

<details>
<summary>Definitions</summary>
<br>


  - Theta => profit per day
</details>



<details>
<summary>Verticals</summary>
<br>

- Vertical deinfition
    -  the combination of buying and selling a CALL
  OR
    -   the combination of buying and selling a PUT to a define risk
  
- Short Vertical
  - selling a CALL or PUT 
- Long Vertical
  - buying a CALL or PUT 
  
  
- Trading Rules
  - Short sell Verticals
  - Time
     - Trade close to 45 days, never less than 30 days & prefer not more than 60 days
  - Votality 
     - if Volatility is > 50 , go with Selling the Verticals
     - if Valatility is < 50 , go with Buying the Verticals
     - List down the stocks with Volatility rank(high to low)
  - Iron Condor
  - Liquidity


 Eg. Buying the veritical
                            
- say stock is currently trading at 299.40
 - BUY 299 CALL
 - SELL 300 CALL  
 - max profit = .45 => 1-.55(credit)
  
- say IWM is trading at 118.27
  - Buy 117 CALL
  - Sell 120 CALL
  - looks for max 50% of profit to book the trade  


 Eg. Selling the veritical
                            
- say stock is currently trading at 397.50
 - SELL 393 PUT
 - BUY 392 PUT  
 - max profit = .40 (credit)
  
- say IWM is trading at 118.27
  - BUY 123 CALL
  - SELL 120 CALL
  - looks for max 50% of profit to book the trade
  
  <img width="865" alt="image" src="https://user-images.githubusercontent.com/75510135/202889687-378e47d8-9d82-4807-949a-d605eb688bb2.png">

  - Check IV, if high , then sell . If Low , then buy
  <img width="1109" alt="image" src="https://user-images.githubusercontent.com/75510135/202890219-b26afb9a-3fa0-4bc9-ba7a-4a686e94c68e.png">

- Rule 
  - Trade small
  - Drawdown effect(how much loose, 2*you need to make)
  - Position size , loss should be = 1% of account on buying , & 2% in case of selling vertical
  - widen the strike
  - Trade more often( number matters)
  - Wealth creation: Discipline 
  - Duration over direction(time to be right)
  - Close before Expiration Day
  - Managing winner , Less % of Profit = more POP
  - Diversification , pick stock from different sectors
  
  
 
  
</details>




## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## dYdX
 
 **Perpetual Contracts in dYdX**        
Perpetual contracts are synthetic trading markets that allow traders to take positions on a variety of assets using stablecoin (USDC) collateral. These contracts can be used to speculate on market movements, hedge risk, or earn profits by going long or short with leverage on a futures contract.

You can start trading with as little as $10 at http://dydx.exchange/.

### Long
If a trader believes that the price of an underlying asset will increase in the future, they may choose to enter into a perpetual contract for that asset. This is done in order to get synthetic exposure, or indirect exposure, to the asset.

### Short 
When a trader goes short, they are selling a Perpetual contract with the belief that the value of the underlying asset will go down in the future. Instead of selling the physical asset, traders sell synthetic exposure to the asset. This allows them to still speculate on the price without having to own the asset.

The working of perpetual contracts/swaps/futures has been explained in detail in the introductory chapter. For more information, please refer to that section. 
 **Placing an Order**        
### TODO
- https://help.dydx.exchange/en/articles/5108526-selecting-order-types
- https://help.dydx.exchange/en/articles/5108531-choosing-the-appropriate-position-buy-or-sell
- https://help.dydx.exchange/en/articles/5108536-understanding-trade-execution
- https://help.dydx.exchange/en/articles/5108538-understanding-open-positions

 
 **Leverage**        
Leverage is the term used to describe how much of your position is being borrowed. The higher the leverage, the less funds you need to deposit as margin and the more you can borrow to open your position. Borrowing more funds comes with more risk, amplifying both your gains and losses, while also making it easier for your position to be liquidated at a loss.

## Simulation
dYdX has an excellent [article](https://dydx.exchange/blog/leverage-intuition) on risks involved in leverage

The purpose of the article is to assist beginners in gaining an understanding of leverage trading and to equip them with the ability to minimize risk by adjusting their position sizes in relation to their collateral balances. By considering a hypothetical scenario, the article aims to provide intuition on appropriate leverage usage. 

In the scenario, it is assumed that the expected return for Ether over the next year is +30%, and a trader has $1000 to invest. The idea of using high leverage to maximize gain is tempting, but the volatility of ETH is also considered to avoid liquidation. Through simulation, it is shown that using 5x leverage results in liquidation in 70% of the return paths, with many successful paths being liquidated before reaching their full potential. 

<image style="max-width:500px" src="https://raw.githubusercontent.com/DoDAO-io/defi-derivatives-course/main/images/dydx/liquidation_chances.png" />

The article concludes by acknowledging that leverage can be beneficial in certain cases, such as for creating capital-efficient positions in hedged portfolios.

## Leverage Limits
[Here](https://help.dydx.exchange/en/articles/4797403-maximum-leverage-for-perpetuals) are the current leverage limits added by dYdX

| Asset | Leverage Limit |
| - | - |
| BTC | 20x |
| ETH | 20x |
| All Other Markets | 10x | 
 **Liquidation**        
## What is Liquidation?
If the total value of an account falls below the maintenance margin requirements, the positions in that account may be closed by the liquidation engine. The positions are closed at the liquidation price, which is described below. The insurance fund pays for any profits or losses from liquidations.

When a liquidation occurs, the liquidator is allowed to take on the entire account balance of the account being liquidated. This could potentially leave the account with zero margin and zero position. Partial liquidation is also an option, where the liquidator would take on a portion of the account's margin and position.

## Liquidation Penalty
If an account is liquidated, the entire value of the account may be taken as a penalty and transferred to the Insurance Fund. The liquidation engine will try to leave funds in accounts of positive value where possible after they have paid the Maximum Liquidation Penalty of 1%.


## Example
Trader A starts with $1000 USDC, then opens a short 1 XYZ (fictional asset) position at $2000 USDC. Their account shows +$3000 USDC, -1 XYZ. The oracle price is $2000 USDC/XYZ, meaning they have a 50% margin.

Later, XYZ's price rises and the oracle reaches $2791 USDC. This drops Trader A's position below the maintenance margin, making it vulnerable to liquidation. The liquidator, with a balance of +$100 USDC, 0 XYZ, liquidates it at the best price of $2800, taking a 1% fee ($28).

This results in A's account balance of $3000-$2800-$28=$172 USDC, and liquidator's balance of +$2928 USDC, -1 XYZ. Finally, the liquidator closes the short position by selling at $2800 USDC, ending with a balance of +$128 USDC, 0 XYZ.

More information on Liquidation can be found [here](https://help.dydx.exchange/en/articles/4797401-perpetual-contract-liquidations) 
 **References**        
- https://dydx.exchange/blog/leverage-intuition
- https://help.dydx.exchange/en/articles/5108521-understanding-your-account-balance-leverage
- https://dydx.exchange/blog/max-leverage-reduction
- https://help.dydx.exchange/en/articles/4797403-maximum-leverage-for-perpetuals
- https://medium.com/dydxderivatives/getting-started-with-dydx-margin-trading-part-1-fe43789c2368
- https://help.dydx.exchange/en/articles/5108526-selecting-order-types
- https://help.dydx.exchange/en/articles/5108531-choosing-the-appropriate-position-buy-or-sell
- https://help.dydx.exchange/en/articles/5108536-understanding-trade-execution
- https://help.dydx.exchange/en/articles/5108538-understanding-open-positions 
 

## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## GMX
 
 **Trading**        
## Opening a position
### Definition of "Entry Price" and "Liquidation Price":
- The "Entry Price" is set at $3541.17
- The "Liquidation Price" is set at $2903.76
- "Exit Price" is the price used to calculate profits if you open and close a position immediately, it changes with the token price you are trading.

#### Trading Fees:
- A fee of 0.1% of the position size is charged when opening a position
- A fee of 0.1% of the position size is charged when closing a position

#### Borrow Fee:
- Deducted hourly and paid to the counter-party(GLP Holders) of your trade
- Varies based on utilization, calculated as (assets borrowed) / (total assets in pool) * 0.01%

#### Slippage:
- The difference between expected trade price and execution price
- Can occur due to price movements during trade confirmation on blockchain

## Fees
- Opening/closing a position cost: 0.1% of the position size
- Swap fee (if applicable): 0.2% to 0.8% of the collateral size, depends on improving balance or reducing it
- Execution fee: This network cost is paid to the blockchain network. 
 **GLP Token**        
GLP is the token that provides liquidity to the platform. It is made up of a collection of assets used for swapping and leverage trading. You can create GLP tokens using any of the index assets and convert them back into index assets at a price that's calculated based on the total value of assets in the index (including profits and losses from open positions) divided by the GLP supply.

Holders of GLP tokens earn Escrowed GMX rewards and receive 70% of platform fees, which are distributed in ETH on Arbitrum and AVAX on Avalanche. Keep in mind that these fees take into account referral rewards and network costs for keepers (usually around 1% of total fees).

It's important to note that GLP is specific to the network where it's minted and is not directly transferable between networks. The price and rewards for GLP tokens will vary between networks. The performance of GLP, including past PnL data and price chart, can be viewed at https://stats.gmx.io. Keep in mind that as a liquidity provider, the profit or loss of GLP holders is tied to the success or failure of leverage traders.

## Minting and Rebalancing
The fees for minting GLP, burning GLP, or executing swaps will vary based on whether the action increases or decreases the balance of assets in the index. For example, if the index has a large proportion of ETH and a small proportion of USDC, actions that add to the ETH in the index will incur a high fee, while actions that decrease the ETH will have a low fee.

The token weights are adjusted to hedge GLP holders based on the trading positions of traders. For instance, if many traders have long positions on ETH, ETH will have a higher token weight, and if many traders have short positions, stablecoins will have a higher token weight.






 
 **GMX & GLP Tokens**        
## GMX
GMX is the platform's utility and governance token, holding the token unlocks a variety of benefits.
After staking GMX, you will receive a staked GMX token.

### Escrowed GMX
Escrowed GMX (esGMX) can be used in two ways:
1. Staked for rewards similar to regular GMX tokens
2. Vested to become actual GMX tokens over a period of one year

Each staked Escrowed GMX token will earn the same amount of Escrowed GMX and ETH / AVAX rewards as a regular GMX token.

### Staked GMX
Staked GMX receives three types of rewards:
- Escrowed GMX
- Multiplier Points
- ETH / AVAX Rewards

30% of fees generated from swaps and leverage trading are converted to ETH / AVAX and distributed to staked GMX tokens. If you are staking on Arbitrum you would receive ETH, if you are staking on Avalanche then you would receive AVAX. Note that the fees distributed are based on the number after deducting referral rewards and the network costs of keepers, keeper costs are usually around 1% of the total fees.

### Vesting

The esGMX tokens can be transformed into GMX tokens through a process called vesting. During vesting, the average amount of GMX or GLP tokens used to earn the esGMX rewards will be reserved. For instance, if you staked 1000 GMX and received 100 esGMX tokens, then to vest 100 esGMX tokens, 1000 GMX tokens will be set aside. The actual ratio may vary based on your staked amount and rewards earned.

Once vesting has been initiated, esGMX tokens will no longer earn rewards. However, the GMX tokens reserved for vesting will still earn rewards. The esGMX tokens will be converted into GMX tokens over a period of 365 days. Once they are fully converted, they can be claimed at any time.

If you sell GMX or GLP tokens and later wish to vest your esGMX rewards, you'll need to purchase those tokens again. You can use GMX, esGMX or Multiplier Points to fulfill the required reserve amount.

It's possible to deposit into the vesting vault while ongoing vesting is in progress.

### Floor Price Fund
The GMX token has a floor price fund in ETH and GLP. It grows in two ways:
- GMX/ETH liquidity is provided and owned by the protocol, the fees from this trading pair will be converted to GLP and deposited into the floor price fund
- 50% of funds received through Olympus bonds are sent to the floor price fund, the other 50% is used for marketing 

The current floor price fund is viewable on the Dashboard.

The floor price fund helps to ensure liquidity in GLP and provide a reliable stream of ETH rewards for all staked GMX.

As the floor price fund grows, it can also be used to buyback and burn GMX if the (Floor Price Fund) / (Total Supply of GMX) is less than the market price, this would lead to a minimum price for GMX in terms of ETH and GLP.

 
 **References**        
- https://blockgeeks.com/guides/what-is-gmx-protocol/
- https://academy.binance.com/en/articles/what-is-gmx
- https://www.youtube.com/watch?v=LJwxOF_L65s

Stats
- https://app.gmx.io/#/dashboard
- https://stats.gmx.io 
 

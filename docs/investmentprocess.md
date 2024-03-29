# How to use uTrade

## How to start?  

Investing on uTradeFi requires a couple of simple steps to create a synthetic tracker and implement advanced trading rules. All the steps are described below

## Step 1: Bring investment capital to the protocol

To start the journey, **investment capital** need to be transferred to the protocol. This is simply done by connecting the investor's digital wallet (e.g. Metamask or alike) to uTradeFi via the "Connect" button. Then the investor can define how much of his wallet to transfer to the protocol via the App. Once the funds are transferred, a synthetic tracker is minted equivalent to the value of the investment capital. By default, 100% of the funds will be invested in Ether in his synthetic tracker, ie the same currency as the investment capital.

> Connect the investor's digital wallet to the protocol and transfer investment capital to create personalized synthetic trackers

## Step 2: Define the asset allocation of the synthetic trackers

The asset allocation of the synthetic tracker can be changed by **converting** the original investment capital into another asset or asset class: e.g. convert from ETH to BTC. This is done via specific menus in the App. The conversion from an asset to another one is done in real time at the prevailing prices provided by oracle blockchains. There are no bid/ask spreads nor real buy/sell via exchanges. The trades are executed on a peer-to-contract model.

The simplest form of trade are trades with an immediate execution. These trades are executed directly after the trade capture and don't rely on triggers to be executed
* Buy now
* Sell now
* Short now

> Convert from an asset to another one frictionless with "simple trades"

## Step 3: Implement smart trading logics

Smart trading rules can be easily set up. The **smart trading rules** will be run automatically by the trading bots when pre-defined triggers are hit. These trading logics allow the investors to have conditional buys or sell based on agreed triggers. These advanced functionalities are not mandatory and can be skipped if investors prefer simple trades. The advanced trades are:

Advanced trade: trigger based
* Buy now with profit taking and stop loss triggers
* Sell now with buy back triggers
* Deferred buy based on trigger
* Deferred sell based on trigger

> "Advanced trades" rely on triggers for conditional future execution

## Step 4: Let the bot trade for you

Let the bot monitor the market and trade for you to benefit from the smart trading logics!

## Step 5: Liquidate your position

At any time the synthetic trackers can be liquidated, the corresponding investment capital freed up, and brought back to the investors wallets. The liquidation is done in 2 steps: i) all exposures are converted into Ether at the prevailing prices and ii) the Ether balance transferred to the investor wallet. The amount of Ether transferred back is adjusted for the gains and losses of the synthetic tracker.  

>Example: 100 is invested at time=0. At time=1 the investment strategy is worth 90, i.e. a loss of 10. If the investor decide to liquidate its synthetic tracker and bring back the investment capital to its wallet, only 90 would be available. The investor made a loss of 10!

>Example: 100 is invested at time=0. At time=1 the investment strategy is worth 110, i.e. a gain of 10. If the investor decide to liquidate its synthetic tracker and bring back the investment capital to its wallet, 110 would be available: 100 originally posted and an additional 10 from the gain from the synthetic tracker. The investor made a gain of 10!

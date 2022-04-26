# How to use uTrade

## How to start trading on uTradeFi?  

Investing on uTradeFi requires a couple of simple steps to collateralize the sythetic trackers and define smart trading rules to generate returns.

## Step 1: Transfer ETH from wallet to the protocol

The protocol supports ETH as collateral. The collateral need to be transfered from a digital wallet to the trading protocol. The collateral is used to mark-to-market the PnL of the synthetic trackers.

Let's imagine that the investment strategy doesn't perform as expected and a loss occurs, the corresponding amount of collateral would be lost.

>Example: 100 is invested at time=0. At time=1 the investment strategy is worth 90, i.e. a loss of 10. If the investor decide to liquiditate its synthetic tracker and bring back the collateral to its wallet, only 90 would be available. The investor made a loss of 10!
Example: 100 is invested at time=0. At time=1 the investment strategy is worth 110, i.e. a gain of 10. If the investor decide to liquiditate its synthetic tracker and bring back the collateral to its wallet, 110 would be available: 100 originally posted and an additional 10 from the gain from the synthetic tracker. The investor made a gain of 10!

## Step 2: Define the asset allocation of the synthetic trackers

The asset allocation of the synthetic tracker can be define by converting the orginal invested amount into another asset: e.g. convert from ETH to BTC.

## Step 3: Implement smart trading rules

Various smart trading rules can be easily set up. The smart trading rules will be run automatically by the trading bots when a pre-defined trigger is hit
* with profit taking triggers
* with stop-loss triggers

## Step 4: Let the bot trade for you

Relax and let the bot trade for you to capitalize some trading gains!

## Step 5: Liquidtate your position to free the collateral posted to the protocol

At any time the synthetic trackers can be liquiditated and the corresponding ETH amount brought back to the investor wallet.

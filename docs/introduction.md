# Overview

## What is uTradeFi?

uTradeFi allows investors to create **synthetic trackers** or **sTrack** across multiple asset classes. Investors define their trading rules by setting up **smart trading logics** that are executed automatically according to the instructions. Investors can setup various trigger points when defining their trading strategies to maximize their profits under different scenarios: e.g. profit taking triggers when a high price trigger is reached, stop loss triggers if a low price is reached, buy backs triggers for sell orders, etc.

> Investors create their own synthetic trackers to take advantage of their proprietary asset allocation and trading strategy.

uTradeFi is a "closed" system where gains of some actors and absorbed by losses of others. There are no connectivity required with external exchanges and all trading activity is performed in the protocol itself.

> uTradeFi is a self-sufficient protocol that doesn't require external connectivity (e.g. CeX or DeX)

## What is unique to uTradeFi?

It's based on a peer-to-contract trading model where synthetic trackers are minted and burned accordingly to the investors trading activity, without buying, minting or holding the underlying assets. **sTrack** are onchain representation of the underlying basket it's tracking, including its composition and exposure. The creation of the synthetic trackers is insured by smart contracts on the blockchain.

> sTrack are onchain representation of the basket it's tracking: symbols and exposures

By design, the protocol is a "closed" system based on the redistribution of the risks between 2 different stakeholders: the **investors** themselves which naturally will create some diversification effects (e.g. some making money and some losing) and the **pool performance underwriters** which are responsible for the overall performance of the investment pool. This unique setup ensures that all actors making money are paid from the one losing, ie between investors and underwriters.

> uTradeFi is based on an ingenious redistribution mechanism where gains and losses are cleared amongst the actors of the protocol: the investors and the pool performance underwriters

## What are synthetic trackers or sTrack?

sTrack is the **symbol** for the synthetic trackers created by protocol. Each tracker is unique as it's customized to the investor trading strategy. Therefore sTrack is a non-tradable asset that can't be transferred or traded outside uTradeFi. sTrack are "non-fungible non-tradable" assets. Each synthetic tracker can be redeemed in their ETH equivalent value. There are no limitation for the monetization of the synthetic trackers and is allowed 24/7.

> sTrack are non-fungible non-tradable synthetic trackers

Synthetic trackers or sTrack are created as soon as investors bring **investment capital** to the protocol. The investment capital is used as collateral if the investor lose money with his synthetic tracker. Once the investment capital (or collateral) is transferred to the protocol, a unique sTrack is created with a default asset allocation. The investors can then amend the synthetic tracker to reflect their own trading strategies.

Ether is the only currency accepted by the protocol as investment capital. ETH is defined as the reference asset to calculate the profit and losses of each synthetic tracker. All mark-to-market gains and losses of the synthetic trackers are cleared in the reference asset currency.

> Bring Ether to the protocol and start defining the asset allocation of the synthetic tracker

## How do I make money as an investor?

Each investor will then amend the composition of his synthetic tracker by deploying the investment capital to other asset types which will hopefully **outperform the reference asset** (e.g. convert ETH to BTC). If the value of the tracker is above the amount of trading capital transferred, a gain was generated and the investor is in a position to capitalize that gain by redeeming the tracker to unlock it's trading capital and corresponding gains.

## Are sTrack tradable outside the protocol?

No, synthetic trackers or sTrack are **locked in the protocol** and can't be traded outside. However they can be liquidated at any time by converting the underlying assets into their ETH equivalent price and the initial investment capital freed up accordingly. The burning of the sTrack is executed by the investors with the investment capital automatically transferred back. This gives the investors the capability to exit the system at any time and have their funds back (adjusted with the potential gain and losses of their past investments).

> No, the sTracks need to be burned to free up the investment capital transferred initially to the protocol

## To whom is it addressed to?

uTradeFi is a protocol relying on two pillars: investors and pool performance underwriters. These are the main actors of the system.

Therefore it's addressed to all **investors** who want to make money by setting up winning trading strategies across a large trading universe, without the hassle to hold the underlying assets. uTradeFi allows the creation of synthetic trackers or **sTrack** in a simple way that mimic the performance of the underlying assets. Investors benefit from the profits generated by these synthetic trackers. Investors might face losses if poor investment decisions are made where the synthetic trackers underperform the reference asset.

> uTradeFi is addressed to all investors capable of creating profits with smart investment strategies

For the **pool performance underwriters** there are two different business models that can be envisaged.

Option 1: Financial institutions - **private protocol**

uTradeFi is a great solutions for financial institutions who want to offer a new type of investment opportunities into digital assets to its client base. A financial institution can play the role of the pool performance underwriter and hedge the aggregated exposure of the investors synthetic trackers and collect transactional fees from the protocol. The solution can work on public or private blockchains based on the preference of the institution.

Option 2: Pure DeFi - **public protocol**

uTradeFi could also work on a fully DeFi basis where the pool performance underwriters are simple "individuals" who want to earn fees by assuming the overall performance of the pool. These fees are collected from the investors (trading fees and performance fees) and redistributed as a reward to assume the net pool performance risk. However the protocol would be a bit more risky as it relies on enough pool performance underwriter capacity. Therefore the DeFi model is not favoured at the moment and the focus is on Option 1.

> uTradeFi is also addressed to all pool performance underwriters (financial institutions or private based on options above) that want to earn fees while being exposed to the net performance of the synthetic tracker pool.

## How much does it costs?

uTradeFi pricing is fairly simple:
* a flat fee of 10bps (tbd) for each transaction is collected (for buy/sell, shorts and all type of advanced trade)
* a performance fee of 30bp (tbd) is also collected if the synthetic tracker generates a positive gain (on the gains only), ie outperform the reference asset

The fees collected are distributed to the pool performance underwriters which assume the overall risk of the investment pool. This ingenious fee redistribution gives a strong incentive to the underwriters to assume the overall risk of the investment pool.

## How much gains and losses are covered by the protocol logic?

The protocol allows each sTrack to lose 80% (tbc) of its value before being automatically converted back into the reference asset, ie Ether (if no actions are taken by the investors). The automatic conversion into the reference asset (Ether) is executed with smart contracts to mitigate future losses.

The protocol guarantees an increase of 80% (tbc) of the overall investment pool size if no specific actions are taken by the pool performance underwriters. This means that if all the pool was invested in non-Ether assets, the protocol would guarantee a performance of 80% above Ether before liquidating the position of the underwriters and investors.

## What are the main risks?

The main risk is market risk, i.e. the risk to lose money with bad investment decisions. Please read carefully the section on "Risks".

?> The unique design of uTradeFi with collateralized investors losses and collateralized pool performance underwriters losses allow the clearing of the gains and losses of the system in all circumstances.

# Key concepts

## Synthetic tracker

uTradeFi enables investors to create customized synthetic trackers "sTrack". A synthetic tracker is an asset that tracks the value of various underlying assets without the need to buy the underlying assets. The composition of the synthetic trackers reflect the trading activity of the investors. There are as many synthetic trackers as investors as each investor can setup its own asset allocation rule. The pricing of the synthetic trackers is a function of the quantity of the assets it's tracking and the prices of the underlying assets. The content of the synthetic trackers are represented in the blockchain by specific smart contracts. The composition of the trackers is dynamic and changes over time based on new trading instructions.

Investors customize the composition of their synthetic tracker by setting up trading rules via "smart trading" functionalities the protocol offers. The valuation of the synthetic tracker is performed by blockchain Oracles  that independently provide pricing feeds to the protocol.  

The individual performance of each synthetic tracker is assumed by the investor via a collateralization mechanisms. The overall pool performance is assumed by underwriters.

?> Synthetic trackers are onchain representation of exposures across multiple assets. Each synthetic tracker is uniquly reflecting each investor trading strategy.

## Peer-to-Contract trading

uTradeFi is based on synthetic exposures and doesn't require connectivity to Decentralized exchanges (DeX) or Centralized exchanges (CeX). All trades are executed against smart contracts, commonly known as peer-to-contract trading (P2C). The exposures of each synthetic trackers are minted and burned accordingly to the trading activity of the investors. When an investor ammend the compostion of a tracker (e.g. convert ETH into BTC), the composition of the tracker is ammended accordingly at the prevailing price of BTC|ETH.

This unique P2C setup allows instant conversion across the synthetic asset universe of the protocol without liquidity issues nor impact on the prices of the underlying assets. This represents a significant simplification for trading execution as there's no need for complex order books and any connectivity to exchanges. All trading happens within the trading protocol independently based on logics defined by smart contracts .

?> Trading in the protocol is executed against smart contracts following a P2C model by minting and burning the corresponding composition of the syntetic trackers.

## Centralized trading execution

The synthetic trackers are onchain representations of the investors trading strategy. These synthetic trackers are not usual tokens (e.g. ERC20 tokens) and can't be traded outside the protocol as they can be unique for each investor. All trade orders are executed by the protocol on behalf of the investors based on defined trading rules and can't be executed by anyone else. The value of the syntetic trackets could be theoretically displayed in the investor wallet by importing the respective smart contract address but can NOT be bought, sold or transfer directly.

?> The execution of the trade instructions is performed by the Protocol on behalf of the investors to allow trading bots to run automatically 24/7 without manual approval

## Who absorbs the P&L of the overall pool?

The gains and losses of the overall investment pool are absorbed by the underwriters of the pool performance. These are stakeholders that are absorbing the overall risk of the entire pool in exchange of trading fees and performance fees paid by the investors as a result of their trading activity. In a situation where investors have opposite exposures (e.g. short vs long), the overall market risk of the pool will be low and the gains of some investors will be absorbed the losses of others investors. If the overall pool is imbalanced (e.g. all investors are long) the overall gains and losses will be covered by the underwriters. See next section for more information.

?> The gains and losses of the investment pool is absorbed by the pool performance underwriters

## Pool capacity

The pool capacity represents the ratio between investors and pool performance underwriters. The clearing of the gains and losses require an adequate amount of pool performance underwriters. Therefore new investors can invest only when pool performance underwriters are available to absorb the potential increased performance risk. The capacity measures the ratio between investors and underwriters and is targeted at 90%. New investors need to wait once that threshold is reached and will be able to invest if other investors leave the protocol or new underwriters join the protocol.

?> The pool capacity is at maximum 90%. If more capacity is required, additional pool performance underwriters are required (or other investors to leave the protocol)

## Price of the synthetic trackers

The prices of the synthetic trackers are determined by blockchain Oracles.

The prices of the all underlying synthetic assets are determined by a decentralized blockchain Oracles. The prices are used to convert assets amongst each others at these prevailing prices. The mark-to-market gains and losses of the investor synthetic tracker is based on the same price feed. The prices are fetched every X seconds and fed to the trading bots. The trading activity within the Protocol have no impact on the prices at which the synthetic assets are traded. These prices are an input to the trading Protocol.

?> Prices are provided by blockchain Oracles and used to define the exchange rate between synthetic assets.

## Synthetic asset universe

The trading universe of the Protocol is defined by the data availability from the blockchain Oracles. The exact universe will evolve over time but it's envisaged to cover initially the following asset classes:
- Crypto coins: ETH, BTC, DOT, ...
- Cryp tokens: UNI, AAVE, ...
- FX: USD, CHF, EUR, GBP, JPY, ...
- Commodities: XAU, XAG, XPD, ...
- Stocks: to be defined

?> The synthetic trackers can take exposure against as many asset classes and instruments type as long as a reliable price feed is available. The trading universe will increase over time based on the price availability.

## Monetization of the synthetic trackers back to the investor wallets

When investors want to exit the protocol and monetize the gains or losses of their respective synthetic trackers, they can convert all their synthetic holdings back to ETH independently with a special smart contract functionality. The smart contract will convert all none ETH synthetic exposures back to ETH based on prices from blockchain Oracles automatically. Then it transfers the corresponding amount of collateral back to the investor wallet: e.g. if the investor invested at t=0 100 and now has 110 worth if ETH, the investor will receive back 110 (i.e. a gain of 10). In the other hand if the investor has only 90 worth of ETH, he will receive only 90 out of the 100 he initially transferred to the protocol (i.e. a loss of 10).

## Pool performance underwriters

The value of overall investment pool is a function of the net total supply of each synthetic assets and the prevailing prices at that time. Any net gains and losses are absorbed by the pool performance underwriters. The underwriters have to collateralize the amount of debt they own and any losses is monetized by the corresponding amount of collateral locked in the protocol. E.g. if an underwriter provide 100 of collateral but the amount of debt he owns is worth 120, a net amount of 20 will be kept, i.e. the investor will be able to repatriate only 80 worth of collateral if his exposure is liquidated.

?> underwriters are absorbing the risks of the overall investment pool

## Wallets

Investors need to own a digital wallet to interact with the protocol. Investors need to connect his wallet to the protocol (e.g. Metamask and alike) and transfer ETH to the protocol. This will result to a debit of the investor wallet and a credit of the protocol wallet. The amount transfered is represented by a smart contract and tracked for each investor.

?> Investors connect to the protocol with classic digital wallets: Metamask and alike

## Reference assets

The reference asset is defined as the reference "currency" of the protocol and is used as reference to calculate the profit and losses of each investor. It's envisaged that Ether will be the reference currency and therefore any profit and losses will be calculated against the performance of Ether.

?> The reference asset of uTradeFi is Ether. The gains and losses are calculated against the reference asset

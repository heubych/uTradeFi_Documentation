
# Risk Overview

## Introduction

The sections below contain some of the key risks that users of the protocol face. Most of these risks are common to other DeFi protocols. Some are specific to uTradeFi (e.g. market risk of the trackers). Please read carefully and make sure you understand those before investing.

## Market risk

Market risk refers to the possibility that participants of the protocol will experience losses due to factors that affect the overall performance of the synthetic trackers.

### Market risk of the synthetic trackers

The protocol empowers investors to make money based on synthetic trackers and smart trading logics. But at the same time it creates a risk of losses when poor investment decisions are made. Investors are exposed to the market risk of their synthetic tracker as a result of their investment strategy. When bad investment decisions are made, investors might occur severe losses and will lose some of the investment capital they have locked in the protocol. The risk of loses arise from long positions when prices decrease and short positions when prices increase. In theory, an unlimited loss could occur with short positions as the underlying prices could increase infinitely. In case of losses, investors will be able repatriate to their respective wallets their investment capital adjusted by the losses.

!> Investors might lose money if bad investments decisions are made (e.g. wrong timing, investment in under-performing assets)

### Market risk of the overall pool for the pool performance underwriters

Pool performance underwriters are exposed to the overall pool performance. Loses arise when the value of the overall pool increases (denominated in the reference asset, i.e. Ether) as a consequence of successful investors investment strategies. In a scenario where all investors beat the reference asset performance (Ether), the value of the pool would increase and underwriters would suffer losses.

!> Underwriters are exposed to the overall pool performance. When the overall pool grows due to the increase of the prices of the synthetic assets, underwriters will suffer losses.

## Smart contract risk

The core logics ruling uTradeFi are implemented as smart contract in the blockchain. Smart contract risks are risks that are the consequence of unknown bugs in the smart contracts. To mitigate these risks, various actions will be performed:
* extensive testing of the protocol and its smart contracts, including on testnets
* independent review of the smart contracts by an audit firm
* publish the code of the smart contracts on github

!> Smart contracts might be exposed to bugs (like any software)

## Regulatory risk

Regulatory risk is the risk that a change in regulations or laws will materially impact uTradeFi. Regulators might ban such Defi protocols in the coming years.

If regulators were to ban such protocols, the synthetic trackers would be simply converted back to ETH and the investment capital transferred back to the investors wallets (adjusted by the gain and losses of the investment strategies obviously). Therefore there's no real risk as the funds would be transferred immediately back the investors.


# Risk Overview

## Is it risky to use uTradeFi?

The sections below contain some of the key risks that users of the protocol face. Most of these risks are common to other DeFi protocols. Some are specific to uTradeFi (e.g. market risk of the trackers). Please read carefully and make sure you understand those before investing.

## Market risk

Market risk refers to the possibility that participants of the protocol will experience losses due to factors that affect the overall performance of the synthetic trackers.

### Market risk of the synthetic trackers

The protocol empowers investors to make money based on synthetic trackers and smart trading logics. But at the same time it creates a risk of losses when poor investment decisions are made. Investors are exposed to the market risk of their synthetic tracker as a result of their investment strategy. When bad investment decisions are made, investors might occur severe losses and will lose some of the investment capital they have locked in the protocol. The risk of loses arise from long positions when prices decrease and short positions when prices increase. In theory, an unlimited loss could occur with short positions as the underlying prices could increase infinitely. In case of losses, investors will be able repatriate their investment capital adjusted by the losses to their respective wallets.

!> Investors will lose money if bad investments decisions are made (e.g. wrong timing, investment in under-performing assets)

### Market risk of the overall pool for the pool performance underwriters

Pool performance underwriters are exposed to the overall pool performance. Loses arise when the value of the overall pool increases (denominated in the reference asset, i.e. Ether) as a consequence of successful investors investment strategies. In a scenario where all investors beats the reference asset performance (Ether), the value of the pool would increase and underwriters would suffer losses.

!> Underwriters are exposed to the overall pool performance. When the overall pool grows due to the increase of the prices of the synthetic assets, underwriters will suffer losses.

### Safe-guard: Automatic conversion of synthetic trackers

Loss making synthetic trackers are automatically converted back to Ether once 80% of the invested capital is gone. The automatic conversion of the losing synthetic trackers cap the amount of loss investors might experience. Therefore investors should never be in a position where they lost more than the invested capital.

?> Synthetic trackers are automatically liquidated if 80% of the invested capital is lost

A 20% buffer is available for close-out risk as prices might be very volatile when the synthetic trackers are converted back to Ether.

?> A 20% buffer is available for close-out risk to ensure that investors don't lose more than their invested capital

### Safe-guard: Automatic liquidation of pool performance underwriters positions

Underwriters positions are automatically liquidated once 80% of the provided collateral is consumed. The key risk of loses arise from an increase in value of the overall pool (denominated in the reference asset, i.e. Ether) as a consequence of successful investors investment strategies. This is a safe-guard to ensure the stability of the protocol and make sure that the net gains of all investors are paid accordingly.

?> Underwriters positions are automatically liquidated (if no action taken) once 80% of their collateral is consumed

## Volume risks

Volume risk refers to the mismatch between the amount of investors versus the amount of pool performance underwriters. Imbalances (in term of collateral provided) is problematic.

### Excess of underwriters vs investors

Any excess of underwriters capacity doesn't lead to significant issues. E.g. if existing investors are exiting the protocol (therefore leading to an excess of underwriters), the investment pool would shrink accordingly and the amount of performance the underwriters are responsible for would decrease. Therefore there are no risk in that scenario as all gains and loses would be still 100% collateralized. In an extreme scenario where all investors would be exiting the protocol, no synthetic trackers would be still live and the pool performance underwriters not needed anymore. Therefore a reduction of investors appetite doesn't represent a risk for the system.

!> An excess of underwriters capacity doesn't represent a risk for the protocol. All gains and losses can be cleared between investors and pool peformance underwriters

### Excess investors vs underwriters

The protocol requires performance underwriters to guarantee the overall investment pool performance. If there's more investor than underwriter capacity, the clearing of the gains and losses is problematic in a scenario where the overall pool grows (from trading gains) and actions need to be taken to guarantee the stability of the protocol. This would require a proportional decrease of the investor capacity accordingly to the pool performance underwriters. The decrease in investor capacity is handled automatically by smart contracts that guarantee the stability of the protocol.  

If underwriters are exiting the system while investors are 100% using the pool capacity, this would result in issues as the exposure of the investors would need to be reduced proportionally. In an extreme situation where all peformance underwriters are exiting the protocol, the full liquidation of all sTrack is required.

!> An excess of investors represent a risk...!!! More thinking to be done here!!!

## Smart contract risk

The core logics ruling uTradeFi are implemented as smart contract in the blockchain. Smart contract risks are risks that are the consequence of unknown bugs in the smart contracts. To mitigate these risks, various actions will be performed:
* extensive testing of the protocol and its smart contracts, including on testnets
* independent review of the smart contracts by an audit firm
* publish the code of the smart contracts on github

!> Smart contracts might be exposed to bugs (like any software)

## Regulatory risk

Regulatory risk is the risk that a change in regulations or laws will materially impact uTradeFi. Regulators might ban such Defi protocols in the coming years.

If regulators were to ban such protocols, the synthetic trackers would be simply converted back to ETH and the investment capital transferred back to the investors wallets (adjusted by the gain and losses of the investment strategies obviously). Therefore there's no real risk as the funds would be transferred immediately back the investors.

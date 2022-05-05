
# Risk Overview

## Is it risky to use uTradeFi?

The sections below contain some of the key risks that users of the protocol face. Most of these risks are common with other Defi protocols. Some are specific to uTradeFi (e.g. market risk of the trackers). Please read carefully and make sure you understand those before investing.

## Market risk

Market risk refers to the possibility that participants of the protocol will experience losses due to factors that affect the overall performance of their synthetic trackers.

### Market risk of the synthetic trackers

The protocol empowers investors to make money based on synthetic trackers and smart trading logics. But at the same time it creates a risk of losses when poor investment decisions are made. Investors are exposed to the market risk of their synthetic tracker as a result of their investment strategy. When bad investment decisions are made, investors might occur severe losses and will lose some of the investment capital they have locked in the protocol. The risk of loses arise from long positions when prices decrease and short positions when prices increase. In theory, an unlimited loss could occur with short positions as the underlying prices could increase infinitely. In case of losses, investors will be able repatriate their investment capital adjusted by the losses to their respective wallets.

!> Investors will lose money if bad investments decisions are made (e.g. wrong timing, investment in under-performing assets)

### Market risk of the overall pool for the CDP Issuers

Funding providers are exposed to the overall pool performance. Loses arise when the value of the overall pool increase (denominated in the reference asset, i.e. Ether) as a consequence of successful investment strategies. In a scenario where all investors beats the reference asset performance (Ether), the value of the pool would increase and CDP issuers would suffer a loss.

!> Funding providers are exposed to the overall pool performance. When the overall pool grows due to the increase of the prices of the synthetic assets, funding providers will suffer a loss.

### Safe-guard: Automatic liquidation of losing synthetic trackers

Loss making synthetic trackers are automatically liquidated by the protocol once 80% of the invested capital is gone. The automatic liquidation of the losing synthetic trackers cap the amount of loss investors might experience. Therefore investors should never be in a position where they lost more than the invested capital.

!> Synthetic trackers are automatically liquidated if 80% of the invested capital is lost

### Safe-guard: Close-out risk

Synthetic trackers are liquidated once 80% of their value is lost. A 20% buffer is available for close-out risk as prices might be very volatile when the synthetic trackers are burned.

!> A 20% buffer is available for close-out risk to ensure that investors don't lose more than their invested capital

### Safe-guard: Automatic liquidation of CDP issuer positions

Funding providers positions are automatically liquidated once 80% of the provided funding is consumed. The key risk of loses arise from an increase in value of the overall pool (denominated in the reference asset, i.e. Ether) as a consequence of successful investment strategies. This is a safe-guard to ensure the stability of the protocol and make sure that the net gains of all investors are paid accordingly.

!> Funding provider positions are automatically liquidated (if no action taken) once 80% of their position is lost

## Smart contract risk

The logics defining uTradeFi are implemented as smart contract on the blockchain. Smart contract risks are risks that are the consequence of unknown bugs in the smart contracts. To mitigate these risks, various actions will be performed:
* extensive testing of the protocol and its smart contracts, including on testnets
* independent review of the smart contracts by an audit firm
* publish the code of the smart contracts on github

!> Smart contracts are exposed to bugs (like any software)

## Regulatory risk

Regulatory risk is the risk that a change in regulations or laws will materially impact uTradeFi. Regulators might ban such Defi protocols in the coming years.

If regulators were to ban such protocols, the synthetic trackers would be simply converted back to ETH and the investment capital transferred back to the investors wallets (adjusted by the gain and losses of the investment strategies obviously). Therefore there's no real risk as the funds would be transferred immediately back the investors.

## Volume risks

Volume refers in that context to the amount of invested capital investors have provided and to the amount CDP issuers have provided.

### Volume risk: lack of Investors

If investors are exiting the protocol, the investment pool would shrink accordingly and the amount of debt the funding providers would be responsible would also decrease. Therefore there are no risk in that scenario and all the gains and loses could be paid, just on a smaller pool. In an extreme scenario where all investors would be exiting the protocol, all synthetic trackers would have been liquidated and the funding providers not needed anymore. Therefore the lack of investors doesn't represent a real risk.

### Volume risk: Lack of pool CDP Issuers

The protocol requires funding providers to guarantee the overall investment pool performance. If there are more investors than CDP issuers capacity, the clearing of the gain and losses is problematic and actions need to be taken to guarantee the stability of the protocol.

If funding providers are exiting the system while investors are 100% using the pool capacity, this would result in issues as the exposure of the investors would need to be reduced proportionally. In an extreme situation where all funding providers are exiting the protocol, the full liquidation of all sTrack would be required.

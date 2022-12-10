# Collateralization mechanism of the Pool Performance Underwriter

## Undisclosed collateral amount by the pool performance underwriter

The provider of the protocol doesn't disclose the amount of collateral it holds to back the net growth of the pool (in the case of positive investment returns from investors). The investors need to trust the provider of the platform that he will meet his obligations by holding enough collateral. If not enough collateral is held, in a situation where the pool size increased due to positive performance the liquidation of the sTrack will be problematic.

## Disclosed collateral amount and safe guard

The provider of the protocol explicitly define the amount of collateral it holds (e.g. 50% of the value of the pool) and ensure that it holds that much at any time. If not enough collateral is held (say 40%), the liquidation of the sTrack are executed automatically with smart contracts and all investors get back their funds. This automatic liquidation mechanism safe-guard the investors against unfunded gains.

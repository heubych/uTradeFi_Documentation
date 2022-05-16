# Overview

The protocol is based on a set of smart contracts that define exactly the rules of the trading protocol.

Content to be written!


## Addresses

Overview of the smart contract addresses

## sTrack

```solidity
Contract sTrack

{
  minting of asset allocation
}
```

## AdminRole

An AdminRole is provided to the Protocol to execute transaction on behalf of the investors

```solidity
Contract AdminRole

{
  modifier onlyAdmin(){};
  function isAdmin(address account) public view returns (bool){};
  function addAdmin(address account) public onlyAdmin{};
}
```

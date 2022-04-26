# Overview

The protocol is based on a set of smart contracts that define exactly the rules of the trading protocol

## Trading capital

A set of smart contracts

```solidity
Contract CollateralInvestor

{
   function mintCollateral(address _externalAddress, uint256 _collAmount) public onlyAdmin returns (bool){};
   function burnCollateral(address _externalAddress, uint256 _collAmount) public onlyAdmin returns (bool){};

   event mintCollateralEvent(address indexed _from, uint256 _amount);
   event burnCollateralEvent(address indexed _from, uint256 _amount);
}
```

## Trading

```solidity
Contract Trading

{

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

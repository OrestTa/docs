
This library provides functionality for computing bit properties of an unsigned integer

## mostSignificantBit
```solidity
  function mostSignificantBit(
    uint256 x
  ) internal returns (uint8 r)
```
The function satisfies the property:
    x >= 2**mostSignificantBit(x) and x < 2**(mostSignificantBit(x)+1)

#### Parameters:
| Name | Type | Description                                                          |
| :--- | :--- | :------------------------------------------------------------------- |
|`x` |  | the value for which to compute the most significant bit, must be greater than 0

#### Return Values:
| Name                           | Type          | Description                                                                  |
| :----------------------------- | :------------ | :--------------------------------------------------------------------------- |
|`r`|  | the index of the most significant bit
## leastSignificantBit
```solidity
  function leastSignificantBit(
    uint256 x
  ) internal returns (uint8 r)
```
The function satisfies the property:
    (x & 2**leastSignificantBit(x)) != 0 and (x & (2**(leastSignificantBit(x)) - 1)) == 0)

#### Parameters:
| Name | Type | Description                                                          |
| :--- | :--- | :------------------------------------------------------------------- |
|`x` |  | the value for which to compute the least significant bit, must be greater than 0

#### Return Values:
| Name                           | Type          | Description                                                                  |
| :----------------------------- | :------------ | :--------------------------------------------------------------------------- |
|`r`|  | the index of the least significant bit
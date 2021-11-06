# Ether and Wei

```
contract EtherUnits {
    uint public oneWei = 1 wei;
    // 1 wei is equal to 1
    bool public isOneWei = 1 wei == 1;

    uint public oneEther = 1 ether;
    // 1 ether is equal to 10^18 wei
    bool public isOneEther = 1 ether == 1e18;
}
```

Transactions' transaction fees are paid with ether.

Similar to how one dollar is equal to 100 cent, one ether is equal to 10^18 wei.

Solidity has denomination modifiers for `uint`s `wei` and `ether`.
if you define `uint oneEther = 1 ether`, value of `oneEther` will be translated internally to `10^18`.

All transaction fees and payments on ethereum happen in the smallest denomination that is a wei. it is not possible to have a smaller denomination than `1 wei`. you can't have `0.1 wei`.

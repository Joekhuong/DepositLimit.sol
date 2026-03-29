# DepositLimit.sol
Remix - Deploy Contract On Base Network DepositLimit.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract DepositLimit {
    function deposit() public payable {
        require(msg.value <= 1 ether, "Too much");
    }
}

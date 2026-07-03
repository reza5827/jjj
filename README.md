// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;
contract SimpleStorage {
uint256 private storedNumber;

event NumberUpdated(uint256 newValue);

function setNumber(uint256 _number) public {
        storedNumber = _number;
   emit NumberUpdated(_number);
}
function getNumber() public view returns (uint256) {
    return storedNumber;
    }
}

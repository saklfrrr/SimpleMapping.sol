# SimpleMapping.sol
SimpleMapping.sol
pragma solidity ^0.8.20;

contract SimpleMapping {
    mapping(address => uint) public balances;

    function setBalance(uint _value) public {
        balances[msg.sender] = _value;
    }
}

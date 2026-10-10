# luna-token
Smart contract and documentation for Luna (LUNA), a fixed-supply ERC-20 token.

 // SPDX-License-Identifier: MIT
pragma solidity ^0.8.24;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract LunaToken is ERC20 {
    constructor()
        ERC20("Luna", "LUNA")
    {
        _mint(msg.sender, 4_000_000 * 10 ** decimals());
    }
}

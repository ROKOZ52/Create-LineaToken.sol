# Create-LineaToken.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract KCInvest is ERC20 {
    constructor() ERC20("KCInvest", "KCI") { //значения KCInvest та KCI ви можете обрати свої
        uint256 power = 10 ** 18; //кількість символів після крапки
        _mint(msg.sender, 1000 * power); // 10000 токенов KCI
    }
}

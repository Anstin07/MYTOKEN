
# NewToken
This is a Solidity smart contract made by me for the last project assessment that implements a basic token called NEWTOKEN (TOKEN_META_CRAFTERS) with functionalities for minting and burning tokens.
# Requirements
The contract has public variables to store details about the token, including its name, abbreviation, and total supply.
A mapping is used to track the token balances of different addresses (address => uint).
The contract includes a mint function that takes an address and a value as parameters. It increases the total supply by the specified value and adds that value to the balance of the sender's address.
The contract also includes a burn function that works in the opposite way of the mint function. It takes an address and a value as parameters, deducts the value from the total supply, and reduces the balance of the sender's address accordingly.
The burn function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount to be burned.If the balance is lesser than the amount to be burned then the balance is not deducted.
# Usage
tokenName: A public variable that represents the name of the token. In this contract, it is set to "TOKEN_META_CRAFTERS".

tokenAbbrv: A public variable that represents the abbreviation of the token. In this contract, it is set to "TKMC".

totalSupply: A public variable that stores the total supply of the token. Initially set to 0, it increases when tokens are minted and decreases when tokens are burned.
balances: A mapping that associates addresses with token balances. Each address's balance is stored as a positive integer.

mint: A function that mints new tokens. It takes an address (_address) and a value (_value) as parameters. It increases the total supply by the specified value and adds that value to the balance of the specified address. 

burn: A function that burns existing tokens. It takes an address (_address) and a value (_value) as parameters. If the balance of the specified address is greater than or equal to the value, it deducts the value from the total supply and reduces the balance of the specified address.



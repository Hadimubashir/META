# META
MyToken Smart Contract README
The MyToken smart contract is designed to create a custom token that adheres to specific requirements. The contract provides functionalities to mint new tokens and burn existing tokens, along with storing essential details about the token.

Contract Overview
The MyToken smart contract includes the following features:

Public Variables:

TokenName: A public string variable representing the full name of the token.
TokenAbbr: A public string variable representing the abbreviation or symbol of the token.
TotalSupply: A public uint variable representing the total supply of tokens in circulation.
Balances Mapping:

balances: A mapping that associates addresses with their corresponding token balances.
Mint Function:

Signature: function mint(address _address, uint _value) public
Functionality: Increases the total supply by _value and adds _value tokens to the balance of the specified _address.
Burn Function:

Signature: function burn(address _address, uint _value) public
Functionality: Decreases the total supply by _value and deducts _value tokens from the balance of the specified _address.
Additional Check: The burn function includes conditionals to ensure that the balance of the _address is greater than or equal to the amount being burned (_value).
How to Use the Contract
Deployment:

Deploy the MyToken contract to the desired Ethereum network using a compatible development environment like Remix or Truffle.
Token Details:

The TokenName variable can be accessed publicly to retrieve the full name of the token.
The TokenAbbr variable can be accessed publicly to retrieve the abbreviation or symbol of the token.
The TotalSupply variable can be accessed publicly to check the total supply of tokens in circulation.
Minting Tokens:

To mint new tokens, call the mint function with the desired _address and _value parameters. This will increase the total supply and add the specified amount of tokens to the balance of the given address.
Burning Tokens:

To burn existing tokens, call the burn function with the desired _address and _value parameters. This will decrease the total supply and deduct the specified amount of tokens from the balance of the given address. The function will perform a check to ensure that the balance of the _address is sufficient to burn the requested amount.

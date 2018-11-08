# BIZ-Token

The BIZ Token contract is used for both BIZ and CRYPTO, two ERC-20 tokens deployed to the Ethereum blockchain on November 7th 2018.

The token details are as follows :

## BIZ

Description       | Value
----------------- | -------------
Token Name        | BIZpaye Crypto
Token Symbol      | BIZ
Total Supply      | 1,000,000,000
Decimal places    | 18
Ethereum Address  | 0xc98d1ed49b8a9f52ea7843f149c1a75e1bdea326

## CRYPTO

Description       | Value
----------------- | -------------
Token Name        | BIZpaye Crypto
Token Symbol      | CRYPTO
Total Supply      | 1,000,000,000
Decimal places    | 18
thereum Address   | 0x7875bafc5d63fa035dea0809c2a57a382d772903

The token contracts are based on standard contracts from https://openzeppelin.org

To give a little background:

ERC-20 is one of several technical standard used for token smart contracts on the Ethereum blockchain.

ERC stands for "Ethereum Request for Comment", and 20 is the number that was assigned to this request some time ago.

At this point the clear majority of tokens issued on the Ethereum blockchain are ERC-20 compliant. Well over 100,000 are presently issued.

The standard defines a common list of rules for Ethereum tokens to follow within the larger Ethereum ecosystem, allowing developers to accurately predict interaction between tokens, including how tokens are transferred between addresses and how data within each token is accessed.

Function required by ERC-20 and implemented within this contract are as follows:

#### totalSupply() - public view returns (uint256 totalSupply)

Get the total token supply

#### balanceOf(address _owner) - public view returns (uint256 balance)

Get the account balance of another account with address _owner

#### transfer(address _to, uint256 _value) - public returns (bool success)

Send _value amount of tokens to address _to

#### transferFrom(address _from, address _to, uint256 _value) - public returns (bool success)

Send _value amount of tokens from address _from to address _to

#### approve(address _spender, uint256 _value) - public returns (bool success)

Allow _spender to withdraw from account, multiple times, up to the _value amount.

If this function is called again it overwrites the current allowance with _value

#### allowance(address _owner, address _spender) - public view returns (uint256 remaining)

Returns the amount which _spender is still allowed to withdraw from _owner

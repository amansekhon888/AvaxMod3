# AmanToken (AMAN)

AmanToken is an ERC20-compatible token deployed on the Ethereum blockchain. It is designed to provide functionality for transferring tokens, burning tokens, and minting new tokens, with additional ownership controls.

## Features

- **ERC20 Compatibility**: AmanToken adheres to the ERC20 standard, enabling seamless integration with existing Ethereum wallets, exchanges, and smart contracts.
- **Token Burning**: Token holders can burn their tokens, reducing the total token supply.
- **Token Minting**: Only the contract owner has the ability to mint new tokens, providing control over token issuance.
- **Ownership Controls**: The contract inherits from OpenZeppelin's Ownable, allowing the contract owner to execute certain privileged functions.

## Deployment

The AmanToken contract is deployed on the Ethereum mainnet with the following parameters:

- **Token Name**: AmanToken
- **Token Symbol**: AMAN
- **Initial Supply**: 1,000,000 tokens (adjustable)
- **Decimals**: 18 (adjustable)

## Usage

### Initial Deployment

When deploying the AmanToken contract, provide the address of the initial owner. The initial owner will receive the entire initial token supply.

### Minting Tokens

The contract owner can mint new tokens by calling the `mint` function, specifying the recipient's address and the amount of tokens to mint.

### Burning Tokens

Token holders can burn their own tokens by calling the `burn` function, specifying the amount of tokens to burn.

### Transferring Tokens

Token holders can transfer tokens to other addresses by calling the `transfer` function, specifying the recipient's address and the amount of tokens to transfer.

## Security

- Ensure that only trusted addresses have ownership of the contract to prevent unauthorized minting or other privileged actions.
- Use caution when burning tokens, as burned tokens cannot be recovered.
- Verify contract code and perform thorough testing before interacting with the contract in a production environment.

## License

AmanToken is licensed under the [MIT License](LICENSE).

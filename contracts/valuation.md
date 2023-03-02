# Valuation

![Valuation Module](../../images/valuation.png)

**Valuation** module measures the value of a DeFi position by using tokenization with external oracles.

## Tokenization

`Tokenization` turns a DeFi position into a token (i.e., ERC1155) so that it can be easily valuated and collateralized.

## Write Methods

### setCustomTokenFactor

`function setCustomTokenFactor(uint256 _tokenTypeOrId, uint _collateralFactor, uint _debtFactor)`

Set token collateral/debt custom factor.

- `_tokenTypeOrId`: If erc20 asset, token id. If factorial asset, 24bit tokenType.
- `_collateralFactor`: The collateral factor of token/wrapping sepc.
- `_debtFactor`: The debt factor of token/wrapping spec.

### wrap

`function wrap(uint24 _wrapperType, bytes calldata _param)`

Wrap token/assets to ERC1155 factorial token.

- `_wrapperType`: The 24-bit wrapper type. Not underlying asset type.
- `_param`: The parameter using specific wrapping contract.

### unwrap

`function unwrap(uint _tokenId, uint _amount)`

Unwrap token/assets from ERC1155 factorial token.

- `_tokenId`: The ERC1155 factorial token id.
- `_amount`: The amount of token to unwrap. If NFT token, it should be 1.

## View Methods

### getValue

`function getValue(uint _tokenId, uint _amount) external view override returns (uint)`

Return value of token by id and amount.

- `_tokenId`: The token ID to be valued.
- `_amount`: The amount of token to be valued. If NFT token, it should be 1.

### getValueAsCollateral

`function getValueAsCollateral(address _lendingProtocol, uint _tokenId, uint _amount) external view returns (uint)`

Return token value as collateral. For debt token wrapper.

- `_lendingProtocol`: The lending protocol address. This is for custom factor.
- `_tokenId`: The token ID to be valued.
- `_amount`: The amount of token to be valued. If NFT token, it should be 1.

### getValueAsDebt

`function getValueAsDebt(address _lendingProtocol, uint _tokenId, uint _amount) external view returns (uint)`

Return token value as debt. For debt token wrapper.

- `_lendingProtocol`: The lending protocol address. This is for custom factor.
- `_tokenId`: The token ID to be valued.
- `_amount`: The amount of token to be valued. If NFT token, it should be 1.

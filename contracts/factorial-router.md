# Factorial Router

**Factorial Router** is to route the users transaction request to the corresponding app on Factorial.

## Write Methods

### execute

`function execute(address _target, bytes calldata _data)`

Call to the target using the given data.

### executeBatch

`function executeBatch(uint256 _maximumLoss, address[] calldata _targetArray, bytes[] calldata _dataArray)`

Call batch to the target using the given data array.

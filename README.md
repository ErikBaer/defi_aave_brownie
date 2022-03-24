1. Swap our ETH for WETH
2. Deposite some ETH (WETH) into AAVE
3. Borrow some aset with the ETH collateral
    1. Sell that borrowed asset. (Short selling)
4. Repay everything back

Testing:
Integration test: Kovan
Unit tests: Mainnet-fork (Mock all of Mainnet!)

This demo is based on the chainlink-mix repo as presented in these tutorials from Chainlink: https://github.com/smartcontractkit/full-blockchain-solidity-course-py

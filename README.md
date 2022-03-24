# defi_aave_brownie
This project is a demo of a back-end written in python / brownie and solidity, utilizing several smart-contracts in order to execute staking and borrowing on the defi-platform aave which is deployed to the Etherium-Blockchain. 

To connect to the aave trading platform and execute the example trades, just install brownie and enter the following information into the file sample.env, then rename it to .env :

WEB3_INFURA_PROJECT_ID, ETHERSCAN_TOKEN, PRIVATE_KEY

Then run the command ```brownie run scripts/get_weth.py``` in order to programmatically swap some Ether for WETH, which is the currency required for deposits on aave. After that, just run ```brownie run scripts/aave_borrow.py``` to execute the trades and see the full functionality in action:

1. Swap our ETH for WETH
2. Deposite some ETH (WETH) into AAVE
3. Borrow DAI-Coin with the ETH collateral
4. Repay everything back

Testing:
Integration test: Kovan
Unit tests: Mainnet-fork (Mock all of Mainnet!)

This demo is based on the chainlink-mix repo as presented in these tutorials from Chainlink: https://github.com/smartcontractkit/full-blockchain-solidity-course-py

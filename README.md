# PayWizard
PayWizard is the Paymasters master. Sorcerer of AA. Manage a fleet of paymasters using JIT liquidity provisioning. 

<img width="904" alt="pay-wizard" src="https://github.com/user-attachments/assets/186ee0d6-5345-4326-8c65-42d3b7c23278" />


This is an entry to EthSydney 2024 hackathon, building toward a solution that provides a seamless UX by covering transaction costs within system(s). This project requires a ChainLink account and $LINK (testnet is suggested) and the token your project is to be deployed (ETH, Polygon, Optimism..). The stage reached allows for wallets to transact with the PayWizard, and recieve a full gas refund. 

Steps to test drive PayWizard (hackathon entry).

1. Upon deploying the PayWizard Smart Contract, set minWaitPeriodSeconds for example to 60 (interval 60s). Set this to a value that best suits the needs of your application (note: this is a cost to your application in $LINK).

2. Trigger `setWatchList` with values (for demonstration purposes you can use one or many wallet addresses), minimum balance per account, and amount to top up per account.

3. Once complete, navigate to ChainLink `https://automation.chain.link/new-custom-logic` and register the custom smart contract. 

- Project name
- $LINK starting balance 2
- Add any custom details required / optional

4. Wait for completion and then select the new upkeep when shown in the page.

5. Copy the forwarder address and add this via the setForwarderAddress in the Smart Contract to connect ChainLink with the PayWizard contract.

6. Now you can experiment with making transactions to adjust balances to trigger automatic topups of funds.


Additional:

Example dashboard of PayWizard running on Sepolia network, where a condition is met and the funds are sent accordingly to the rules in place.

https://automation.chain.link/sepolia/90122082278454152060304220536370708940286860125896525211271584568390900145237

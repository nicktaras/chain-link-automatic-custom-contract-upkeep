# PayWizard
PayWizard is the Paymasters master. Sorcerer of AA. Manage a fleet of paymasters using JIT liquidity provisioning. 

Steps to test drive PayWizard.

1. Upon deploying the PayWizard Smart Contract, set minWaitPeriodSeconds for example to 60 (interval 60s). Set this to a value that best suits the needs of your application (note: this is a cost to your application in $LINK).

2. Trigger `setWatchList` with values (for demonstration purposes you can use one or many wallet addresses), minimum balance per account, and amount to top up per account.

3. Once complete, navigate to ChainLink `https://automation.chain.link/new-custom-logic` and register the custom smart contract. 

- Project name
- $LINK starting balance 2
- Add any custom details required / optional

4. Wait for completion and then select the new upkeep when shown in the page.

5. Copy the forwarder address and add this via the setForwarderAddress in the Smart Contract to connect ChainLink with the PayWizard contract.

6. Now you can experiment with making transactions to adjust balances to trigger automatic topups of funds.

To take this project further:

- Front end. 

An application is required to help end users trigger events and see live information as changes occur per system interval.

- Smart Contract.

Further testing is required to ensure the added features and contract as a whole is secure and optimised.

Example contract scenarios are needed to help illustrate the full process(es) and uses of this solution.

- Backend.

Backend functionality is required to inform the owner when funds are low in $LINK and ETH for the project as a whole to help ensure stability. 

Additional:

Example dashboard of PayWizard running on Sepolia network, where a condition is met and the funds are sent accordingly to the rules in place.

https://automation.chain.link/sepolia/90122082278454152060304220536370708940286860125896525211271584568390900145237
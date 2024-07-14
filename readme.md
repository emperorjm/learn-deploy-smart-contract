This file lists all the commands you'll need to execute during our hands-on workshop for developing smart contracts on the Archway platform.
Follow each command carefully to set up, create, modify, deploy, and interact with your smart contract.

1. Create new account: `archway accounts new [ACCOUNT-NAME]`

2. Change to your home directory: `cd ~`

3. Create new project: `archway new [PROJECT-NAME]`

4. Show project configuration: `archway config show`

5. Configure project: `archway config set KEY VALUE`

6. To compile your contracts execute: `archway contracts build`

7. Execute the following to store your contract on chain: `archway contracts store [CONTRACT] --from [my-account]`

8. To create an instance of a contract from a deployed WASM executable execute: `archway contracts instantiate [contract-name] --args '{"count":0}'`

9. To execute a transaction to increment count: `archway contracts execute [contract-name] --args '{"increment": {}}'`

10. To execute a query to retrieve the current count: `archway contracts query smart [contract-name] --args '{"get_count": {}}'`

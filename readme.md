This file lists all the commands you'll need to execute during our hands on workshop for developing smart contracts on Archway.

1. Create new account: `archway accounts new mywallet`

3. Change to your home directory: `cd ~`

4. Create new project: `archway new incrementproject`

   - Select a chain to use: `Archway Testnet`
   - Choose a name for your contract: `increment`
   - Choose a starter template: `Increment`
   - Which version do you want to generate? `full`

5. Change to your project folder: `cd incrementproject`
6. To compile your contract execute: `archway contracts build`

7. Execute the following to store your contract on chain: `archway contracts store increment --from mywallet`

8. To create an instance of the contract execute: `archway contracts instantiate increment --args '{"count":0}'`

9. Check to see what is the initial count: `archway contracts query smart increment --args '{"get_count": {}}'`

10. To increment the count by one, execute: `archway contracts execute increment --args '{"increment": {}}'`

11. Query the count value to see if it was updated: `archway contracts query smart increment --args '{"get_count": {}}'`

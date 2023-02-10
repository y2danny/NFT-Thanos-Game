# NFT-Thanos-Game :video_game:
A multiplayer NFT card game built on the Avalanche network.
## :warning: Please use the chrome browser with the metamask wallet to run. 
Thanos Game is a multiplayer game running with smart contracts deployed on the avalanche network.
It features a simple interaction mechanism initialized by approving transaction with your metamask wallet.
You would need 2 players to actually play the game but you can individually test around the creating and joining battle sequence, register and assign your wallet id a name, view created battles by other players as well as change backgrounds and attempt to join a battle.
# Instructions on setting up your blockchain or web3 environment :hammer_and_pick:
1. `cd web3`
2. `npx hardhat` -> y → typescript → enter → enter
3. `npm install @openzeppelin/contracts dotenv @nomiclabs/hardhat-ethers` + Hardhat packages `npm install --save-dev "hardhat@^2.12.0" "@nomicfoundation/hardhat-toolbox@^2.0.0"`
4. Install [Metamask] (https://metamask.io/) wallet
5. Turn on the testnet mode by: opening up the Metamask extension -> click the hamburger menu on the top right -> go to advanced -> turn on the testnet mode
6. Fund your wallet from the [Avax Faucet] (https://faucet.avax.network/)
7. Create a `.env` file and specify a PRIVATE_KEY variable.
8. To get to the private key, do the following steps:
Open up the Metamask extension -> click the hamburger menu on the top left -> go to security and privacy -> click show recovery phase -> enter your password -> copy the phrase -> go to [wallet.avax.network] (https://wallet.avax.network/) -> click access wallet -> choose mnemonic key phrase -> paste what the words we’ve copied from Metamask -> on the sidebar click manage keys -> view c-chain private key -> copy -> paste it in the `.env` file
9. Copy the `hardhat.config.ts` file from the GitHub repo
10. Copy the `deploy.ts` script from the GitHub repo
11. Copy the `AvaxGods.sol` smart contract code from the GitHub repo
12. Compile the contract by running the `npx hardhat compile` command
Deploy the smart contract on the Fuji test network by running the `npx hardhat run scripts/deploy.ts --network fuji` command Move the `/artifacts/contracts/AVAXGods.json` file to the /contract folder on the frontend Copy the address of the deployed contract from the terminal and paste it into the `/contract/index.js` file of the frontend application


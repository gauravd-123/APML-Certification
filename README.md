# APML certification using Blockchain Technology

### `Steps`

1. Install the [Metamask extension](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=en) in your chrome browser.<br>
After logging in select **Ropsten Test Network** (see to it that you have some test ethers).


2. Copy the text from **[smart_contract.txt](https://github.com/nitinskumavat/blockchain-certs/blob/master/smart_contract.txt)**

3. Paste this in **Remix ide** .<br>

4. You should select **Injected Web3** as an Environent inside the RemixIde.<br>

5. Then Compile and Deploy your smart contract.<br>

6. Copy the **Address** of deployed contract.<br> 
And replace the address value in **[src/config.js](https://github.com/nitinskumavat/blockchain-certs/blob/master/src/config.js)** with your contract address.<br>


7. In the project directory run:

### `npm install`

This will install all the dependencies

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.


### `Working`

## Writing the contract:
Smart contracts are programs stored on a blockchain that run when predetermined conditions are met. They typically are used to automate the execution of an agreement so that all users can be immediately certain of the outcome, without any intermediary's involvement or time loss.<br>
![Smart contract](https://github.com/gauravd-123/APML-Certification/blob/main/smart%20cont%20img.png)<br>

### So our smart contracts does the following things:
1. Checks the input given by the user,
2. Maps the data to required files(here to our certificates),
3. Initializes the contract by checking the address of owners or        users trying to use the contract,
4. Finally gives us the contract address which we have to use it in      our frontend files.


### Deploying the contract
To deploy our contract, we are using **Remix ide** which has an inbuilt solidity compiler. Firstly, we've to select the appropiate compiler version, compiler language and then click on **compile**<br>
![Deployment](https://github.com/gauravd-123/APML-Certification/blob/main/Deployment%20img.png)<br>
At last we get our deployed contract's address, which we've to paste in our config.js file.

### Writing the web3.js file
Web3 is a collection of libraries which allows us to interact with a local or remote Ethereum node using an HTTP, IPC connection, etc.<br>
![Web3 file](https://github.com/gauravd-123/APML-Certification/blob/main/Web3%20file%20img.png)<br>
Here we just have to declare a constant variable(which is immutable). We've to use the given provider i.e. **Metamask**, establishing the port 8545 as the bridge between web and blockchain.
Now we can access the blockchain artifacts through web3 object.

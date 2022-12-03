# hardhat getting started

Docs [here](https://hardhat.org/hardhat-runner/docs/getting-started#quick-start)

* create project directory
* install hard hat as a dev dependency, which means you need to npm init first
    * npm install --save-dev hardhat
* Enable the following plug in
    * npm install --save-dev @nomicfoundation/hardhat-toolbox
    * add the plugin dependency to the config
* tip - visual studio hardhat extension

Stupid WSL Trick - npm install is exceedingly slow or unreliable when
the host OS is specified as the nameserver. Setting it to say 8.8.8.8
immensly improves things.


Deploy to Ganache

* Edit .env file to add endpoint and private key. Here I seed ganache with the
same phrase each time so my addresses etc are consistent. Obviously this is not 
a regime you would ever use for non-learning projects.
    * Based on [this](https://github.com/abdulhakim-altunkaya/SOLIDITY-web3-youtube/blob/main/12_hardhat_ganache/n_hardhat_ganache.txt)
* Deploy via `npx hardhat run ./scripts/deploy.js --network localganache`
    

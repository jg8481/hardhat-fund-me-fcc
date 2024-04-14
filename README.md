These are my notes while working on [Patrick's Javascript Blockchain/Smart Contract FreeCodeCamp Course](https://www.youtube.com/watch?v=gyMwXuJrbJQ).

- On April 14, 2024 successfully compiled and deployed the following "Hardhat smart contract deployment and local Hardhat Node" example code using `hardhat deploy` on a locally installed Hardhat fake blockchain node. I used a similar build automation pipeline approach found in my [hardhat-simple-storage-fcc](https://github.com/jg8481/hardhat-simple-storage-fcc) fork, but it now has a reduced and more efficient sequence of steps because of the included `hardhat deploy` code.

- On April 14, 2024 successfully compiled and deployed the following 2 examples to the following address on Sepolia Testnet using my own Alchemy Sepolia Testnet RPC.

  - https://sepolia.etherscan.io/address/0xa94f822c3e3fd90e914fd5d848a73dd444425d67
  - https://sepolia.etherscan.io/address/0x7b02d0d59feb4f8f4975db3f3da91d65e89fdc0d

---
### Technical Requirements

Check the basic technical requirements from Patrick's original GitHub repo. For convenience, MacOS users can run `bash ./Lesson7CodeSessions_start-deployment-scripts.sh Install-Tools-On-MacOS-Or-Linux` from the root of this repo to help quickly install the required tools.

### Quick Start Script

After the basic technical requirements are installed and working, then you can run the `bash ./Lesson7CodeSessions_start-automation-build-pipeline.sh` script. This automation script will start a sequence of the scripts listed below, and is meant to behave like a typical build pipeline.

### Current Toolkit Capabilities
```
You can view just this help menu again (without triggering any automation) by running 'bash ./Lesson7CodeSessions_start-deployment-scripts.sh -h' or 'bash ./Lesson7CodeSessions_start-deployment-scripts.sh -h --help'.

bash ./Lesson7CodeSessions_start-deployment-scripts.sh Stop-Local-Blockchain-Nodes-Clean-Environment
bash ./Lesson7CodeSessions_start-deployment-scripts.sh Install-Tools-On-MacOS-Or-Linux
bash ./Lesson7CodeSessions_start-deployment-scripts.sh Start-Deployment-On-A-Specific-Network hardhat
bash ./Lesson7CodeSessions_start-deployment-scripts.sh Start-Deployment-On-Real-Ethereum-Testnet
bash ./Lesson7CodeSessions_start-deployment-scripts.sh Start-Hardhat-Test

If you're running this for the first time run the following before running any of these scripts.

bash ./Lesson7CodeSessions_start-deployment-scripts.sh Install-Tools-On-MacOS-Or-Linux

Then you can run the following combined commands in your terminal to deploy the contract to the Hardhat local blockchain node.

bash ./Lesson7CodeSessions_start-deployment-scripts.sh Stop-Local-Blockchain-Nodes && bash ./Lesson7CodeSessions_start-deployment-scripts.sh Start-Deployment-On-A-Specific-Network hardhat
```


# NuCypher Hackathon Guidelines

## Technologies

### Proxy Re-encryption
  * [Whitepaper](https://github.com/nucypher/whitepaper/blob/master/whitepaper.pdf) - A proxy re-encryption network to empower privacy in decentralized systems
  * [Umbral Specification](https://github.com/nucypher/umbral-doc/blob/master/umbral-doc.pdf) - if you want to look at the math behind Umbral
  * [Presentation Slides](https://github.com/nucypher/slides/blob/ETHSingapore/slides.pdf) explaining proxy re-encryption and NuCypher
  * [pyUmbral](https://github.com/nucypher/pyUmbral/) - Python reference implementation of Umbral, our threshold proxy re-encryption scheme
  * [NuCypher Network](https://github.com/nucypher/nucypher/) - the proxy re-encryption network itself 
 
### Fully Homomorphic Encryption
  * [nuFHE](https://github.com/nucypher/nufhe/) - a GPU-accelerated fully homomorphic encryption library
  * [Sputnik](https://github.com/nucypher/sputnik/) - an assembly language and interpreter built using nuFHE to execute the first-ever fully homomorphic smart contract


## Community Links
* [Website](https://nucypher.com/)
* [Discord](https://discord.gg/7rmXa3S) - our main development channel; feel free to jump in with technical questions for our team


## Buidling

### Documentation
Check out our [development guide](https://nucypher.readthedocs.io/en/latest/) to start buidling with NuCypher.
 
### Running a Local Network
Simulate the NuCypher network locally by running a [local development fleet](https://nucypher.readthedocs.io/en/latest/demos/local_fleet_demo.html#local-development-fleet-testing). 

### Sample Demos
Sample demo applications are available:
* [Finnegan's Wake](https://nucypher.readthedocs.io/en/latest/demos/finnegans_wake_demo.html)
* [Heartbeat Demo](https://nucypher.readthedocs.io/en/latest/demos/heartbeat_demo.html)

### Possible Tasks
* The best task is to build some end-to-end encrypted multi-user app which _you_ think is best to build using NuCypher
* Making a UI for staking. This requires understanding [token issuance model](https://blog.nucypher.com/nucypher-staking-economics-a7bb56b20716). If you have time, you may look at the [smart contracts](https://github.com/nucypher/nucypher/blob/master/nucypher/blockchain/eth/sol/source/contracts/MinersEscrow.sol) which control the staking parameters and their corresponding Python wrappers
* Wrapper to interact with NuCypher network from Go, node.js, ...
* Extension to interact with NuCypher network in browsers

Still, it is best is to work on something which _you_ are interested in. Be it a decentralized e2e encrypted group 
chat, or an app to share your medical data, or maybe something that hasn't even been thought of as yet!

**HAPPY HACKING!**


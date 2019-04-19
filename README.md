# NuCypher Hackathon Guidelines

Hi NuCypherinos, we're currently in the midst of two hackathons: ETH Cape Town and Ethereal Virtual Hackathon. Check below for the relevant details.

## ETH Cape Town

Welcome to the Mother City! We have a $1,250 bounty for the best NuCypher-related tooling and a $1,250 bounty for the best application built with NuCypher technology.

## Ethereal Virtual Hackathon

Welcome to the Ethereal Virtual Hackathon! We have two $2,500 bounties: for the best NuCypher-related [tooling](https://github.com/nucypher/hackathon/issues/5) and the [best application](https://github.com/nucypher/hackathon/issues/4) built with NuCypher technology.

## Technologies

### Proxy Re-encryption
  * [NuCypher Network](https://github.com/nucypher/nucypher/) - the proxy re-encryption network itself 
  * [pyUmbral](https://github.com/nucypher/pyUmbral/) - Python reference implementation of Umbral, our threshold proxy re-encryption scheme
  * [Presentation Slides](https://github.com/nucypher/slides/blob/ETHSingapore/slides.pdf) explaining proxy re-encryption and NuCypher
  * [Whitepaper](https://github.com/nucypher/whitepaper/blob/master/whitepaper.pdf) - A proxy re-encryption network to empower privacy in decentralized systems
  * [Umbral Specification](https://github.com/nucypher/umbral-doc/blob/master/umbral-doc.pdf) - if you want to look at the math behind Umbral
 
### Fully Homomorphic Encryption
  * [NuFHE](https://github.com/nucypher/nufhe/) - a GPU-accelerated fully homomorphic encryption library
  * [Sputnik](https://github.com/nucypher/sputnik/) - an assembly language and interpreter built using NuFHE to execute the first-ever fully homomorphic smart contract


## Community Links
* [Website](https://nucypher.com/)
* [Discord](https://discord.gg/7rmXa3S) - our main development channel; feel free to jump in with technical questions for our team


## Buidling

### Documentation
Check out our [development guide](https://nucypher.readthedocs.io/en/latest/) to start buidling with NuCypher.
 
### Connecting to a Fleet

#### Running a Local Network
Simulate the NuCypher network locally by running a [local development fleet](https://nucypher.readthedocs.io/en/latest/demos/local_fleet_demo.html#local-development-fleet-testing). 

#### Connecting to the DevNet

Alternatively, instead of running a local nucypher development fleet of Ursulas, 
you can connect your node to our dedicated hackathon devnet.

See the network status here: http://13.59.39.174:12500/

```
(nucypher) $ nucypher ursula init --federated-only
...
(nucypher) $ nucypher ursula run --network devnet --teacher-uri 18.222.119.242:9151
```

For more detailed information see our official [documentation](https://docs.nucypher.com/en/latest/guides/ursula_configuration_guide.html)

### Sample Demos
Sample demo applications are available:
* [Finnegan's Wake](https://nucypher.readthedocs.io/en/latest/demos/finnegans_wake_demo.html)
* [Heartbeat Demo](https://nucypher.readthedocs.io/en/latest/demos/heartbeat_demo.html)

**HAPPY HACKING!**

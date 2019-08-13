# NuCypher Hackathon Guidelines

Hi NuCypherinos,

## ETHBerlin

 Welcome to ETHBerlin Zwei!

The NuCypher network facilitates end-to-end encrypted data sharing for distributed apps and protocols. Use our tools and network to build privacy into your Dapp and earn your share of a $2500 USD bounty pool.

### To Qualify for the NuCypher Bounty
* Your project must be open-sourced
* Your project must be submitted before the official end time (check with ETHBerlin organizers for end time)
* You must use one of NuCypher's technologies in your hack

### Judging Criteria
* Novelty of Use Case
* Difficulty of Technical Implementation
* Usefulness of the Submission

### Prizes
Up to $2500 USD that can be distributed as we (the judges) see fit.


## Resources
We have a workshop scheduled for 2 pm, August 23rd just after lunch!!

### Proxy Re-encryption
* Our development guide to start building with NuCypher: https://docs.nucypher.com
* NuCypher Network - the proxy re-encryption network itself https://nucypher.dev/nucypher

### Fully Homomorphic Encryption
* NuFHE - a GPU-accelerated fully homomorphic encryption library https://nucypher.dev/nufhe

### Discord and IRL Help
If you need support with your hack or simply want to jam on some ideas, we'll be around all week at ETHBerlin and Dappcon or use Discord. Jump in #hackathons and start asking away https://discord.gg/7rmXa3S

### NuCypher Forum
A forum where we post and discuss NuCypher technical issues and other ongoing updates and changes. https://forum.nucypher.com

Some ideas from past hacks: https://blog.nucypher.com/ethny-nucypher

### Connecting to a Fleet

#### Running a Local Network
Simulate the NuCypher network locally by running a [local development fleet](https://docs.nucypher.com/en/latest/demos/local_fleet_demo.html#local-development-fleet-testing). 

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
* [Finnegan's Wake](https://docs.nucypher.com/en/latest/demos/finnegans_wake_demo.html)
* [Heartbeat Demo](https://docs.nucypher.com/en/latest/demos/heartbeat_demo.html)

**HAPPY HACKING!**

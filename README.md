# Hackathon guidelines

# Possible tasks
* The best is to build some end-to-end encrypted multi-user app which _you_ think is the best to build using NuCypher;
* Enabling NuCypher to do conditional policies (e.g. on payment, if `1` is returned by a solidity method etc). This will require understanding of [NuCypher source code](https://github.com/nucypher/nucypher);
* Making a UI for staking. This requires understanding [token issuance model](https://blog.nucypher.com/nucypher-staking-economics-a7bb56b20716). If you have time, you may look at the [smart contracts](https://github.com/nucypher/nucypher/blob/master/nucypher/blockchain/eth/sol/source/contracts/MinersEscrow.sol) which control the staking parameters and their corresponding Python wrappers.

Still, the best is to work on something which _you_ think is the best to work on. Be it decentralized e2e encrypted group chat, or an app to share your medical data, or maybe something we cannot even think of yet!

# Useful links
* [Mock-net](https://github.com/nucypher/mock-net/) - you can start here to familiarize yourself with main concepts;
* [Proxy re-encryption library Umbral](https://github.com/nucypher/pyUmbral/);
* [Umbral spec](https://github.com/nucypher/umbral-doc/) - if you want to look at the math behind Umbral;
* [NuCypher re-encryption network](https://github.com/nucypher/nucypher/) - The re-encryption network itself;
* [nuFHE](https://github.com/nucypher/nufhe/) - A GPU-accelerated fully homomorphic encryption library;
* [Sputnik](https://github.com/nucypher/sputnik/) - An assembly language and interpreter used to execute the first-ever fully homomorphic smart contract;
* [Slides](https://github.com/nucypher/slides/blob/master/slides.pdf) explaining proxy re-encryption and NuCypher.

# Community Links:
* Our main development channel on [Discord](https://discord.gg/7rmXa3S) - feel free to jump in with technical questions;
* Our [website](https://nucypher.com/);
* [Whitepaper](https://www.nucypher.com/whitepapers/english.pdf);
* [Token economics paper](https://github.com/nucypher/mining-paper/blob/master/mining-paper.pdf);


# Where to start
First of all, go to the [mock-net](https://github.com/nucypher/mock-net/) repository and take your time to follow `umbral-demo.py`.
Follow the installation instructions in the repository `README`.

If you want to build with "real" nucypher network, do the following:
```
git clone https://github.com/nucypher/nucypher.git  # clone NuCypher repository
cd nucypher
git checkout federated  # We need a federated branch which isn't using blockchain
pipenv install --dev --three --skip-lock
pipenv shell
pip3 install -e .
# ok, now you have nucypher installed in virtual environment

# prepare to run several nodes locally
cd examples
mkdir examples-runtime-cruft
# run the following in several terminals
python3 run_ursula_with_rest_and_dht_but_no_mining.py 3500  # <- seed node
python3 run_ursula_with_rest_and_dht_but_no_mining.py 3501 3500
python3 run_ursula_with_rest_and_dht_but_no_mining.py 3502 3500

# now get some text to re-encrypt and run the demo
wget https://www.gutenberg.org/files/2701/old/moby10b.txt
python3 finnegans-wake-federated.py moby10b.txt 3501
```

The mock-net repository also has a toy version of "network" which is just an object you interact with instead of the real network

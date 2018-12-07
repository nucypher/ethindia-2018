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
If you want to build with "real" nucypher network, do the following:
```
virtualenv _venv -p python3
source _venv/bin/activate
pip3 install pip3 install git+https://github.com/nucypher/nucypher.git@federated

git clone https://github.com/nucypher/nucypher.git
cd nucypher
git checkout federated
cd examples/finnegans_wake_demo
./download_finnegans_wake.sh
python3 finnegans-wake-concise-demo.py
```

Finnegan's Wake demo re-encrypts every line of Finnegan's Wake using NuCypher for that. There is another [Heartbeat Demo](https://github.com/cygnusv/nucypher/tree/heart_of_the_sunrise/examples/heartbeat_demo) which you may want to check.

If you want to do low-level stuff without getting into the weeds of NuCypher code, you can use "mock-net" instead of the real network and change its code when you need. Go to the [mock-net](https://github.com/nucypher/mock-net/) repository and take your time to follow `umbral-demo.py` or `test_demo.py`, as well as you're free to modify `nucypher.py` which is the "mock network" itself.
After cloning, you can install the dependencies by running:
```
pipenv install --dev --three --skip-lock
```

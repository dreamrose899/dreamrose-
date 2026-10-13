# DreamRose (DRSE)

Open-source Scrypt coin forked from Dogecoin Core, with merged mining (AuxPoW) support for Dogecoin and Litecoin.

> Pre-launch. All parameters are proposals open to miner and pool feedback.

## Parameters
- Algorithm: Scrypt (AuxPoW)
- Block time: 60s (120s under discussion)
- Max supply: 21,000,000 DRSE
- Reward: 5 DRSE, halving every 2,100,000 blocks (~4 years)
- Premine: 1% (210,000 DRSE)

## Block reward split
- First 4 years: miners 90%, pool bonus 4%, founder 2%, dev 2%, community 2%.
- After first halving: miners 94%, pool bonus 4%, dev 1%, community 1%, founder 0%.

## Premine
- 100,000: early pool bonus (first 10,000 blocks)
- 60,000: listings and marketing (multisig)
- 50,000: audit and infrastructure (multisig)

All addresses will be published before mainnet.

## Build
```
./autogen.sh
./configure --without-gui
make -j$(nproc)
```

## Run (testnet)
```
./src/dreamrosed -testnet -daemon
```

## For pool operators
Uses the same `getauxblock` RPC as Dogecoin. Feedback wanted on multi-output coinbase, percentages and block time.

## Roadmap
Genesis block, reward code and tests, public testnet, pool feedback, security review, mainnet.

## Contributing
Pull requests welcome. Keep consensus changes in separate commits.

## License
MIT, same as Dogecoin Core.
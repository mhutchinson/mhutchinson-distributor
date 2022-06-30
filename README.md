# mhutchinson's Checkpoint Distributor

This repository distributes witnessed checkpoints for the following logs:

 * [sum.golang.org](./distributor/logs/3e9617dce5730053cb82f0481b9d289cd3c384a9219ef5509c91aa60d214794e)
 * [Pixel 6 BT](./distributor/logs/542f1d5cf18cac38a8921be403c6b620eae2c06d5f0d15a050cfe98e8202d02d)
 * [f-secure-foundry/armory-drive-log](./distributor/logs/50dfc1866b26a18b65834743645f90737c331bc5e99b44100e5ca555c17821e3)
 * [Rekor / SigStore](./distributor/logs/e09045bedf247c449acf3fe26375fb5a1b81110546e797d520cb1133f27fbd1a)
 * [LVFS](./distributor/logs/74ea854e2a0cdf00544673d488ef95955b56cdcaa23ec382e437b89a20985bd4)
 * [AlCutter/serverless-test/log](./distributor/logs/48e2ecbc0474292d790906a13023a76a93e0f3706f86f9f939bd91b7dcfde4a6)

The format of the checkpoint files is `checkpoint.N`, where `N` is the number of witness signatures.
Lower `N` values will be fresher, but higher `N` values have been witnessed by more parties.

## Adding more logs or witnesses

Additional logs or witnesses can be added by proposing a PR that updates [distributor config](./distributor/config.yaml).
More witnesses are always welcome!


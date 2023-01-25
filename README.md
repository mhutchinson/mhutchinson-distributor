# mhutchinson's Log Checkpoint Distributor

This is a proof of concept distributor for log checkpoints that have been witnessed.
If none of these terms make sense to you:
  * [Distributor](https://github.com/google/trillian-examples/tree/master/serverless/deploy/github/distributor)
  * [Witness](https://github.com/google/trillian-examples/tree/master/witness)
  * [Log](https://github.com/google/trillian)
  * [Checkpoint](https://github.com/transparency-dev/formats)

For a list of logs and witnesses supported by this distributor, see [generated docs](./distributor/logs).
The format of the checkpoint files is `checkpoint.N`, where `N` is the number of witness signatures.
Lower `N` values will be fresher, but higher `N` values have been witnessed by more parties.

## Adding more logs or witnesses

Additional logs or witnesses can be added by proposing a PR that updates [distributor config](./distributor/config.yaml).
More witnesses are always welcome!


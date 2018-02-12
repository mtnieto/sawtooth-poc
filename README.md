# Hyperledger Sawtooth - Proof of Concept


### Create genesis block
The first validator created in a new network must load a genesis block on creation to enable other validators to join the network. Prior to starting the first validator, run the following commands to generate a genesis block that the first validator can load:

```
$ sudo sawadm keygen
$ sawtooth keygen --key-dir ~/sawtooth
$ sawset genesis --key ~/sawtooth.priv
$ sawadm genesis config-genesis.batch
````

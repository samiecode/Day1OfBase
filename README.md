## GREETER CONTRACT

 URL: https://sepolia.basescan.org/address/0x4f6681122d703a3485f24d899416dadbc3fb32aa


## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Verify

```shell
$ forge verify-contract $GREETER_CONTRACT_ADDRESS ./src/Greeter.sol:Greeter --chain base-sepolia --verifier etherscan --verifier-api-key $ETHERSCAN_API_KEY --verifier-url $BASESCAN_API_URL --constructor-args $(cast abi-encode "constructor(string)" "Hello Base Builders")

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

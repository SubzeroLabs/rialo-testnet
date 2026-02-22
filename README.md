# Rialo Testnet Genesis Configuration

This repository contains the genesis configuration files for the Rialo testnet, including validator public keys and network configuration data used during network initialization.

## Repository Structure

```
.
├── common-config.yaml              # Common genesis configuration
├── genesis-signatures.json         # Genesis block signatures
└── [validator-name]/              # Validator-specific directories
    ├── authority-keypair.pub.json
    ├── network-keypair.pub.json
    ├── protocol-keypair.pub.json
    ├── signing-keypair.pub.json
    ├── validator-addr.txt
    ├── validator-state-sync-addr.txt
    └── [validator-name]-signature.json
```

## Testnet Validators

The following validators are participating in the Rialo testnet:

- node0.testnet.rialo.io
- node1.testnet.rialo.io
- node2.testnet.rialo.io
- fp-rialo-testnet-validator.felixinfra.xyz
- rialo-testnet-validator.bharvest.io
- rialo-testnet-validator.keplr.app
- rialo-testnet-validator.nodeinfra.com
- rialo-testnet-validator.nodes.guru
- rialo-tn-val.citadel.one
- rialo.validator.infstones.com
- testnet-validator.rialo.p2p.org
- val.rialo.testnet.pops.one
- validator.rialo.staking.banansen.dev

## Configuration Files

### common-config.yaml

Contains the shared genesis configuration including:
- Network creation timestamp
- Initial account states
- Genesis validators configuration
- Network parameters

### Validator Directories

Each validator directory contains:

- **authority-keypair.pub.json**: Validator authority public key
- **network-keypair.pub.json**: Network communication public key
- **protocol-keypair.pub.json**: Protocol-level public key
- **signing-keypair.pub.json**: Transaction signing public key
- **validator-addr.txt**: Validator network address
- **validator-state-sync-addr.txt**: State synchronization endpoint address
- **[validator-name]-signature.json**: Genesis signature from this validator

## Purpose

This repository serves as the source of truth for:
- Syncing validator public keys during genesis
- Coordinating genesis block signatures
- Establishing initial network configuration

## Related Resources

- [Rialo Official Website](https://www.rialo.io)
- [Rialo Documentation](https://www.rialo.io/docs)
- [Rialo Learn Platform](https://learn.rialo.io)

## License

Please refer to the official Rialo project for licensing information.

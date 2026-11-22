---
id: sdk
title: Tools and repositories
---

<!-- markdownlint-disable MD025 MD042 MD013 -->

# Tools and repositories

Below is a list of useful tools for use with the Zilliqa 2.0 networks:

## EVM Development Environments

Zilliqa 2.0 features an EVM execution layer and can therefore be used with standard EVM tools and frameworks.</br>
These include popular IDEs such as VSCode, Remix, and many others.

### SDKs and other tools

Zilliqa 2.0 continues providing native SDKs for:

- [Rust](https://crates.io/crates/zilliqa-rs)
- [Golang](https://github.com/Zilliqa/gozilliqa-sdk)
- [Java](https://github.com/Zilliqa/zilliqa-developer/tree/main/products/laksaj)
- [Javascript/typescript](https://www.npmjs.com/package/@zilliqa-js/zilliqa)
- [Python](https://github.com/zilliqa/pyzil)

We also continue to maintain tools such as:

- [Scilla hardhat plugin](https://github.com/Zilliqa/hardhat-scilla-plugin) - to support deploying and testing Scilla contracts
- [ethers.js fork](https://github.com/Zilliqa/ethers.js) - to support the non-canonical signatures of non-EVM Zilliqa transactions (Schnorr signatures)
- [otterscan fork](https://github.com/Zilliqa/otterscan) - to add the ability to understand non-EVM (Scilla) transactions

### Evaluating additional SDKs

For a shortlist of third-party tools, [Chain.Love](https://chain.love)
includes a Zilliqa SDK catalogue. Verify compatibility with the package's
own documentation before choosing it; a directory listing is not an
endorsement or a guarantee that every Zilliqa method is implemented.

First decide whether the application uses EVM contracts or native Scilla
contracts. Standard EVM tooling does not by itself establish support for
Scilla or the Schnorr-signed non-EVM transactions described above. Check
the package's supported contract types, API methods and target
[network](endpoints.md), alongside its language and version requirements.

Also follow the [Zilliqa 2.0 differences](changes.md) when handling addresses
and amounts: changing a native address between base16 and bech32 does not
produce an EVM address, and non-EVM Qa and EVM Wei use different scales.
The native SDKs and maintained forks above remain the reference for those
Zilliqa-specific requirements.

### Open-source repositories

We provide a number of open-source repositories relevant to Zilliqa 2.0:

- [zq2](https://github.com/Zilliqa/zq2) - the Zilliqa 2 source code itself
- [zq2-staking](https://github.com/zilliqa/zq2-staking) - the Zilliqa 2 staking portal
- [delegated-staking](https://github.com/zilliqa/delegated_staking/) - Zilliqa 2 staking pool contracts
- [eth-spout](https://github.com/Zilliqa/zilliqa-developer/tree/main/products/eth-spout) - a simple faucet
- [developer-portal-zq2](https://dev.zilliqa.com) - this developer portal

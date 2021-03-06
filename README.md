[![Build Status](https://travis-ci.com/KZen-networks/multi-party-ecdsa.svg?branch=master)](https://travis-ci.com/KZen-networks/multi-party-ecdsa)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

KZen Multi-party ECDSA
=====================================

This project is a Rust implementation of {t,n}-threshold ECDSA (elliptic curve digital signature algorithm).

Threshold ECDSA includes two protocols:

* Key Generation for creating secret shares.
* Signing for using the secret shares to generate a signature. 

ECDSA is used extensively for crypto-currencies such as Bitcoin, Ethereum (secp256k1 curve), NEO (NIST P-256 curve) and much more.
This library can be used to create MultiSig and ThresholdSig crypto wallet.

Performance
-------

* _Provider:_ EC2 AWS, _bench_: self::bench_full_keygen_party_one_two.

| Feature    | Model     | vCPU | Mem (GiB) | SSD Storage (GB) | Dedicated EBS Bandwidth (Mbps) | Bench                                   |
|------------|-----------|------|-----------|------------------|--------------------------------|-----------------------------------------|
| **Keygen** | m4.xlarge | 4    | 16        | 28               | 750                            | 1,528,965,676 ns/iter (+/- 195,059,290) |

License
-------
Multi-party ECDSA is released under the terms of the GPL-3.0 license. See [LICENSE](LICENSE) for more information.

Development Process
-------------------
The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md), in addition **the [Rust utilities wiki](https://github.com/KZen-networks/rust-utils/wiki) contains information on workflow and environment set-up**.

Contact
-------------------
For any questions, feel free to [email us](mailto:github@kzencorp.com).
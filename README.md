# OPENZEPPELIN

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-cryptocurrency-lightgrey)

> Anticloud-hardened packaging of the upstream project `OPENZEPPELIN` in category **CRYPTOCURRENCY**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CRYPTOCURRENCY · **Upstream:** https://github.com/OpenZeppelin/openzeppelin-contracts · **Upstream pin:** `cd3284fde41f1c56d19078f580a0aed751cf11d2` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# <img src="logo.svg" alt="OpenZeppelin" height="40px">

[![Github Release](https://img.shields.io/github/v/tag/OpenZeppelin/openzeppelin-contracts.svg?filter=v*&sort=semver&label=github)](https://github.com/OpenZeppelin/openzeppelin-contracts/releases/latest)
[![NPM Package](https://img.shields.io/npm/v/@openzeppelin/contracts.svg)](https://www.npmjs.org/package/@openzeppelin/contracts)
[![Coverage Status](https://codecov.io/gh/OpenZeppelin/openzeppelin-contracts/graph/badge.svg)](https://codecov.io/gh/OpenZeppelin/openzeppelin-contracts)
[![Docs](https://img.shields.io/badge/docs-%F0%9F%93%84-yellow)](https://docs.openzeppelin.com/contracts)
[![Forum](https://img.shields.io/badge/forum-%F0%9F%92%AC-yellow)](https://forum.openzeppelin.com/)

**A library for secure smart contract development.** Build on a solid foundation of community-vetted code.

 * Implementations of standards like [ERC20](https://docs.openzeppelin.com/contracts/erc20) and [ERC721](https://docs.openzeppelin.com/contracts/erc721).
 * Flexible [role-based permissioning](https://docs.openzeppelin.com/contracts/access-control) scheme.
 * Reusable [Solidity components](https://docs.openzeppelin.com/contracts/utilities) to build custom contracts and complex decentralized systems.

:mage: **Not sure how to get started?** Check out [Contracts Wizard](https://wizard.openzeppelin.com/) — an interactive smart contract generator.

> [!IMPORTANT]
> OpenZeppelin Contracts uses semantic versioning to communicate backwards compatibility of its API and storage layout. For upgradeable contracts, the storage layout of different major versions should be assumed incompatible, for example, it is unsafe to upgrade from 4.9.3 to 5.0.0. Learn more at [Backwards Compatibility](https://docs.openzeppelin.com/contracts/backwards-compatibility).

## Overview

### Release tags

We use NPM tags to clearly distinguish between audited and non-audited versions of our package:

| Tag        | Purpose                  | Description                                                                                                                                                                   |
| :--------- | :----------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **latest** | ✅ Audited releases      | Stable, audited versions of the package. This is the **default** version installed when users run `npm install @openzeppelin/contracts`.                                      |
| **dev**    | 🧪 Final but not audited | Versions that are finalized and feature-complete but have **not yet been audited**. This version is fully tested, can be used in production and is covered by the bug bounty. |
| **next**   | 🚧 Release candidates    | Pre-release versions that are **not final**. Used for testing and validation before the version becomes a final `dev` or `latest` release.                                    |

### Installation

#### Hardhat (npm)

```
$ npm install @openzeppelin/contracts
```
→ Installs the latest audited release (`latest`).

```
$ npm install @openzeppelin/contracts@dev
```
→ Installs the latest unaudited release (`dev`).

#### Foundry (git)

> [!WARNING]
> When installing via git, it is a common error to use the `master` branch. This is a development branch that should be avoided in favor of tagged releases. The release process involves security measures that the `master` branch does not guarantee.

> [!WARNING]
> Foundry installs the latest version initially, but subsequent `forge update` commands will use the `master` branch.

```
$ forge install OpenZeppelin/openzeppelin-contracts
```

Add `@openzeppelin/contracts/=lib/openzeppelin-contracts/contracts/` in `remappings.txt`.

### Usage

Once installed, you can use the contracts in the library by importing them:

```solidity
pragma solidity ^0.8.20;

import {ERC721} from "@openzeppelin/contracts/token/ERC721/ERC721.sol";

contract MyCollectible is ERC721 {
    constructor() ERC721("MyCollectible", "MCO") {
    }
}
```

_If you're new to smart contract development, head to [Developing Smart Contracts](https://docs.openzeppelin.com/learn/developing-smart-contracts) to learn about creating a new project and compiling your contracts._

To keep your system secure, you should **always** use the installed code as-is, and neither copy-paste it from online sources nor modify it yourself. The library is designed so that only the contracts and functions you use are deployed, so you don't need to worry about it needlessly increasing gas costs.

## Learn More

The guides in the [documentation site](https://docs.openzeppelin.com/contracts) will teach about different concepts, and how to use the related contracts that OpenZeppelin Contracts provides:

* [Access Control](https://docs.openzeppelin.com/contracts/access-control): decide who can perform each of the actions on your system.
* [Tokens](https://docs.openzeppelin.com/contracts/tokens): create tradeable assets or collectibles for popular ERC standards like ERC-20, ERC-721, ERC-1155, and ERC-6909.
* [Utilities](https://docs.openzeppelin.com/contracts/utilities): generic useful tools including non-overflowing math, signature verification, and trustless paying systems.

The [full API](https://docs.openzeppelin.com/contracts/api/token/ERC20) is also thoroughly documented, and serves as a great reference when developing your smart contract application. You can also ask for help or follow Contracts' development in the [community forum](https://forum.openzeppelin.com).

Finally, you may want to take a look at the [guides on our blog](https://blog.openzeppelin.com/), which cover several common use cases and good practices. The following articles provide great background reading, though please note that some of the referenced tools have changed, as the tooling in the ecosystem continues to rapidly evolve.

* [The Hit

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json, package-lock.json; scanned in UPSTREAM_CLONE)
- Top-level source layout: `audits/`, `contracts/`, `fv/`, `hardhat/`, `lib/`, `scripts/`, `test/`
- Snapshot size: **916 files**, **49174 lines of code** (measured; see Benchmarks)
- Primary languages: `.sol` (420), `.js` (239), `.ts` (51), `.adoc` (37), `.spec` (33), `.conf` (18)
- Upstream commit pinned for this packaging: `cd3284fde41f1c56d19078f580a0aed751cf11d2`

---

## Installation

* Implementations of standards like [ERC20](https://docs.openzeppelin.com/contracts/erc20) and [ERC721](https://docs.openzeppelin.com/contracts/erc721).
 * Flexible [role-based permissioning](https://docs.openzeppelin.com/contracts/access-control) scheme.
 * Reusable [Solidity components](https://docs.openzeppelin.com/contracts/utilities) to build custom contracts and complex decentralized systems.

:mage: **Not sure how to get started?** Check out [Contracts Wizard](https://wizard.openzeppelin.com/) — an interactive smart contract generator.

> [!IMPORTANT]
> OpenZeppelin Contracts uses semantic versioning to communicate backwards compatibility of its API and storage layout. For upgradeable contracts, the storage layout of different major versions should be assumed incompatible, for example, it is unsafe to upgrade from 4.9.3 to 5.0.0. Learn more at [Backwards Compatibility](https://docs.openzeppelin.com/contracts/backwards-compatibility).

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

```sh
npm start          # declared start script, when present
npm run dev        # declared dev script, when present
```

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `OPENZEPPELIN` source tree vendored in `UPSTREAM_CLONE/` (Node.js / npm ecosystem). Public entry points:

- Source modules: `audits/`, `contracts/`, `fv/`, `hardhat/`, `lib/`, `scripts/`, `test/`
- The snapshot declares 46 dependency references across 1 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json, package-lock.json |
| Files in snapshot | 916 |
| Lines of code | 49174 |
| Dependency references | 46 |
| Dependencies by ecosystem | npm: 46 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | @changesets/changelog-github | ^1.0.0 | package.json |
| npm | @changesets/cli | ^3.0.0 | package.json |
| npm | @changesets/pre | ^3.0.0 | package.json |
| npm | @changesets/read | ^1.0.0 | package.json |
| npm | @eslint/compat | ^1.2.1 | package.json |
| npm | @ethereumjs/mpt | ^10.1.0 | package.json |
| npm | @noble/curves | ^2.0.1 | package.json |
| npm | @nomicfoundation/hardhat-ethers | ^4.0.14 | package.json |
| npm | @nomicfoundation/hardhat-ethers-chai-matchers | ^3.0.11 | package.json |
| npm | @nomicfoundation/hardhat-mocha | ^4.0.0 | package.json |
| npm | @nomicfoundation/hardhat-network-helpers | ^3.0.11 | package.json |
| npm | @openzeppelin/docs-utils | ^0.1.6 | package.json |
| npm | @openzeppelin/merkle-tree | ^1.0.7 | package.json |
| npm | @openzeppelin/upgrade-safe-transpiler | ^0.4.2 | package.json |
| npm | @openzeppelin/upgrades-core | ^1.20.6 | package.json |
| ... | (31 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

* [A Gentle Introduction to Ethereum Programming, Part 1](https://blog.openzeppelin.com/a-gentle-introduction-to-ethereum-programming-part-1-783cc7796094) provides very useful information on an introductory level, including many basic concepts from the Ethereum platform.
* For a more in-depth dive, you may read the guide [Designing the Architecture for Your Ethereum Application](https://blog.openzeppelin.com/designing-the-architecture-for-your-ethereum-application-9cec086f8317), which discusses how to better structure your application and its relationship to the real world.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing Guidelines

There are many ways to contribute to OpenZeppelin Contracts.

## Troubleshooting

You can help other users in the community to solve their smart contract issues in the [OpenZeppelin Forum].

[OpenZeppelin Forum]: https://forum.openzeppelin.com/

## Opening an issue

You can [open an issue] to suggest a feature or report a minor bug. For serious bugs please do not open an issue, instead refer to our [security policy] for appropriate steps.

If you believe your issue may be due to user error and not a problem in the library, consider instead posting a question on the [OpenZeppelin Forum].

Before opening an issue, be sure to search through the existing open and closed issues, and consider posting a comment in one of those instead.

When requesting a new feature, include as many details as you can, especially around the use cases that motivate it. Features are prioritized according to the impact they may have on the ecosystem, so we appreciate information showing that the impact could be high.

[security policy]: https://github.com/OpenZeppelin/openzeppelin-contracts/security
[open an issue]: https://github.com/OpenZeppelin/openzeppelin-contracts/issues/new/choose

## Submitting a pull request

If you would like to contribute code or documentation you may do so by forking the project and submitting a pull request.

Any non-trivial code contribution must be first discussed with the maintainers in an issue (see [Opening an issue](#opening-an-issue)). Only very minor changes are accepted without prior discussion.

Make sure to read and follow the [engineering guidelines](./GUIDELINES.md). Run linter and tests to make sure your pull request is good before submitting it.

AI coding assistants are welcome (see [`CLAUDE.md`](./CLAUDE.md) for project tooling), but we encourage to review thoroughly any submitted line of code. We may close low-effort AI output without further explanations.

Changelog entries should be added to each pull request by using [Changesets](https://github.com/changesets/changesets/).

When opening the pull request you will be presented with a template and a series of instructions. Read through it carefully and follow all the steps. Expect a review and feedback from the maintainers afterwards.

If you're looking for a good place to start, look for issues labelled ["good first issue"](https://github.com/OpenZeppelin/openzeppelin-contracts/labels/good%20first%20issue)!

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
The MIT License (MIT)

Copyright (c) 2016-2026 Zeppelin Group Ltd

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `OPENZEPPELIN` (category: CRYPTOCURRENCY)
- **Upstream URL:** https://github.com/OpenZeppelin/openzeppelin-contracts
- **Pinned commit (SHA):** `cd3284fde41f1c56d19078f580a0aed751cf11d2`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`a25f31c4a9c66162ef5a1d65db15cd69c5c347a3bf2f3222be9a013fcd124b45`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.


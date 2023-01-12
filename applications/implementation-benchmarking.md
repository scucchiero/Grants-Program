# Implementation Bechmarking

- **Team Name:** Rather Labs, Inc
- **Payment Address:** Ethereumm - USDC/USDT/DAI - 0xc01fdBdDc9FFE3AA1Efccf4FD3001535130041a5
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 2

## Project Overview :page_facing_up:
https://w3f.github.io/Grants-Program/RFPs/Open/implementation-benchmarking

### Overview
We are interested in applying for creating this implementation benchmarking tool to help developers make informed decisions when choosing the best tool for writing application logic. We 

## Team :busts_in_silhouette:

### Team members

- Franco Scucchiero
- Federico Caccia
- Pablo Altamura
- Marcos Tacca

### Contact

- **Contact Name:** Franco Scucchiero
- **Contact Email:** franco@ratherlabs.com
- **Website:** https://ratherlabs.com

### Legal Structure

- **Registered Address:** 2810 North Church Street, PMB 15600, Wilmington, DE 19802
- **Registered Legal Entity:** Rather Labs, Inc

### Team's experience
Rather Labs is a blockchain software development company. From day 1, Rather Labs pioneered new ecosystems, developing key infrastructure in multiple blockchains.

**Some examples**

- Partner with Hatom to develop [the first Lending protocol](https://beta.hatom.com/) in the Elrond blockchain
- Partner with Nervos Foundation to develop [an NFT implementation standard.](https://ratherlabs.com/work/nrc-721)

### Team Code Repos

- https://github.com/rather-labs

Team github

- https://github.com/scucchiero
- https://github.com/fedecaccia
- https://github.com/paltamura
- https://github.com/mstacca

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/scucchiero
- https://www.linkedin.com/in/fedecaccia/
- https://www.linkedin.com/in/pablo1664/
- https://www.linkedin.com/in/marcos-sebastian-tacca/?originalSubdomain=ar


## Development Status :open_book:
So far we are in the stage of evaluation, research & PoCs.

## Development Roadmap :nut_and_bolt:

### Overview

- **Total Estimated Duration:** 7 weeks
- **Full-Time Equivalent (FTE):**  1
- **Total Costs:** 14,000 USD

### Milestone 1 - Definitions

- **Estimated duration:** 1 week
- **FTE:** 1
- **Budget:** 2000 USD
- **Main goal:** Ensure alignment with the RFP
    

| Number | Deliverable | Specification |
| --- | --- | --- |
| 1a. | List of calls | Define set of calls. |
| 1b. | List of measurable metrics | Define basic and advanced metrics. |
| 1c. | Definition of measurement methodology for the basic metrics (doc) | Study in a general way how we are going to access or build the values of each (BASIC) metric (Execution time / storage footprint). |
| 1d. | Measurement toolkit/library (code) | Code a small library that makes the calls (scenario agnostic), obtains the metrics, calculates the estimators, lists them, and exports them as a file  (Checking if we can reuse some of what exists). |

### Milestone 2 - Rust-based Measurements

- **Estimated duration:** 2 week
- **FTE:** 1
- **Budget:** 4000 USD
- **Main goal:** Develop benchmarking stage for Pallet and Ink!.

| Number | Deliverable | Specification |
| --- | --- | --- |
| 2a. | Pallet benchmarking stage -  Design and PoC. (code) | Obtain a conceptual view of the scenario. Set up a first local development environment, and run a mini PoC that includes a custom pallet with a public fn with 2 arguments and return. Call to that function from a subxt based rust client. Study in a specific way how we are going to access or build the values of each (BASIC) metric, and generate a library for the scenario. The retrieval of some metrics may differ between scenarios. |
| 2b. | Pallet benchmarking stage - Specific measurement script. Pallet and client full version. (code) | Code full set of calls into the pallet and the specific client. Code specific measurement script. |
| 2c. | Ink! benchmarking stage -  Design and PoC. (code) | - Similar to 2a. |
| 2d. | Ink! benchmarking stage - Specific measurement script. SC and client full version. (code) | - Similar to 2b. |

### Milestone 3 – Solidity-based Measurements

- **Estimated duration:** 3 weeks
- **FTE:** 1
- **Budget:** 6000 USD
- **Main goal:** Develop benchmarking stage for “native” Solidity and Solidity compiled to WASM.

| Number | Deliverable | Specification |
| --- | --- | --- |
| 3a. | Native Solidity benchmarking stage - Design and PoC. (code) | Obtain a conceptual view of the scenario. Set up a first local development environment, and run a mini PoC that includes a custom smart contract with a public fn with 2 arguments and return. Call to that function from a subxt based rust client. Study in a specific way how we are going to access or build the values of each (BASIC) metric, and generate a library for the scenario. The retrieval of some metrics may differ between scenarios. |
| 3b. | Native Solidity benchmarking stage - Specific measurement script. Pallet and client full version. (code) | Code full set of calls into the smart contract and the specific client. Code specific measurement script. |
| 3c. | WASM-compiled Solidity stage design | - Similar to 3a. |
| 3d. | WASM-compiled Solidity stage implementation | - Similar to 3b. |

### Milestone 4 – Dockerization and reporting

- **Estimated duration:** 1 weeks
- **FTE:** 1
- **Budget:** 2000 USD
- **Main goal:** Package benchmarking scripts in docker and create advance reporting

| Number | Deliverable | Specification |
| --- | --- | --- |
| 4a. | Reporting script (code) | Results integrator script to express them as a benchmark, with the scenarios in columns and the calls in rows. It could print them in console and export a file. |
| 4b. | Dockerization | Configure the system, run the analysis and  execute the integrator script for each context. |
| 4c. | Stack overflow article (text proposal) | A study of the solution, how it works, how it differs from others, and most important how to use it. |

### Milestone 5 – Advance Metrics

- **Estimated duration: TBD**
- **FTE:** 1
- **Budget:** TBD
- **Main goal:** Take advantage of the efficiency and knowledge gained during the early stages of the project to define value and cost-effective tasks.
...


## Future Plans

Please include here

- We are willing to apply to an RFP to maintain this work, updating it on API changes and continuing adding measured parameters and use cases.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** personal recommendation

# Logos Chain Development Environment

**The Logos Project is an initiative dedicated to transforming the provision and management of physical infrastructure for Web3. It moves beyond centralized data centers and cloud services of Web2, aiming to establish a trustless, resilient, and sustainable foundation for a truly decentralized Internet.**

This repository serves as the dedicated development environment for the **Logos Chain**.

Given the extensive research and development activities within the Logos project, we have established this separate environment to focus exclusively on development. No production implementations are hosted here.

The Logos Chain is the primary control component of the Logos Network, responsible for managing all state changes across the entire network. It operates as a trustless public network and is exclusively designed for the provision and operation of the Logos Network. The chain is built with the principles of Zero Trust, Zero Knowledge, and Zero Tolerance to ensure maximum security and reliability.

**Technology Basis**   
The Logos Chain is currently being developed using the Substrate Framework for two key reasons: forkless updates and modularity.

- Forkless Updates
No system is perfect and regular updates are inevitable. The ability to implement updates without requiring forks simplifies maintenance and improves efficiency.

- Modularity
Modularity allows for the development and deployment of new functionalities with ease, ensuring adaptability to evolving requirements.

> [!NOTE]  
> This is a development environment where many features and concepts are tested and developed. These may not necessarily be implemented in their current form in the production-ready Logos Chain. 

## Project structure
> [!NOTE]  
> Since the project is in the early stages, the structure of the project may change or may be extended.

The project structure currently consists of 3 main "segments"

- Chain (/node; /runtime; /pallet; cargo workspace):  
In this section, the blockchain (blockchain logic (runtime) and the infrastructure (client)) is configured, as the cargo workspace and the dependencies.

- Contracts (/contracts):  
As the implementation of the Logos network will mainly be carried out by smart contracts, the development in the smart contract field plays an important role for the project.

- General (.gitignore, rust-toolchain.toml, rustfmt.toml, docker, etc.):
For a clean code and project some general configurations are necessary.

> [!NOTE]  
> The code in this repository is extensively commented to make it easier and faster for beginners to understand and follow.

## Dependency structure
The dependencies are all defined and versioned in the main cargo manifest (/Cargo.toml) and are then implemented where required.
The approach behind this is to make versioning clearer and to enable easier dependency management.

## Nightly vs Stable
In the Rust programming language, there are various "release channels" (stable, nightly, ...) that determine how often and in what form new versions and updates are made available.

The **Stable** channel is Rust's main release line. Versions in the stable channel are released every six weeks and have undergone strict quality control.

The **Nightly** channel, on the other hand, is a pre-release version of Rust which, as the name suggests, is updated daily. Nightly builds contain the very latest features and changes that are not yet available in the stable channel.

Stable is usually the best choice for production-ready applications, while Nightly is a good option for research, development of new Rust features or for projects that rely on the very latest language features.

We choose the stable channel because we do not rely on the latest Rust features, and we prefer to ensure sufficient stability before implementing updates.

> [!NOTE]  
> Clear and detailed information about the individual components of the Logos Chain will be provided in the technical specifications. Once finalized, this information will be included here

## Support and Contribution
The project is community-driven and FOSS-oriented, welcoming everyone to contribute and help us build a Web3-native physical infrastructure for the Internet. If you have any questions or want to contribute, feel free to reach out! You can email us at ***tech.support@logoslabs.io***, open a [GitHub issue](https://github.com/logoslabstech/logos-project-resources/issues/new/choose), or ***ask anything*** on [Discord](https://discord.com/channels/840352211602374657/1242178591744200804).

## Ressources
- [Logos Project website](https://logoslabs.io)
- [Logos Project documentation](https://docs.logoslabs.io)
- [Logos Project blog](https://blog.logoslabs.io/)

### **We look forward to your contributions and insights as we work together to shape the future of the Internet!**
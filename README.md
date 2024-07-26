# Sociopi

## Vision
To create a robust decentralized identity and single sign-on (SSO) solution leveraging Chainlink Oracles on the Avalanche blockchain, while integrating SwapKit to simplify cross-chain blockchain interactions.

## Project Overview
Sociopi integrates Chainlink Oracles on the Avalanche blockchain to offer a secure decentralized identity and SSO solution. Utilizing the Chainflip SDK and SwapKit components, Sociopi provides seamless multi-chain functionality and enhanced user experiences.

## Key Features
1. **Decentralized Identity and SSO**
   - Uses Chainlink Oracles to ensure secure and reliable data feeds.
   - Implements a decentralized identity solution on Avalanche for secure SSO.

2. **Multi-Chain Integration**
   - Leverages SwapKit to enable seamless cross-chain operations.
   - Supports a variety of blockchain networks and tokens.

3. **Enhanced Security**
   - High-security standards using Chainlink Oracles.
   - Secure and efficient single sign-on experience.

## Technical Stack
- **Frontend**: React.js, Next.js
- **Backend**: Node.js, Express.js
- **Blockchain Integration**: Chainlink Oracles, SwapKit SDK, Avalanche
- **Database**: MongoDB, Redis
- **Deployment**: Docker, Kubernetes, AWS/GCP

## SwapKit Integration
Sociopi integrates the following SwapKit components to enable multi-chain capabilities and enhance blockchain interactions:

- **@swapkit/helpers@1.0.0-rc.103**
- **@swapkit/toolbox-evm@1.0.0-rc.109**
- **@swapkit/api@1.0.0-rc.71**
- **@swapkit/toolbox-substrate@1.0.0-rc.38**

### Usage
In the `ThorSwapComponent.js` file, the SwapKit SDK is used as follows:

```javascript
import React, { useState, useEffect } from 'react';
import { Chain, createSwapKit, WalletOption } from '@swapkit/sdk';

// Additional component code here
```

## Documentation
Comprehensive documentation is available for setting up and using SwapKit and integrating with various blockchains.

## Getting Started
Follow these instructions to set up the development environment and start contributing to Sociopi.

## Packages
This repository contains packages related to the SwapKit SDK and its integrations with different blockchains.

### Wallets
Integration with various cryptocurrency wallets for secure transactions.

### Toolboxes
Development toolboxes to aid in building and integrating blockchain functionalities.

## Contributing
### Pre-requisites
```sh
curl -fsSL https://bun.sh/install | bash
```
Copy `.env.example` to `.env` and fill it with data.

### Installation
```sh
bun bootstrap
```

### Branches
- **main** - Production branch.
- **develop** - Development branch - all PRs should be merged here first.
- **nightly** - Branch for nightly builds - can be used for testing purposes.

### Testing
To run tests, use the following command:
```sh
bun test
```

### Pull Requests
- PRs should be created from the `develop` branch.
- PRs should be reviewed by at least one Code Owner (see `CODEOWNERS` file).
- PRs should include a scope in the commit message (see commit messages section).
- PRs should include tests if possible.
- PRs should include a changeset file if needed (see release section).

### New Package
To create a new package, use the following command and pick one of the options:
```sh
bun generate
```
This command sets up the package with necessary files for bundling and publishing.

### Release and Publish
Packages are automatically published to npm when a new PR is merged to the `main` & `develop` branches. To automate and handle the process, we use changesets and GitHub action workflows.

Before running `bun changeset`, pull the `main` & `develop` branches.

To release a new version of a package, create a PR with the changes and add a changeset file to your commit:
```sh
bun changeset
```

After the PR is merged to the `develop` branch with the changeset file, a GitHub action will create a new PR with updated versions of packages and changelogs.

## Conclusion
Sociopi combines Chainlink Oracles, the Avalanche blockchain, and SwapKit components to deliver a powerful decentralized identity and SSO solution. By integrating multi-chain capabilities and focusing on security, Sociopi aims to enhance the decentralized finance ecosystem.

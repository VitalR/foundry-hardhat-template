# <h1 align="center"> Foundry x Hardhat Template </h1>

**Template repository for getting started quickly with Foundry and Hardhat in one project**

![Github Actions](https://github.com/devanonon/hardhat-foundry-template/workflows/test/badge.svg)

### Getting Started

 * Use Foundry: 
```bash
forge install
forge test
```

 * Use Hardhat:
```bash
npm install  ||  yarn
npx hardhat test
```

### Features

 * Write / run tests with either Hardhat or Foundry:
```bash
forge test  ||  yarn test
# or
npx hardhat test  ||  yarn testhh
```

 * Install libraries with Foundry which work with Hardhat.
```bash
forge install rari-capital/solmate # Already in this repo, just an example
```

### Notes

Whenever you install new libraries using Foundry, make sure to update your `remappings.txt` file by running `forge remappings > remappings.txt`. This is required because we use `hardhat-preprocessor` and the `remappings.txt` file to allow Hardhat to resolve libraries you install with Foundry.
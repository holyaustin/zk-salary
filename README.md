# zk-Salary DApp for Partisia Blockchain

This a development environment for the Partisia Blockchain, made for creating applications and smart contracts utilizing the Zk Rust and public blockchain.

## It is an Automated setup

To interact with the Partisia Blockchain you need an account with gas.
The codespace automatically provides you with three new accounts,
`Account-A.pk`, `Account-B.pk` and `Account-C.pk`.

The created accounts have test_coins pre-minted which gives you 100.000.000 gas on the Testnet to
interact, deploy and
play around with as part of the codespace. You can continue using these outside of the codespace,
just remember the private keys, because they are not saved when you delete the codespace.

Read how addresses works
for [accounts and smart contracts](https://partisiablockchain.gitlab.io/documentation/pbc-fundamentals/dictionary.html#address).

## It is your own online personalized DApp playground

To use the codespace to develop your own DApps, fork the repository.
On the fork you can modify the contract- and client code, to make your own DApp.
To save your changes, use git to commit those changes to your forked repository.

Read about using codespaces in a forked
repository [here](https://www.freecodecamp.org/news/how-to-make-your-first-open-source-contribution/).

When forking the repository you can drastically decrease boot up time for new dev containers
by [configuring prebuilds](https://docs.github.com/en/codespaces/prebuilding-your-codespaces/configuring-prebuilds).

If you want to do local development read
the [dev container documentation](https://docs.github.com/en/codespaces/developing-in-a-codespace/using-github-codespaces-in-visual-studio-code).

## Try, Learn and Interact with Partisia Blockchain

We have included 2 challenge-based tutorials as part of your codespace, to help you learn and
experiment.

The first one explores the [Petition example application](tutorial/petition-example-application.md),
showing how to collect signatures for showing interests in making specific changes in the world. The
application consists of a smart contract written in Rust and a web frontend written in TypeScript.

The second one explores
the [Average Salary example application](tutorial/average-salary-example-application.md), showing
how
to compute the average salary of a group, without revealing the salary of any individual. This
example
uses the superpower of Partisia
Blockchain,
[Zk contracts](https://partisiablockchain.gitlab.io/documentation/smart-contracts/zk-smart-contracts/zk-smart-contracts.html).

## Simple Average Salary contract
Average salary is a common multi-party computation example, where several privacy-concious individuals are interested in determining whether they are getting a fair salary, without revealing the salary of any given individual.
This implementation works in following steps:

Initialization on the blockchain.

Receival of multiple secret salaries, using the real zk protocol.

Once enough salaries have been received, the contract owner can start the ZK computation.

The Zk computation sums all the given salaries together.
Once the zk computation is complete, the contract will publicize the the summed variable.

Once the summed variable is public, the contract will compute the average and store it in the state, such that the value can be read by all.


The application consists of a smart contract written in Rust
and [Zk Rust](https://partisiablockchain.gitlab.io/documentation/smart-contracts/zk-smart-contracts/zk-rust-language-zkrust.html)
and a web frontend written in TypeScript.

If you want to know more about the blockchain, ZK Rust or just contracts in general,
we urge you to visit our [documentation](https://partisiablockchain.gitlab.io/documentation/) and
participate
in [our active community on Discord](https://partisiablockchain.gitlab.io/documentation/get-support-from-pbc-community.html).

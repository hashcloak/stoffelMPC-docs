# Smart Contracts

In order to for the MPC sidechain to retrieve public user inputs and coordinate the computation, they need to interact with a set of smart contracts.
These smart contracts are meant to be integrated directly into the blockchain environment that you will be using. At the time of this writing, we only support Solidity.

## Collecting Public User Inputs
When a Stoffel lang program is compiled, the compiler will provide a set of smart contracts that developers can use as libraries within their contracts.
For functionality that requires getting public inputs from users, the smart contract collecting these inputs will have functions that users will call. These functions will emit events in order to facilitate the collection of public inputs for the MPC nodes.

```
contract MPCInputs {
    TODO
}
```

## Coordinating MPC nodes
In order for the MPC nodes to know when to do the computation, and what public inputs the computation needs, they coordinate through the use of a smart contract.
This smart contract also contains information about the identities of the MPC nodes in addition to basic parameters that are dependent on the MPC protocol in use.

```
contract MPCCoordination {
    TODO
}
```
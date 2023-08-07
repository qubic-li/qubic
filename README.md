# qubic - node
Qubic Node Source Code - this repository contains the source code of a full qubic node.

## How to run a Listening Node
To run a "listen-only" node, just add 3-4 known pulic peers to the code.
```c++
static const unsigned char knownPublicPeers[][4] = {
};
```
Compile with RELEASE.

## How to run a Computor Node
1. Add your Computor Seed(s)
```c++
static unsigned char computorSeeds[][55 + 1] = {
    "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
};
```
2. Add your Operator Identity
The Operator Identity is used to identify the Operator. The Operator can send Commands to your Node.
```c++
#define OPERATOR "AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"
```
3. Add 3-4 Known Public Peers (can be obtained from https://app.qubic.li/network/live)
```c++
static const unsigned char knownPublicPeers[][4] = {
  {12,13,14,12}
};
```

## License
The Anti-Military License. See https://github.com/computor-tools/qubic-js

## Installation and Configuration
Please refer to https://docs.qubic.world

## Limited Support
We cannot support you in any case. You are welcome to provide updates, bugfixes or other code changes by pull requests.

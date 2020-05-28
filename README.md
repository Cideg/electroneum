
# Tesoro

Copyright (c) 2014-2019 The Monero Project.

Copyright (c) 2019-2020 TesoroDev.

Portions Copyright (c) 2012-2013 The Cryptonote developers.



### Tesoro (TSX)

Tesoro (TSX) is a decentralized cryptocurrency based on PoW consensus that uses RandomX
algorithm which favours CPU powered PCs over GPUs allowing average users to be a part of the
creation and maintenance of its blockchain and network and also using modified Monero source
code in Tesoro grants compatibility along with high security and privacy features.

TesoroDev was initiated as a group of independent of developers spread out through many
different countries to develop the Tesoro (TSX) cryptocurrency.

### Purpose and Use-case of Tesoro (TSX)

Blockfinex is a cryptocurrency trading and exchange platform built upon a lightning fast execution
engine. For the ease of its users to use trading fee discounts, community rewards, community
incentives, online payments etc. a new currency was proposed to be used within the exchange as
well as to be utilized as a measure of online payments outside the exchange.

Unlike a token issued using smart contracts where a handful of people take control of the supply,
developers behind Blockfinex exchange decided to develop Tesoro (TSX) as a new
cryptocurrency since its integral properties help users themselves participate in nurturing the
blockchain thus bringing decentralization and fair distribution of supply to its network.

### Technical Features of Tesoro (TSX)

```
• Block Size – Dynamic
• Block Time – 60 Seconds
• Coin Supply - 14,716,800 (No Pre-mine)
• Mining Algorithm – RandomX
• Block Reward – 4 Coins per Block
• Block Reward Halving – Every 4 Years or 2,102,400 Blocks
• Other Features – Anonymous Transactions, ASIC Resistant
```
### Coin Emission and Distribution

```
Emission Plan | Emission (TSX) | Total Supply (TSX)
4 TSX/ Block until Blockheight 2,102,400 | 8,409,600 | 8,409,600
2 TSX/ Block until Blockheight 4,204,800 | 4,204,800 | 12,614,400
1 TSX/ Block until Blockheight 6,307,200 | 2,102,400 | 14,716,800
0.5 TSX/ Block from Blockheight 6,307,201 onwards adding 262,800 TSX/ year to Total Supply
```

### Compiling Tesoro from source

[1] On Debian/Ubuntu libgtest-dev only includes sources and headers. You must build the library binary manually. This can be done with the following command sudo apt-get install libgtest-dev && cd /usr/src/gtest && sudo cmake . && sudo make && sudo mv libg* /usr/lib/ [2] libnorm-dev is needed if your zmq library was built with libnorm, and not needed otherwise

Install all dependencies at once on Debian/Ubuntu:

sudo apt update && sudo apt install build-essential cmake pkg-config libboost-all-dev libssl-dev libzmq3-dev libunbound-dev libsodium-dev libunwind8-dev liblzma-dev libreadline6-dev libldns-dev libexpat1-dev doxygen graphviz libpgm-dev qttools5-dev-tools libhidapi-dev libusb-dev libprotobuf-dev protobuf-compiler

Install all dependencies at once on macOS with the provided Brewfile: brew update && brew bundle --file=contrib/brew/Brewfile

FreeBSD one liner for required to build dependencies pkg install git gmake cmake pkgconf boost-libs libzmq libsodium

Cloning the repository
Clone recursively to pull-in needed submodule(s):

$ git clone --recursive https://github.com/Tesoro-Dev/tesoro.git

If you already have a repo cloned, initialize and update:

$ cd tesoro && git submodule init && git submodule update

Build instructions
tesoro uses the CMake build system and a top-level Makefile that invokes cmake commands as needed.

On Linux and macOS
Install the dependencies

Change to the root of the source code directory, change to the most recent release branch, and build:

cd tesoro
make


#### CLI RPC Commands
[**Wallet**](https://web.getmonero.org/resources/developer-guides/wallet-rpc.html) | 
[**Daemon**](https://web.getmonero.org/resources/developer-guides/daemon-rpc.html)

References:

https://github.com/tevador/RandomX

https://github.com/monero-project/research-lab/blob/master/whitepaper/whitepaper.pdf

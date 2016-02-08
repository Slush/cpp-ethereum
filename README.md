## Ethereum C++ Client.

[![Join the chat at https://gitter.im/ethereum/cpp-ethereum](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ethereum/cpp-ethereum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

By Gav Wood et al*, 2013, 2014, 2015.

          | Status
----------|-----------
develop   | [![Build Status](http://52.28.164.97/buildStatus/icon?job=ethbinaries-develop)](http://52.28.164.97/job/ethbinaries-develop/)
release   | [![Build Status](http://52.28.164.97/buildStatus/icon?job=ethbinaries-release)](http://52.28.164.97/job/ethbinaries-release/)

Ethereum is based on a design in an original whitepaper by Vitalik Buterin. This implementation is based on the formal specification of a refinement of that idea detailed in the 'yellow paper' by Gavin Wood. Contributors, builders and testers include:

- *arkpar* (**Arkadiy Paronyan**) Mix, PV61/BlockQueue
- *debris* (**Marek Kotewicz**) JSONRPC, web3.js
- *CJentzsch* (**Christoph Jentzsch**) tests, lots of tests
- *LefterisJP* (**Lefteris Karapetsas**) Solidity, libethash
- *chriseth* (**Christian Reitwiessner**) Solidity
- *subtly* (**Alex Leverington**) libp2p, rlpx
- *yann300* (**Yann Levreau**) Mix
- *LianaHus* (**Liana Husikyan**) Solidity
- *chfast* (**Paweł Bylica**) EVMJIT
- *cubedro* (**Marian Oancea**) web3.js
- *gluk256* (**Vlad Gluhovsky**) Whisper
- *programmerTim* (**Tim Hughes**) libethash-cl

And let's not forget: Caktux (neth, ongoing CI), Eric Lombrozo (original MinGW32 cross-compilation), Marko Simovic (original CI).

### Building

See the [Wiki](https://github.com/ethereum/webthree-umbrella/wiki) for build instructions, compatibility information and build tips. 

### Testing

To run the tests, make sure you clone github.com/ethereum/tests and point the environment variable
`ETHEREUM_TEST_PATH` to that path.

### Contributing

External contributions are more than welcome! We try to keep a list of tasks that are suitable for
newcomers under the tag [good first task](https://github.com/ethereum/webthree-umbrella/labels/good%20first%20task).
If you have any questions, please ask in our [gitter channel](https://gitter.im/ethereum/cpp-ethereum).

Please refer to the file [CONTRIBUTING.md] for some guidelines.

All new contributions are added under the MIT License. Please refer to the `LICENSE` file in the root directory.
To state that you accept this fact for all of your contributions please add yourself to the list of external contributors like in the example below.

### License

All new contributions are under the [MIT license](http://opensource.org/licenses/MIT).
See [LICENSE](LICENSE). Some old contributions are under the [GPLv3 license](http://www.gnu.org/licenses/gpl-3.0.en.html). See [GPLV3_LICENSE](GPLV3_LICENSE).

#### External Contributors

I hereby place all my contributions in this codebase under an MIT
licence, as specified [here](http://opensource.org/licenses/MIT).
- *Name Surname* (**email@domain**)

Please add yourself in the `@author` doxygen  section of the file your are adding/editing
with the same wording as the one you listed yourself in the external contributors section above,
only replacing the word **contribution** by **file**

All development goes in develop branch - please don't submit pull requests to master.

Please read [CodingStandards.txt](CodingStandards.txt) thoroughly before making alterations to the code base. Please do *NOT* use an editor that automatically reformats whitespace away from astylerc or the formatting guidelines as described in [CodingStandards.txt](CodingStandards.txt).

libweb3jsonrpc/abstractwebthreestubserver.h is autogenerated from the jsonrpcstub executable that comes with the libjsonrpc library (json-rpc-cpp project). It shouldn't be maually altered.

```bash
jsonrpcstub spec.json --cpp-server=AbstractWebThreeStubServer
```

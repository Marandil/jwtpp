# jwtpp-json
JSON Object Signing and Encryption library for C++

This fork of [jwtpp](https://github.com/troian/jwtpp) substitutes [jsoncpp](https://github.com/open-source-parsers/jsoncpp) for [JSON for Modern C++](https://github.com/nlohmann/json). Thanks to minimal differences on the APIs used by jwtpp, the changes to the core are minimal.

<!--
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/da9665fd01ba4c759cef755d1ff03d2c)](https://www.codacy.com/app/troian/jwtpp?utm_source=github.com&utm_medium=referral&utm_content=troian/jwtpp&utm_campaign=badger)
[![Build Status](https://travis-ci.com/troian/jwtpp.svg?branch=master)](https://travis-ci.com/troian/jwtpp)
[![Codecov](https://codecov.io/gh/troian/jwtpp/branch/master/graph/badge.svg)](https://codecov.io/gh/troian/jwtpp)
<a href="https://jwt.io"> <img src="https://jwt.io/img/badge-compatible.svg?sanitize=true" width="80"/></a>
-->

#### Dependencies:
  - [JSON for Modern C++](https://github.com/nlohmann/json)
  - OpenSSL

#### Built and tested with:
  - GCC
    - C++11
    - С++14
    - С++17
  - СLang
    - C++11
    - С++14
    - С++17

#### Supported features:
  - Sign
  - Verify

#### Supported algorithms
|Alg|Status|
|:---:|:------:|
| HS256 | **Supported** |
| HS384 | **Supported** |
| HS512 | **Supported** |
| RS256 | **Supported** |
| RS384 | **Supported** |
| RS512 | **Supported** |
| ES256 | **Supported** |
| ES384 | **Supported** |
| ES512 | **Supported** |
| PS256 | **Supported** |
| PS384 | **Supported** |
| PS512 | **Supported** |
| EdDSA | **Supported** |

#### Claims
|Claim|Options|Status|
|:---:|:---:|:----:|
|**_ess_**|set,verify| **Supported** 
|**_sub_**|set,verify| **Supported** 
|**_aud_**|set,verify| **Supported** 
|**_exp_**|set,verify| **Supported** 
|**_nbf_**|set,verify| **Supported** 
|**_iat_**|set,verify| **Supported** 
|**_jti_**|set,verify| **Supported** 

### How to use
Refer to tests dir

### How to build/install
#### CMake sources deps
add_subdirectory(<path to>)
#### System-wide installation
On MacOS OPENSSL_ROOT_DIR might need to be specified. Add `-DOPENSSL_ROOT_DIR=$(brew --prefix openssl)` to cmake stage

```bash
git clone https://github.com/troian/jwtpp
mkdir build && cd build
cmake -Wno-dev -DCMAKE_INSTALL_PREFIX=<install prefix> ..
make install
```
#### Homebrew
```
brew tap troian/tap
brew install jwtpp
```

### TODO
- Documentation
- Examples
- Tests

## How to contribute
Just do it! :)

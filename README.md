## TrustNote

TrustNote is an open source project that provides reliable and trusted public blockchain network services. The wallet created for the community is also named TrustNote. This project is supported by the TrustNote Foundation.

TrustNote wallet is safe, simple and easy to use, it supports transfer TRC20 Tokens, send private instant messaging, provide security solutions, etc.

We welcome everyone joins this open source community to build decentralized applications running on a fast, scalable, and truly decentralized blockchain powered by TrustNote.

Please visit TrustNote official site [trustnote.org](https://trustnote.org/) to get more information.

## Download

Official Site:
- [trustnote.org](https://trustnote.org/application.html)

Github release:
- [github.com](https://github.com/trustnote/trustnote-wallet/releases)


## Installation

We provide executable programs for multiple platforms. You can either start using the TrustNote wallet by clicking the download link above, or you can use the source code to compile into an executable program.

#### Dependences

**Choose the install package according to your operation system**

- git
- [Node.js v8.9.4](https://nodejs.org/dist/v8.9.4/)
- [NW.js v0.26.6](https://dl.nwjs.io/v0.26.6)
- bower
    - `npm install -g bower@1.8.2`
- grunt
    - `npm install -g grunt-cli`
- nw-gyp
    - `npm install -g nw-gyp`


##### Windows

**Option 1:**

- Open PowerShell by using administrator privileges, run `npm install --global --production windows-build-tools`
- Set environment variable `GYP_MSVS_VERSION = 2017`
- `npm config set msvs_version 2017`

Please refer to [windows-build-tools](https://github.com/felixrieseberg/windows-build-tools)


**Option 2:**

- Install [Visual Studio 2017](https://visualstudio.microsoft.com/zh-hans/thank-you-downloading-visual-studio/?sku=Community&rel=15)，with VC++ 2015 (v140) tools.
- Install [Python 2.7.14](https://www.python.org/downloads/release/python-2714/)
- Set environment variable, add the Python insall directory to `PATH`.
- Set environment variable `GYP_MSVS_VERSION = 2017`
- `npm config set msvs_version 2017`


#### Clone project code

```sh
git clone https://github.com/trustnote/trustnote-wallet.git
cd trustnote-wallet
```

#### Compile

```sh
# ./trustnote-wallet

bower install
npm install
npm rebuild sqlite3 --build-from-source --runtime=node-webkit --target_arch=x64 --target=0.26.6
grunt
```

#### Execute

```sh
# ./trustnote-wallet
./nwjs/nwjs .
```

#### Package

The release package will be generated under ../trustnotebuilds

```
--|
  | trustnote-wallet
  | trustnotebuilds
```

##### Android

- Install Android SDK （refer to https://developer.android.google.cn/studio/）
- Run `make android`

##### iOS

- Install Xcode 9 (or higher version)
- Install Cordova `npm install -g cordova`
- Install ios-deploy `npm install -g ios-deploy`
- Run `make ios`


##### macOS

- `make osx64`

##### Windows

- `make win64`

##### Linux

- `make linux64`


## Wallet Backup and Restore

Once the user starts to use TrustNote Wallet, cache files will be generated in the user directory to store data and user profiles, and to prevent personal data loss due to incorrect uninstallation, these caches files won’t be deleted after installation, all data will be recovered after reinstalling the software. If the user decides to delete these data, please follow the instructions below:

* macOS: `~/Library/Application Support/TTT`
* Linux: `~/.config/TTT`
* Windows: `%LOCALAPPDATA%\TTT`


## Issues and Questions

* [GitHub Issues](https://github.com/trustnote/trustnote-wallet/issues)
* [Email Support](mailto:foundation@trustnote.org)

## Translation

- **Turkish** - Caner Sevince, Sait Dogan Etiler，
- **Indonesian** - IYOES

big thanks !

## License

MIT


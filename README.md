# Android build tools installer

[![AppVeyor build status](https://img.shields.io/appveyor/ci/mortend/android-build-tools/master.svg?logo=appveyor&logoColor=silver&style=flat-square)](https://ci.appveyor.com/project/mortend/android-build-tools/branch/master)
[![Travis CI build status](https://img.shields.io/travis/mortend/android-build-tools/master.svg?style=flat-square)](https://travis-ci.org/mortend/android-build-tools)
[![NPM package](https://img.shields.io/npm/v/android-build-tools.svg?style=flat-square)](https://www.npmjs.com/package/android-build-tools)
[![License: MIT](https://img.shields.io/github/license/mortend/android-build-tools.svg?style=flat-square)](LICENSE)
![Supported platforms](https://img.shields.io/badge/os-Linux%20%7C%20macOS%20%7C%20Windows-7F5AB6?style=flat-square)

Android SDK and NDK installer for Uno and Fuse apps.

> Possibly useful in other scenarios where Android SDK and NDK are needed as well.

> Visit [Fuse Open](https://fuseopen.com/) for more information about Uno and Fuse.

## Install

```
$ npm install android-build-tools -g
```

> This package is suitable for Linux, macOS and Windows (64-bit).

The SDK is installed to one of the locations below. The installer will only download the SDK or additional components when something is missing.

| Host OS  | Location                      |
|:---------|:------------------------------|
| Linux    | `~/Android/Sdk`               |
| macOS    | `~/Library/Android/sdk`       |
| Windows  | `%LOCALAPPDATA%\Android\sdk`  |

### Remarks

* Please note that [JDK8](https://adoptopenjdk.net/) (not 9+) [is required](https://stackoverflow.com/questions/46402772/failed-to-install-android-sdk-java-lang-noclassdeffounderror-javax-xml-bind-a) to install Android SDK, and that `bash` is required to run the install script. `bash` is included in [Git for Windows](https://git-scm.com/downloads).

> On Windows, if your user name or `%LOCALAPPDATA%` contain non-ASCII characters, the SDK is installed to `%PROGRAMDATA%\Android\sdk` instead. This is because we get build errors if the SDK location contains non-ASCII characters.

> If you're using Fuse SDK v1.14 or lower, you should install `android-build-tools@1.4.0` because later versions aren't compatible with older Fuse SDK releases.

> If you're using Fuse SDK v1.12 or lower, you should install `android-build-tools@1.2.0` because later versions aren't compatible with older Fuse SDK releases.

### Related packages

* [fuse-sdk](https://www.npmjs.com/package/fuse-sdk)
* [uno](https://www.npmjs.com/package/@fuse-open/uno)

## Contributing

Please [report an issue](https://github.com/mortend/android-build-tools/issues) if you encounter a problem, or [open a pull request](https://github.com/mortend/android-build-tools/pulls) if you make a patch.

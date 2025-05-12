# Compatible SRP implementations

The list and umbrella issue tracker for compatible SRP implementations.

## The list


| Library | Language | Badges |
| ------ | ------ | ------ |
| [SRP][srp-swift] | Swift | [![Build][srp-swift-b-img]][srp-swift-b] |
| [srp.net][srp-net] | .NET: Standard 1.6+, Framework 3.5+ | [![Version][srp-net-v-img]][srp-net-v] [![Build][srp-net-b-img]][srp-net-b] |
| [srptools][srptools] | Python: 2, 3 | [![Version][srptools-v-img]][srptools-v] [![Build][srptools-b-img]][srptools-b] |
| [pysrp][pysrp][^1] | Python 2, 3 | [![Version][pysrp-v-img]][pysrp-v] |
| [Windwalker SRP][ww-github] ([PHP][ww-pkg] / [JS][ww-npm]) | PHP, JS (TS) | [![Version][ww-v-php]][ww-pkg] [![Version][ww-v-js]][ww-npm]


[^1]: Compatibility with `pysrp` requires usage of `rfc5054_enable()` in that library. The library also requires padding of the generator `g` before deriving the session variables. For more details on how to workaround that with the other SRP implementations, see [srp.net/issues/19][srp-net-issue-19].

## Adding an implementation to the list

1. Ensure the compatibility using one of the above mentioned libraries.
2. Fork the repository.
3. Add your implementation into this file.
4. Make a pull request.


[srp-swift]: <https://github.com/Bouke/SRP>
[srp-swift-b]: <https://travis-ci.org/Bouke/SRP>
[srp-swift-b-img]: <https://travis-ci.org/Bouke/SRP.svg?branch=master>

[srp-net]: <https://github.com/secure-remote-password/srp.net>
[srp-net-v]: <https://www.nuget.org/packages/srp>
[srp-net-v-img]: <https://img.shields.io/nuget/v/srp.svg>
[srp-net-b]: <https://ci.appveyor.com/project/yallie/srp-net>
[srp-net-b-img]: <https://img.shields.io/appveyor/ci/yallie/srp-net.svg>
[srp-net-issue-19]: <https://github.com/secure-remote-password/srp.net/issues/19>

[srptools]: <https://github.com/idlesign/srptools>
[srptools-v]: <https://pypi.python.org/pypi/srptools>
[srptools-v-img]: <https://img.shields.io/pypi/v/srptools.svg>
[srptools-b]: <https://github.com/idlesign/srptools/actions/workflows/ci.yaml>
[srptools-b-img]: <https://github.com/idlesign/srptools/actions/workflows/ci.yaml/badge.svg?event=push>

[pysrp]: <https://github.com/cocagne/pysrp>
[pysrp-v]: <https://pypi.python.org/pypi/srp>
[pysrp-v-img]: <https://img.shields.io/pypi/v/srp.svg>

[ww-github]: <https://github.com/windwalker-io/srp>
[ww-pkg]: <https://packagist.org/packages/windwalker/srp>
[ww-npm]: <https://www.npmjs.com/package/@windwalker-io/srp>
[ww-v-php]: <https://img.shields.io/packagist/v/windwalker/srp.svg>
[ww-v-js]: <https://img.shields.io/npm/v/%40windwalker-io/srp.svg>

# Serial

<a href="https://jsr.io/@serial/serial"><img align="right" src="https://github.com/Serial-IO/.github/blob/main/assets/profile.svg" width="180px" alt="the serial port standing in the rain"></a>

[![Lint](https://github.com/Serial-IO/serial/actions/workflows/lint.yml/badge.svg)](https://github.com/Serial-IO/serial/actions/workflows/lint.yml)
[![Unit Tests](https://github.com/Serial-IO/serial/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/Serial-IO/serial/actions/workflows/unit_tests.yml)
[![JSR](https://jsr.io/badges/@serial/serial)](https://jsr.io/@serial/serial)

A [serial](https://en.wikipedia.org/wiki/Serial_communication) library written in TypeScript for [Deno](https://deno.land) without any third party modules.

This library provides an interface for the communication with serial devices and **doesn't use any third party modules**. It uses C++ functions which are compiled to dynamic libraries. These functions are then loaded by Deno to establish a serial connection and talk to the devices.

## Features
- Communication with serial devices.
- Create multiple serial connections at the same time.
- List available ports and their properties (if available).
- Set timeouts for both reading and writing.
- Async functions.
- Uses no third party modules.
- Works on multiple different operating systems (check [compatibility](#compatibility) for more info).

## Compatibility
| OS      | Tested version          | Current state                           |
|---------|-------------------------|-----------------------------------------|
| Windows | Windows 10 (x64)        | in progress                             |
| Linux   | Ubuntu Server 22.04 LTS | in progress                             |
| MacOS   | -                       | planned (contributions are appreciated) |

## Overview
The library consists of:
- The [Serial](https://github.com/Serial-IO/serial) library (Source Code for TypeScript Serial library)
- The core [C++ Core](https://github.com/Serial-IO/cpp-core) (Source Code for C++ Core)
- The higher level [C++ bindings (Windows)](https://github.com/Serial-IO/cpp-bindings-windows) (Source Code for C++ higher level bindings for Windows platforms)
- The higher level [C++ bindings (Linux)](https://github.com/Serial-IO/cpp-bindings-linux) (Source Code for C++ higher level bindings for Linux platforms)
- The higher level [C++ bindings (MacOS)](https://github.com/Serial-IO/cpp-bindings-macos) (Source Code for C++ higher level bindings for MacOS platforms)

## Documentation/Examples
- [Serial](https://github.com/Serial-IO/serial): Check out the [Wiki](https://github.com/Serial-IO/serial/wiki) section on how to use the TypeScript library.
- [C++ Core](https://github.com/Serial-IO/cpp-core): Check out the [Wiki](https://github.com/Serial-IO/cpp-core/wiki) section on how to use the C++ Core.
- [C++ bindings (Windows)](https://github.com/Serial-IO/cpp-bindings-windows): Check out the [Wiki](https://github.com/Serial-IO/cpp-bindings-windows/wiki) section on how to use the C++ bindings for Windows.
- [C++ bindings (Linux)](https://github.com/Serial-IO/cpp-bindings-linux): Check out the [Wiki](https://github.com/Serial-IO/cpp-bindings-linux/wiki) section on how to use the C++ bindings for Linux.
- [C++ bindings (MacOS)](https://github.com/Serial-IO/cpp-bindings-macos): Check out the [Wiki](https://github.com/Serial-IO/cpp-bindings-macos/wiki) section on how to use the C++ bindings for MacOS.

## Community/Discussions
Get in touch with the community [here](https://github.com/orgs/Serial-IO/discussions) or provide feedback and suggestions for the library.

Found a bug? Feel free to [open an issue](https://github.com/Serial-IO/serial/issues/new?template=bug_report.yml).

## Credits
- Big thanks goes out to [@Katze719](https://github.com/Katze719) who wrote most of the C++ files and functions!
- Thanks to [@AapoAlas](https://github.com/aapoalas) any many others for the great support and help on the [Deno Discord](https://discord.gg/deno)!
- Thanks to [@Dj](https://github.com/DjDeveloperr) for the inspiration on how to write such a library!

## Licence
- [Serial](https://github.com/Serial-IO/serial): `GPLv2.1` Check [LICENSE](https://github.com/Serial-IO/serial/blob/main/LICENSE) for more details.
- [C++ Core](https://github.com/Serial-IO/cpp-core): `LGPL-2.0` Check [LICENSE](https://github.com/Serial-IO/cpp-core/blob/main/LICENSE) for more details.
- [C++ bindings (Windows)](https://github.com/Serial-IO/cpp-bindings-windows): `LGPL-2.0` Check [LICENSE](https://github.com/Serial-IO/cpp-bindings-windows/blob/main/LICENSE) for more details.
- [C++ bindings (Linux)](https://github.com/Serial-IO/cpp-bindings-linux): `LGPL-2.0` Check [LICENSE](https://github.com/Serial-IO/cpp-bindings-linux/blob/main/LICENSE) for more details.

Feel free to contribute to this project.

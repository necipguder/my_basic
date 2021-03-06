![](resource/icon.ico)

Copyright (C) 2011 - 2015 W. Renxin

## Introduction

MY-BASIC is a tiny cross-platform easy extendable BASIC interpreter written in pure C with about 6000 lines of source code. Its grammar is similar to structured BASIC in early era, but without line number. It is aimed to be either an embeddable scripting language or a standalone interpreter. The core is pretty light; all in a C source file and an associated header file. You can combine MY-BASIC with an existing C/C++/Objective-C project easily, scripting driven can make your projects more powerful, elegant and neat.

## Main features

* It is free
* Written in clean ANSI C, source code portable
* Most GW-BASIC like syntax, but without line numbers
* Small (within memory usage less than 128KB) and fast
* Case-insensitive tokens
* Integer/float point/string/boolean/array data types support
* User customizable type support
* `IF-THEN-ELSEIF-ELSE-ENDIF` support
* `FOR-TO-STEP-NEXT/WHILE-WEND/DO-UNTIL` support
* `GOTO/GOSUB-RETURN` support
* Numeric functions
* String functions
* It's able to use it as a standalone interpreter, or integrate it with existing C/C++/Objective-C projects, or learn how to build an interpreter from scratch
* It's able to build your own dialect based on it
* Debug APIs
* High expansibility, easy to use APIs, easy to write customized scripting interfaces
* More features/modules under developing

## Installation

### Use standalone interpreter binary

This repository contains precompiled binaries for [Win32](output/my_basic.exe) and [MacOS](output/my_basic_mac), it's efficient to download it and have a first impressive playground.

To compile an interpreter binary for your own platform, please see the steps as follow.

* Retrieve `core` and `shell` folders
* Setup your compile toolchain configuration
* Use your compiler to process `core/my_basic.c` and `shell/main.c`, both require including `core/my_basic.h`

### Combine with exist projects

MY-BASIC is cleanly written in a single C source file and an associated header file. Just copy `my_basic.c` and `my_basic.h` to your project folder and add them to a build configuration.

You can definitely [link with MY-BASIC as a lib](https://github.com/paladin-t/my_basic/wiki/Link-with-MY_BASIC) as well.

For more details about using MY-BASIC when it's already integrated with exist projects, please see [MY-BASIC Quick Reference](MY-BASIC%20Quick%20Reference.pdf).

## [WIKI](https://github.com/paladin-t/my_basic/wiki)

* [Workflow](https://github.com/paladin-t/my_basic/wiki/Workflow)
* [Link with MY-BASIC](https://github.com/paladin-t/my_basic/wiki/Link-with-MY_BASIC)
* [Redirect PRINT and INPUT](https://github.com/paladin-t/my_basic/wiki/Redirect-PRINT-and-INPUT)
* [Redefine int_t and real_t](https://github.com/paladin-t/my_basic/wiki/Redefine-int_t-and-real_t)
* [Use usertype values](https://github.com/paladin-t/my_basic/wiki/Use-usertype-values)
* [Customize macros](https://github.com/paladin-t/my_basic/wiki/Customize-macros)
* [Write a debugger](https://github.com/paladin-t/my_basic/wiki/Write-a-debugger)
* [More scripting APIs](https://github.com/paladin-t/my_basic/wiki/More-scripting-APIs)
 * [File module](https://github.com/paladin-t/my_basic/wiki/File-module)
* [FAQ](https://github.com/paladin-t/my_basic/wiki/FAQ)

## References

* [BASIC - Wikipedia](http://en.wikipedia.org/wiki/BASIC)
* [MY-BASIC Quick Reference](MY-BASIC%20Quick%20Reference.pdf)

-----

You can support MY-BASIC development with a donation:
<br>
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=hellotony521%40gmail%2ecom&lc=US&item_name=my-basic&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHostedGuest)

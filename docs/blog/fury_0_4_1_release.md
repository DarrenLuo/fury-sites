# Fury v0.4.1 released

Author: [chaokunyang](https://github.com/chaokunyang)

I'm pleased to announce the 0.4.1 release of the Fury: https://github.com/alipay/fury/releases/tag/v0.4.1. With this release, Fury support rust row format now. C++ row format has been enhanced too, now iterable types can be encoded to fury row format too.

## Highlight
* [Rust] Support row format
* [C++] Support iterable types for RowEncoder 
* [JavaScript] Support partial record
* [Java] Fix JIT error in corner case, now Fury can generate serializer for every class

## What's Changed
* [Doc] Refine issue template by a yaml form by @chaokunyang in https://github.com/alipay/fury/pull/1185
* [C++] Fix ownership problem for children writers by visitor by @PragmaTwice in https://github.com/alipay/fury/pull/1193
* [C++] Remove useless fields and macro in logging by @PragmaTwice in https://github.com/alipay/fury/pull/1195
* [Doc] add docs for java FuryBuilder #1188 by @mof-dev-3 in https://github.com/alipay/fury/pull/1192
* [Rust] support row format by @wangweipeng2 in https://github.com/alipay/fury/pull/1196
* [C++] Add RowEncoder wrapper to RowEncodeTrait by @PragmaTwice in https://github.com/alipay/fury/pull/1200
* [Rust] Row support more types by @wangweipeng2 in https://github.com/alipay/fury/pull/1202
* [Rust] Support row map by @wangweipeng2 in https://github.com/alipay/fury/pull/1206
* [C++] update bazel version from 4.2 to 6.3.2 by @chaokunyang in https://github.com/alipay/fury/pull/1204
* [JavaScript] Support partial record by @wangweipeng2 in https://github.com/alipay/fury/pull/1208
* [Java] fix package access level class accessor jit by @chaokunyang in https://github.com/alipay/fury/pull/1210
* [JavaScript] Fix register a description twice will get undefined serializer by @bytemain in https://github.com/alipay/fury/pull/1211
* [C++] Support iterable types in RowEncodeTrait by @PragmaTwice in https://github.com/alipay/fury/pull/1212
* [C++] Support iterable types for RowEncoder by @PragmaTwice in https://github.com/alipay/fury/pull/1215
* [Python] Refine py register class method by @chaokunyang in https://github.com/alipay/fury/pull/1218
* [Java] Clear extRegistry.getClassCtx if generate serializer class failed in https://github.com/alipay/fury/pull/1221

## New Contributors
* @bytemain made their first contribution in https://github.com/alipay/fury/pull/1211

**Full Changelog**: https://github.com/alipay/fury/compare/v0.4.0...v0.4.1
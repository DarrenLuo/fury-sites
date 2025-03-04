# Fury v0.4.0 released

Author: [chaokunyang](https://github.com/chaokunyang)

I'm pleased to announce the 0.4.0 release of the Fury. With this release, [GraalVM native image](https://www.graalvm.org/latest/reference-manual/native-image/) and C++ row format automatic encoder based on compile-time reflection are supported. Please try it out and share your feedbacks with us. 

## Highlight
* [Java] Support Graalvm native image. The implementation will generate all serialization code at image build time, the runtime will be extremely fast, see [fury graalvm usage doc](https://github.com/alipay/fury/blob/main/docs/guide/graalvm_guide.md)
* [Java] Fury vs JDK benchmark on Graalvm native image
* [Scala] Serialization support for package scoped object
* [C++] Reflection support by macro/template programing
* [C++] Automatic row format encoder

## What's Changed
* [Python] fix python release by @chaokunyang in https://github.com/alipay/fury/pull/1125
* [Java] make unsafe offset compatible with graalvm by @chaokunyang in https://github.com/alipay/fury/pull/1117
* [Scala] Fix scala package object JIT error by @chaokunyang in https://github.com/alipay/fury/pull/1130
* [Java] Refine maven pom config by @chaokunyang in https://github.com/alipay/fury/pull/1126
* [Rust]  add rust building by @caicancai in https://github.com/alipay/fury/pull/1129
* [C++] Remove useless overload of Writer::WriteString by @PragmaTwice in https://github.com/alipay/fury/pull/1136
* [Rust] fix typo by @caicancai in https://github.com/alipay/fury/pull/1133
* [Rust]  add mesaage about rust ci by @caicancai in https://github.com/alipay/fury/pull/1131
* [C++] Add move ctor/assign op to Status by @PragmaTwice in https://github.com/alipay/fury/pull/1134
* [Rust] fix cargo test error by @wangweipeng2 in https://github.com/alipay/fury/pull/1135
* [Rust] improve rust ci by @caicancai in https://github.com/alipay/fury/pull/1138
* [Scala] Fix scala collection serialization nested in pojo by @chaokunyang in https://github.com/alipay/fury/pull/1140
* [Java] make sting builder serializer codegen eager by @chaokunyang in https://github.com/alipay/fury/pull/1141
* [Rust] fix rust ci bug by @caicancai in https://github.com/alipay/fury/pull/1139
* [Java] support add static fields in fury codegen by @chaokunyang in https://github.com/alipay/fury/pull/1147
* [C++] Add the basic row format serializer for C++ class types via reflection by @PragmaTwice in https://github.com/alipay/fury/pull/1144
* [C++] Add duplicated fields detection in `FURY_FIELD_INFO` macro by @PragmaTwice in https://github.com/alipay/fury/pull/1151
* [Java] support create serializer when register class by @chaokunyang in https://github.com/alipay/fury/pull/1154
* [Java] Support graalvm native image by @chaokunyang in https://github.com/alipay/fury/pull/1143
* [C++] Support string type in RowEncoder by @PragmaTwice in https://github.com/alipay/fury/pull/1158
* [Scala] add graalvm support for scala singleton by @chaokunyang in https://github.com/alipay/fury/pull/1159
* [Scala] Fix scala singleton map/collection serialization in struct by @chaokunyang in https://github.com/alipay/fury/pull/1160
* [Java] add read resolve circular test suite by @chaokunyang in https://github.com/alipay/fury/pull/1161
* [Java] Remove load arrow serializers by default by @chaokunyang in https://github.com/alipay/fury/pull/1163
* [Java] Support thread safe fury for graalvm native image by @chaokunyang in https://github.com/alipay/fury/pull/1164
* [Scala] Fix package object serialization in scala App by @chaokunyang in https://github.com/alipay/fury/pull/1166
* [Java] add graalvm usage doc by @chaokunyang in https://github.com/alipay/fury/pull/1168
* [C++] Split util.h to bit_util.h and time_util.h by @PragmaTwice in https://github.com/alipay/fury/pull/1171
* [C++] Support cv-qualified types in row encoder by @PragmaTwice in https://github.com/alipay/fury/pull/1172
* [C++] Add support for nested class types in row encoder by @PragmaTwice in https://github.com/alipay/fury/pull/1173
* [Java] Add graalvm benchmark by @chaokunyang in https://github.com/alipay/fury/pull/1178
* [Java] Fix string key serializer ref tracking by @chaokunyang in https://github.com/alipay/fury/pull/1174
* [Java] Add graalvm benchmark test results by @chaokunyang in https://github.com/alipay/fury/pull/1180
* [Scala] fix package object inaccessible from source code by @chaokunyang in https://github.com/alipay/fury/pull/1181


**Full Changelog**: https://github.com/alipay/fury/compare/v0.3.1...v0.4.0
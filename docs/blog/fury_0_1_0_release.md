# Fury v0.1.0 released

Author: [chaokunyang](https://github.com/chaokunyang)

I'm excited to release Fury v0.1.0 . Fury 0.1.0 is our first release since we started the development in github in 2023.04.28, and open sourced in 2023.07.15. 

In this release we closed 314 issues, 412 PRs, and we have 5 new contributors. Thanks for their contributions to fury, looking forward to further cooperation with them.

This release includes many features, see more details on https://github.com/alipay/fury/releases/tag/v0.1.0:
- Production-ready java serialization: 
  - Highly optimized Java serialization primives
  - Runtime codegen framework
  - Interpreter mode java serialization
  - JIT accelerated serializer for java serialization
  - Support async and multi-thread JIT
  - Support type forward-backward compatibility.
  - Support meta sharing to send class meta only once.
  - Support JDK custom serialization on fury natively. 
  - Out-of-band zero-copy serialization for java
- Cross language Serialization
  - Support basic types cross-language between java/python/javascript/rust
  - Support struct cross-language automatically, no need for IDL definition
  - Supports shared and circular reference object serialization between java/python/javascript.
  - Support object polymorphism between java/python/javascript.
  - Out-of-band zero-copy serialization between java/python
- Row format
  - Support row format between java/python/c++.
  - Support lazy/partial deserialization.
  - Support convert to arrow format automatically.


With this release, we take big strides towards our goal of making serialization fast, cross-language, unified and open.
For details, please refer to the following commit messages.

Note that javascript/rust support is still experimental, please let us know if you have any issues.

## New Contributors
* @wangweipeng2 made their first contribution in https://github.com/alipay/fury/pull/215
* @rainsonGain made their first contribution in https://github.com/alipay/fury/pull/429
* @leeco-cloud made their first contribution in https://github.com/alipay/fury/pull/436
* @dependabot made their first contribution in https://github.com/alipay/fury/pull/590
* @tisonkun made their first contribution in https://github.com/alipay/fury/pull/762
* @hieu-ht made their first contribution in https://github.com/alipay/fury/pull/786
* @s31k31 made their first contribution in https://github.com/alipay/fury/pull/782

## What's Changed
* Create pull_request_template.md by @chaokunyang in https://github.com/alipay/fury/pull/2
* add apache licence file by @chaokunyang in https://github.com/alipay/fury/pull/3
* [Java] add java code structure by @chaokunyang in https://github.com/alipay/fury/pull/4
* [Java] add java code formatter by @chaokunyang in https://github.com/alipay/fury/pull/5
* [Java] Add licence to file header by @chaokunyang in https://github.com/alipay/fury/pull/6
* [Docs] add fury debug doc by @chaokunyang in https://github.com/alipay/fury/pull/8
* [Docs] refine readme by fix syntax error by @chaokunyang in https://github.com/alipay/fury/pull/10
* [Community] add getting involved document by @chaokunyang in https://github.com/alipay/fury/pull/12
* [Java] add java ci by @chaokunyang in https://github.com/alipay/fury/pull/14
* [Java] fix license format conflict with checkstyle by @chaokunyang in https://github.com/alipay/fury/pull/16
* [Java] Add unsafe memory util by @chaokunyang in https://github.com/alipay/fury/pull/18
* [Java] add tuple2/tuple3 utils by @chaokunyang in https://github.com/alipay/fury/pull/20
* [Java] add LoggerFactory for disable logging more easily by @chaokunyang in https://github.com/alipay/fury/pull/22
* [Java] add string utils by @chaokunyang in https://github.com/alipay/fury/pull/24
* [Java] add memory read/write utils by @chaokunyang in https://github.com/alipay/fury/pull/26
* [Community] update slack invite link by @chaokunyang in https://github.com/alipay/fury/pull/27
* [Java] add cross-language type id by @chaokunyang in https://github.com/alipay/fury/pull/35
* [Java] Add api annotation to mark api stability by @chaokunyang in https://github.com/alipay/fury/pull/37
* [Java] add int array to avoid box cost by @chaokunyang in https://github.com/alipay/fury/pull/39
* [Java] add auto-growing object array by @chaokunyang in https://github.com/alipay/fury/pull/41
* [Java] Add optimized map for faster lookup by @chaokunyang in https://github.com/alipay/fury/pull/43
* [Java] add basic type inference support by @chaokunyang in https://github.com/alipay/fury/pull/45
* [Java] Add long map support by @chaokunyang in https://github.com/alipay/fury/pull/47
* [Java] add fury exceptions by @chaokunyang in https://github.com/alipay/fury/pull/48
* [Java] add MurmurHash3 support by @chaokunyang in https://github.com/alipay/fury/pull/50
* [Java] add Reflection support by @chaokunyang in https://github.com/alipay/fury/pull/52
* add FieldAccessor and fields compare by @chaokunyang in https://github.com/alipay/fury/pull/54
* [Java] implement basic compiler backend based on janino by @chaokunyang in https://github.com/alipay/fury/pull/56
* [Java] Add extensible classloaders by @chaokunyang in https://github.com/alipay/fury/pull/58
* [Java] Support multi key weak map by @chaokunyang in https://github.com/alipay/fury/pull/60
* [Java] codegen framework for fury java jit by @chaokunyang in https://github.com/alipay/fury/pull/61
* [Java] add utility for lambda functions by @chaokunyang in https://github.com/alipay/fury/pull/63
* [Java] add common expression ir for programing construct by @chaokunyang in https://github.com/alipay/fury/pull/64
* [Java] fix if expression with return child node by @chaokunyang in https://github.com/alipay/fury/pull/66
* [Java] add expression tree traverser and updater by @chaokunyang in https://github.com/alipay/fury/pull/68
* [Java] add missing author java odc by @chaokunyang in https://github.com/alipay/fury/pull/69
* [Java] add enum string resolver support by @chaokunyang in https://github.com/alipay/fury/pull/72
* [Java] add reference tracking support by @chaokunyang in https://github.com/alipay/fury/pull/74
* [Java] add java serializer interface by @chaokunyang in https://github.com/alipay/fury/pull/76
* [Java] add test utils by @chaokunyang in https://github.com/alipay/fury/pull/77
* [Java] add generics hierarchy resolving support by @chaokunyang in https://github.com/alipay/fury/pull/79
* [Java] add serialization context to relate serializing different objects by @chaokunyang in https://github.com/alipay/fury/pull/82
* [Java] add class info util by @chaokunyang in https://github.com/alipay/fury/pull/83
* [Java] add buffer callback by @chaokunyang in https://github.com/alipay/fury/pull/87
* [Java] implement basic java serialization framework by @chaokunyang in https://github.com/alipay/fury/pull/88
* [Java] Add string serializer by @chaokunyang in https://github.com/alipay/fury/pull/90
* [Java] add string builder/buffer serializers by @chaokunyang in https://github.com/alipay/fury/pull/93
* [Java] add missing uint serializers tests by @chaokunyang in https://github.com/alipay/fury/pull/95
* [Java] Implement enum serialization for java by @chaokunyang in https://github.com/alipay/fury/pull/97
* [Java] Implement bigint/decimal serialization for java by @chaokunyang in https://github.com/alipay/fury/pull/101
* [Community] add zhihu link by @chaokunyang in https://github.com/alipay/fury/pull/103
* [Community] fix zhihu link by @chaokunyang in https://github.com/alipay/fury/pull/104
* [Community] update slack desc by @chaokunyang in https://github.com/alipay/fury/pull/105
* [Java] Add object array serializer by @chaokunyang in https://github.com/alipay/fury/pull/107
* [Java] Implement primitive array serializers by @chaokunyang in https://github.com/alipay/fury/pull/109
* [Java] support serializing byte buffer by @chaokunyang in https://github.com/alipay/fury/pull/113
* [Java] support serializing java.util.concurrent.atomics by @chaokunyang in https://github.com/alipay/fury/pull/115
* [Java] move string array serializers by @chaokunyang in https://github.com/alipay/fury/pull/116
* [Java] support Currency serialization by @chaokunyang in https://github.com/alipay/fury/pull/118
* [Java] support charset serialization by @chaokunyang in https://github.com/alipay/fury/pull/120
* [Java] support URI serialization by @chaokunyang in https://github.com/alipay/fury/pull/122
* [Java] add support for regex serialization by @chaokunyang in https://github.com/alipay/fury/pull/124
* [Java] support uuid serialization by @chaokunyang in https://github.com/alipay/fury/pull/126
* [Java] add class serialization test by @chaokunyang in https://github.com/alipay/fury/pull/127
* [Java] add Locale Serializer support by @chaokunyang in https://github.com/alipay/fury/pull/129
* [Java] fix LocaleSerializer cache thread safety by @chaokunyang in https://github.com/alipay/fury/pull/132
* [Java] serialization support for java.util.OptionalXXX by @chaokunyang in https://github.com/alipay/fury/pull/134
* [Java] Add time serializers by @chaokunyang in https://github.com/alipay/fury/pull/137
* [Java] add ObjectInput/Output based on fury by @chaokunyang in https://github.com/alipay/fury/pull/139
* [Java] add JavaSerializer based on ObjectInputStream/ObjectOutputStream by @chaokunyang in https://github.com/alipay/fury/pull/141
* [Java] implement jdk proxy serialization by @chaokunyang in https://github.com/alipay/fury/pull/143
* [Java] implement Externalizable serialization by @chaokunyang in https://github.com/alipay/fury/pull/145
* [Java] implement Collection serialization by @chaokunyang in https://github.com/alipay/fury/pull/147
* [Java] add sortedset serializer by @chaokunyang in https://github.com/alipay/fury/pull/149
* [Java] add empty collection serializer by @chaokunyang in https://github.com/alipay/fury/pull/151
* [Java] add single collection serializers by @chaokunyang in https://github.com/alipay/fury/pull/153
* [Java] add ConcurrentSkipListSet serializer by @chaokunyang in https://github.com/alipay/fury/pull/155
* [Java] add java.util.Vector serializer by @chaokunyang in https://github.com/alipay/fury/pull/157
* [Java] add java.util.ArrayDeque serializer by @chaokunyang in https://github.com/alipay/fury/pull/159
* [Java] add java.util.EnumSet serializer by @chaokunyang in https://github.com/alipay/fury/pull/161
* [Java] implement java.util.BitSet serializer by @chaokunyang in https://github.com/alipay/fury/pull/163
* [Java] implement java.util.PriorityQueue serialization by @chaokunyang in https://github.com/alipay/fury/pull/165
* [Java] implement map serialization framework by @chaokunyang in https://github.com/alipay/fury/pull/167
* [Java] support java.util.SortedMap serialization by @chaokunyang in https://github.com/alipay/fury/pull/169
* [Java] support empty map serialization by @chaokunyang in https://github.com/alipay/fury/pull/171
* [Java] implement singleton map serialization by @chaokunyang in https://github.com/alipay/fury/pull/173
* [Java] support concurrent map serialization by @chaokunyang in https://github.com/alipay/fury/pull/175
* [Java] implement enum map serialization by @chaokunyang in https://github.com/alipay/fury/pull/177
* [Java] group and sort descriptors for cache and consistency by @chaokunyang in https://github.com/alipay/fury/pull/179
* [Java] Implement object serialization by @chaokunyang in https://github.com/alipay/fury/pull/181
* [Java] fury native lambda serialization for java by @chaokunyang in https://github.com/alipay/fury/pull/183
* Update feature_request.md by @chaokunyang in https://github.com/alipay/fury/pull/184
* Update bug_report.md by @chaokunyang in https://github.com/alipay/fury/pull/185
* Update bug_report.md by @chaokunyang in https://github.com/alipay/fury/pull/186
* [Java] Optimize Collections.synchronized serialization performance by @chaokunyang in https://github.com/alipay/fury/pull/188
* [Java] optimize unmodifiable serialization by @chaokunyang in https://github.com/alipay/fury/pull/191
* [Java] add native readResolve/writeReplace serialization support by @chaokunyang in https://github.com/alipay/fury/pull/193
* [Java] [1/N] support type forward/backward compatibility by @chaokunyang in https://github.com/alipay/fury/pull/196
* [Java] Add struct util to create test struct class dynamically by @chaokunyang in https://github.com/alipay/fury/pull/199
* Revert "[Java] Add struct util to create test struct class dynamically" by @chaokunyang in https://github.com/alipay/fury/pull/200
* [Java] Add struct util to create test struct class dynamically by @chaokunyang in https://github.com/alipay/fury/pull/201
* [Java][2/N] support type forward/backward compatibility by @chaokunyang in https://github.com/alipay/fury/pull/195
* [Java] Optimize subclass container serialization by @chaokunyang in https://github.com/alipay/fury/pull/205
* [Java] remove generated classes automatically by @chaokunyang in https://github.com/alipay/fury/pull/207
* [Java] implement collection serialization field by field by @chaokunyang in https://github.com/alipay/fury/pull/209
* [Java] implement java map serialization field by field by @chaokunyang in https://github.com/alipay/fury/pull/210
* [Java] optimize jdk compatible collection serializer by @chaokunyang in https://github.com/alipay/fury/pull/212
* [Java] support compatible map serialization by @chaokunyang in https://github.com/alipay/fury/pull/213
* [JavaScript] javascript of fury by @wangweipeng2 in https://github.com/alipay/fury/pull/215
* [JavaScript]Replace Nodejs lib by standard lib by @wangweipeng2 in https://github.com/alipay/fury/pull/217
* [JavaScript]Add test by @wangweipeng2 in https://github.com/alipay/fury/pull/219
* [JavaScript] Change package.json entry file by @wangweipeng2 in https://github.com/alipay/fury/pull/221
* Update feature_request.md by @chaokunyang in https://github.com/alipay/fury/pull/223
* [Java] implement fury-native jdk compatible object serialization by @chaokunyang in https://github.com/alipay/fury/pull/222
* [Java] Add class def for meta sharing by @chaokunyang in https://github.com/alipay/fury/pull/226
* [Java] Support meta shared serialization by @chaokunyang in https://github.com/alipay/fury/pull/225
* [Java] add missing license to ObjectStreamSerializer by @chaokunyang in https://github.com/alipay/fury/pull/228
* [Java] move loadClass to ClassUtils by @chaokunyang in https://github.com/alipay/fury/pull/229
* [javascript] add javascript ci by @chaokunyang in https://github.com/alipay/fury/pull/230
* Fix CI by @chaokunyang in https://github.com/alipay/fury/pull/232
* [Java] forbid classes serialization by blacklist by @chaokunyang in https://github.com/alipay/fury/pull/234
* [Java] generate field accessor on the flight by @chaokunyang in https://github.com/alipay/fury/pull/240
* [Java] expression optimizer for method split by @chaokunyang in https://github.com/alipay/fury/pull/241
* [JavaScript]Fix ci by @wangweipeng2 in https://github.com/alipay/fury/pull/242
* [Java] add codec builder base class by @chaokunyang in https://github.com/alipay/fury/pull/244
* [Java] add jdk serializable check by @chaokunyang in https://github.com/alipay/fury/pull/248
* [Java] add base object serializer builder by @chaokunyang in https://github.com/alipay/fury/pull/249
* [Java] Implement jit serialization for object by @chaokunyang in https://github.com/alipay/fury/pull/250
* [Java] Fix meta shared serializer when jit enabled by @chaokunyang in https://github.com/alipay/fury/pull/252
* Update bug_report.md by @chaokunyang in https://github.com/alipay/fury/pull/253
* [Java] type forward/backward compatible jit serializer by @chaokunyang in https://github.com/alipay/fury/pull/254
* [Java] Meta shared object jit serializer by @chaokunyang in https://github.com/alipay/fury/pull/255
* [Java] jit context for manage compilation by @chaokunyang in https://github.com/alipay/fury/pull/259
* [Java] fix javaFury thread safety by @chaokunyang in https://github.com/alipay/fury/pull/261
* [Java] set rootdir for maven multi-module project by @chaokunyang in https://github.com/alipay/fury/pull/263
* [Java] add guava immutable list serializer by @chaokunyang in https://github.com/alipay/fury/pull/264
* [Java] add guava immutable map serializer by @chaokunyang in https://github.com/alipay/fury/pull/266
* [Java] Async compilation for jit serializers by @chaokunyang in https://github.com/alipay/fury/pull/268
* [Java] add url serializer by @chaokunyang in https://github.com/alipay/fury/pull/269
* [Java] optimize java serialization by @chaokunyang in https://github.com/alipay/fury/pull/271
* [Java] bind fury with classloader by @chaokunyang in https://github.com/alipay/fury/pull/274
* [Java] add forward serializer by @chaokunyang in https://github.com/alipay/fury/pull/276
* [Java] add thread-safe fury serializer by @chaokunyang in https://github.com/alipay/fury/pull/278
* [Java] Add guava/sublist todo serializer by @chaokunyang in https://github.com/alipay/fury/pull/282
* [Java] add zero-copy tests by @chaokunyang in https://github.com/alipay/fury/pull/284
* [Java] Profiling fury init by @chaokunyang in https://github.com/alipay/fury/pull/286
* [Java] add complex cyclic tests by @chaokunyang in https://github.com/alipay/fury/pull/288
* [Java] enable testArrayStructZeroCopy by @chaokunyang in https://github.com/alipay/fury/pull/290
* [Java] add complex collection struct tests by @chaokunyang in https://github.com/alipay/fury/pull/292
* [Java] add complex map struct tests by @chaokunyang in https://github.com/alipay/fury/pull/294
* [Java] misc serializer tests by @chaokunyang in https://github.com/alipay/fury/pull/295
* [Java] optimize time reference by @chaokunyang in https://github.com/alipay/fury/pull/297
* [Java] add unsafe accessor test for duplicate fields by @chaokunyang in https://github.com/alipay/fury/pull/299
* [Java] add serializer factory test by @chaokunyang in https://github.com/alipay/fury/pull/301
* [Java] add duplicate fields tests by @chaokunyang in https://github.com/alipay/fury/pull/303
* [Java] add protocol interoperability tests by @chaokunyang in https://github.com/alipay/fury/pull/305
* [Java] Lazy map support by @chaokunyang in https://github.com/alipay/fury/pull/307
* [Java] Support deserialize unexisted classes by @chaokunyang in https://github.com/alipay/fury/pull/309
* [Java] fix OutOfBandTest pkg by @chaokunyang in https://github.com/alipay/fury/pull/310
* javascript latin1 string performance improvement by @wangweipeng2 in https://github.com/alipay/fury/pull/312
* [Java] Add row format interface by @chaokunyang in https://github.com/alipay/fury/pull/316
* [Java] add Default arrow type visitor by @chaokunyang in https://github.com/alipay/fury/pull/318
* [Java] add decimal util by @chaokunyang in https://github.com/alipay/fury/pull/320
* [Java] add pyarrow style data types API in java by @chaokunyang in https://github.com/alipay/fury/pull/322
* [Java] add fury InputStream/OutputStream by @chaokunyang in https://github.com/alipay/fury/pull/324
* [Java] Infer arrow schema for java bean by @chaokunyang in https://github.com/alipay/fury/pull/326
* [Java] add bitmap utils by @chaokunyang in https://github.com/alipay/fury/pull/328
* [Java] binary row format data structure by @chaokunyang in https://github.com/alipay/fury/pull/330
* [Java] binary row format writer by @chaokunyang in https://github.com/alipay/fury/pull/333
* [Java] add arrow visitor for value accessor by @chaokunyang in https://github.com/alipay/fury/pull/335
* [Java] add row format tests by @chaokunyang in https://github.com/alipay/fury/pull/337
* [Java] add row format encoder interface by @chaokunyang in https://github.com/alipay/fury/pull/339
* [Java] Base builder for building jit encoder by @chaokunyang in https://github.com/alipay/fury/pull/341
* [Java] add jit-based row encoder implementation by @chaokunyang in https://github.com/alipay/fury/pull/343
* [Java] format code by @chaokunyang in https://github.com/alipay/fury/pull/344
* [Java] add missing license by @chaokunyang in https://github.com/alipay/fury/pull/345
* [Java] Add fury channel by @chaokunyang in https://github.com/alipay/fury/pull/346
* [Java] Mock io for count bytes by @chaokunyang in https://github.com/alipay/fury/pull/349
* [Java] Arrow record batch zero-copy serializers by @chaokunyang in https://github.com/alipay/fury/pull/351
* [Java] Add missing license by @chaokunyang in https://github.com/alipay/fury/pull/352
* [Java] optimize decimal encoding performance by @chaokunyang in https://github.com/alipay/fury/pull/354
* [Java] optimize schema creation perf by @chaokunyang in https://github.com/alipay/fury/pull/356
* [Java] update row javadoc by @chaokunyang in https://github.com/alipay/fury/pull/357
* [Java] Support convert row to arrow format by @chaokunyang in https://github.com/alipay/fury/pull/359
* [Java] add arrow serializers tests  by @chaokunyang in https://github.com/alipay/fury/pull/361
* [Java] fix arrow tests by @chaokunyang in https://github.com/alipay/fury/pull/362
* [Java] add serialize to buffer tests by @chaokunyang in https://github.com/alipay/fury/pull/364
* [Java] add basic cross-langauge serialization tests by @chaokunyang in https://github.com/alipay/fury/pull/366
* [Java] add serializeBeanTest by @chaokunyang in https://github.com/alipay/fury/pull/367
* [Java] add registerTest by @chaokunyang in https://github.com/alipay/fury/pull/368
* [Java] add testTreeMap by @chaokunyang in https://github.com/alipay/fury/pull/369
* [Java] add offheap tests by @chaokunyang in https://github.com/alipay/fury/pull/371
* [Java] refine classresovler tests by @chaokunyang in https://github.com/alipay/fury/pull/373
* [Java] add private bean tests by @chaokunyang in https://github.com/alipay/fury/pull/375
* [Java] add blocking queue test by @chaokunyang in https://github.com/alipay/fury/pull/377
* [Java] add duplicate fields test by @chaokunyang in https://github.com/alipay/fury/pull/378
* [Java] add guava tests by @chaokunyang in https://github.com/alipay/fury/pull/381
* [Java] add test for jdk serializable check by @chaokunyang in https://github.com/alipay/fury/pull/383
* [Java] add secure mode test by @chaokunyang in https://github.com/alipay/fury/pull/385
* [Java] ensure fury doesn't introduce class leak by @chaokunyang in https://github.com/alipay/fury/pull/387
* [Java] add tests for ignoring fields  by @chaokunyang in https://github.com/alipay/fury/pull/389
* [Java] add thread to blacklist by @chaokunyang in https://github.com/alipay/fury/pull/391
* [Java] Add complex testsuite by @chaokunyang in https://github.com/alipay/fury/pull/393
* [Java] add benchmark framework by @chaokunyang in https://github.com/alipay/fury/pull/399
* [Java] add plotting tool by @chaokunyang in https://github.com/alipay/fury/pull/400
* [Java] add usertype benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/401
* [Java] Add string benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/403
* [Java] add array benchmark by @chaokunyang in https://github.com/alipay/fury/pull/405
* [Java] add map benchmark by @chaokunyang in https://github.com/alipay/fury/pull/409
* [Java] add memory benchmark by @chaokunyang in https://github.com/alipay/fury/pull/410
* [Java] add row format benchmark by @chaokunyang in https://github.com/alipay/fury/pull/411
* [Java] add zero copy benchmark by @chaokunyang in https://github.com/alipay/fury/pull/413
* [Java] Add flatbufffer/protobuffer benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/415
* [Java] update integration_tests readme by @chaokunyang in https://github.com/alipay/fury/pull/416
* [C++] generate arrow bazel depdencies from pyarrow bundled shared library  by @chaokunyang in https://github.com/alipay/fury/pull/418
* [C++] Add bazel C++ build support by @chaokunyang in https://github.com/alipay/fury/pull/420
* [C++] add c++ logging util by @chaokunyang in https://github.com/alipay/fury/pull/423
* [C++] add cpp status util by @chaokunyang in https://github.com/alipay/fury/pull/425
* [C++] basic util for bytes operations  by @chaokunyang in https://github.com/alipay/fury/pull/427
* Update bug_report.md by @chaokunyang in https://github.com/alipay/fury/pull/430
* [Java] register class check duplciate id  by @chaokunyang in https://github.com/alipay/fury/pull/432
* [Java] move ExpressionOptimizer into codegen package by @chaokunyang in https://github.com/alipay/fury/pull/433
* Format/container encoder by @rainsonGain in https://github.com/alipay/fury/pull/429
* [Java] Thread-safe fury implementation by pooling by @leeco-cloud in https://github.com/alipay/fury/pull/436
* [C++] Add c++ buffer util  by @chaokunyang in https://github.com/alipay/fury/pull/438
* [CI] fix CI by @chaokunyang in https://github.com/alipay/fury/pull/439
* [C++] Binary row format for c++  by @chaokunyang in https://github.com/alipay/fury/pull/441
* [C++] C++ row format to arrow by @chaokunyang in https://github.com/alipay/fury/pull/442
* [C++] Add c++ ci by @chaokunyang in https://github.com/alipay/fury/pull/444
* [CI] Add code lint ci job by @chaokunyang in https://github.com/alipay/fury/pull/446
* [Doc] Add c++ debugging doc by @chaokunyang in https://github.com/alipay/fury/pull/448
* [Python] [1/n] Fury python binding by @chaokunyang in https://github.com/alipay/fury/pull/450
* [python] Type infer for python by @chaokunyang in https://github.com/alipay/fury/pull/458
* [Java] skip checkstyle in java test by @chaokunyang in https://github.com/alipay/fury/pull/459
* [Python] Fix python ci by @chaokunyang in https://github.com/alipay/fury/pull/461
* [Python] Python row format by @chaokunyang in https://github.com/alipay/fury/pull/463
* [Python] Python encoder for row format by @chaokunyang in https://github.com/alipay/fury/pull/466
* [Python] Row and arrow format converter by @chaokunyang in https://github.com/alipay/fury/pull/467
* [C++] cpp murmurhash by @chaokunyang in https://github.com/alipay/fury/pull/469
* [Python] Python murmur hash binding by @chaokunyang in https://github.com/alipay/fury/pull/472
* [Python] add weak key identity map by @chaokunyang in https://github.com/alipay/fury/pull/474
* [Python] add reference resolver by @chaokunyang in https://github.com/alipay/fury/pull/476
* [Python] Implement python serialization framework by @chaokunyang in https://github.com/alipay/fury/pull/478
* [Python] add common python serializers by @chaokunyang in https://github.com/alipay/fury/pull/480
* [Python] struct serialization support  by @chaokunyang in https://github.com/alipay/fury/pull/482
* [Java] Fix get super type exception by @chaokunyang in https://github.com/alipay/fury/pull/484
* [Java] fix map final value type serializer in jit compatible mode by @chaokunyang in https://github.com/alipay/fury/pull/485
* [Docs] add fury logo by @chaokunyang in https://github.com/alipay/fury/pull/487
* [Docs] add square fury logo by @chaokunyang in https://github.com/alipay/fury/pull/488
* [python] add cpp reference resolver based on abseil map by @chaokunyang in https://github.com/alipay/fury/pull/493
* [python] add cpp class resolver by @chaokunyang in https://github.com/alipay/fury/pull/494
* [Python] cython serialization framework by @chaokunyang in https://github.com/alipay/fury/pull/496
* [Python] cython basic serializers by @chaokunyang in https://github.com/alipay/fury/pull/501
* [Python] cython container serializers by @chaokunyang in https://github.com/alipay/fury/pull/502
* [Pyhton] cython array serializers by @chaokunyang in https://github.com/alipay/fury/pull/503
* [Python] cython struct serializer by @chaokunyang in https://github.com/alipay/fury/pull/505
* [Python] cython misc serializers by @chaokunyang in https://github.com/alipay/fury/pull/506
* [Python] Unify cython python serializer by @chaokunyang in https://github.com/alipay/fury/pull/507
* [Python] Codegen serialization support by @chaokunyang in https://github.com/alipay/fury/pull/509
* [Python] Support arrow serialization in objgraph by @chaokunyang in https://github.com/alipay/fury/pull/515
* [Python] Add common pytests by @chaokunyang in https://github.com/alipay/fury/pull/517
* [C++] pin bazel to 4.2.0 by @chaokunyang in https://github.com/alipay/fury/pull/519
* [Community] Update contacts about wechat/dingding by @chaokunyang in https://github.com/alipay/fury/pull/521
* [Java] support struct cross language serialization by @chaokunyang in https://github.com/alipay/fury/pull/523
* [Java] add java/python cross language row format tests by @chaokunyang in https://github.com/alipay/fury/pull/525
* feat: fix qrcode size in readme by @wangweipeng2 in https://github.com/alipay/fury/pull/526
* [Java] replace io.furyx with org.furyio by @chaokunyang in https://github.com/alipay/fury/pull/527
* [Java] Add missing map license by @chaokunyang in https://github.com/alipay/fury/pull/529
* [Java] reduce string serializer caller stack by jit by @chaokunyang in https://github.com/alipay/fury/pull/531
* [Java] fix nested map generics by @chaokunyang in https://github.com/alipay/fury/pull/533
* [Java] fix jdk11 string jit serialization by @chaokunyang in https://github.com/alipay/fury/pull/535
* [JavaScript] improve write performance by @wangweipeng2 in https://github.com/alipay/fury/pull/538
* [Java] refine java benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/536
* [Java] fix fury java kryo/fst benchmark classloading by @chaokunyang in https://github.com/alipay/fury/pull/542
* [Java] Unsafe method invoke optimization by @chaokunyang in https://github.com/alipay/fury/pull/543
* [Java] Optimize string serialization mem ops by @chaokunyang in https://github.com/alipay/fury/pull/545
* [Java] Optimze jit generated code by @chaokunyang in https://github.com/alipay/fury/pull/548
* [Java] Optimize primitive fields jit read/write by @chaokunyang in https://github.com/alipay/fury/pull/550
* [Java] Fix benchmark plot by @chaokunyang in https://github.com/alipay/fury/pull/554
* [Java] Upload benchmark data by @chaokunyang in https://github.com/alipay/fury/pull/555
* [Docs] Update benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/560
* [Docs] use a smaller size for benchmark plots by @chaokunyang in https://github.com/alipay/fury/pull/561
* [Docs] update docs by @chaokunyang in https://github.com/alipay/fury/pull/565
* [Doc] update docs by @chaokunyang in https://github.com/alipay/fury/pull/566
* [Docs] update readme by @chaokunyang in https://github.com/alipay/fury/pull/567
* [JavaScript] Import js write performance by @wangweipeng2 in https://github.com/alipay/fury/pull/569
* [Docs ] fix benchmarks figures align by @chaokunyang in https://github.com/alipay/fury/pull/571
* [Docs] fix python typehint comment by @chaokunyang in https://github.com/alipay/fury/pull/572
* [Docs] add row format to arrow conversion java example by @chaokunyang in https://github.com/alipay/fury/pull/573
* [JavaScript] update benchmark by @wangweipeng2 in https://github.com/alipay/fury/pull/574
* [JavaScript] easy type description by @wangweipeng2 in https://github.com/alipay/fury/pull/576
* [JavaScript] add generic constraints to the serializer by @wangweipeng2 in https://github.com/alipay/fury/pull/577
* [Docs] Refine benchmark plots by @chaokunyang in https://github.com/alipay/fury/pull/578
* [Docs] fix java header by @chaokunyang in https://github.com/alipay/fury/pull/582
* [Python] support secure mode for python by @chaokunyang in https://github.com/alipay/fury/pull/584
* [Docs] update readme speedup by @chaokunyang in https://github.com/alipay/fury/pull/585
* [Docs] remove `Binary Serialization` from header by @chaokunyang in https://github.com/alipay/fury/pull/586
* [Docs] add Serialization to header by @chaokunyang in https://github.com/alipay/fury/pull/587
* [Docs] fix invalid image links in cpp debug doc by @chaokunyang in https://github.com/alipay/fury/pull/589
* Bump protobuf-java from 3.11.0 to 3.16.3 in /java/fury-benchmark by @dependabot in https://github.com/alipay/fury/pull/590
* Bump testng from 7.3.0 to 7.5.1 in /java by @dependabot in https://github.com/alipay/fury/pull/591
* Bump checkstyle from 8.19 to 8.29 in /java by @dependabot in https://github.com/alipay/fury/pull/592
* Bump guava from 30.0-jre to 32.0.0-jre in /java by @dependabot in https://github.com/alipay/fury/pull/593
* Bump protobuf-java from 3.15.0 to 3.16.3 in /integration_tests by @dependabot in https://github.com/alipay/fury/pull/594
* [Java] replace log4j by log4j2 for test modules by @chaokunyang in https://github.com/alipay/fury/pull/595
* [JavaScript] update benchmark by @wangweipeng2 in https://github.com/alipay/fury/pull/597
* [Java] rename reference to ref by @chaokunyang in https://github.com/alipay/fury/pull/599
* [Java] fix checkstyle failure by @chaokunyang in https://github.com/alipay/fury/pull/602
* [Java] fix missing reference renaming by @chaokunyang in https://github.com/alipay/fury/pull/603
* [Java] Rename requireClassRegistration by @chaokunyang in https://github.com/alipay/fury/pull/604
* [JavaScript]: remove dependency on v8 by @wangweipeng2 in https://github.com/alipay/fury/pull/606
* [Rust] Add readme for fury rust by @chaokunyang in https://github.com/alipay/fury/pull/607
* [Java] add missing license for java code by @chaokunyang in https://github.com/alipay/fury/pull/608
* [Java] update java benchmarks by @chaokunyang in https://github.com/alipay/fury/pull/609
* [Docs] update java benchmarks chart size by @chaokunyang in https://github.com/alipay/fury/pull/610
* [Docs] use same color for fury best performance by @chaokunyang in https://github.com/alipay/fury/pull/611
* [Java] add MetaContext tests by @chaokunyang in https://github.com/alipay/fury/pull/613
* [Java] Add java misc tests by @chaokunyang in https://github.com/alipay/fury/pull/614
* [Java] Add codegen class loading/gc tests by @chaokunyang in https://github.com/alipay/fury/pull/616
* [Java] add warn logs when requireClassRegistration disabled by @chaokunyang in https://github.com/alipay/fury/pull/618
* [Docs] Add java adcanced user guide doc by @chaokunyang in https://github.com/alipay/fury/pull/621
* [Docs] Update java advanced doc by @chaokunyang in https://github.com/alipay/fury/pull/625
* [JavaScript] Eliminate polymorphism in JS code by @wangweipeng2 in https://github.com/alipay/fury/pull/627
* [Python] rename reference to ref for python by @chaokunyang in https://github.com/alipay/fury/pull/629
* [Java/Python] Rename crosslanguage to x by @chaokunyang in https://github.com/alipay/fury/pull/631
* [JavaScript] reduce generated code size by @wangweipeng2 in https://github.com/alipay/fury/pull/633
* [Java] update java snapshot url by @chaokunyang in https://github.com/alipay/fury/pull/635
* [CI] Enable Fury CI by @chaokunyang in https://github.com/alipay/fury/pull/636
* [Docs] add benchmark data by @chaokunyang in https://github.com/alipay/fury/pull/639
* [Doc] use camel naming for benchmark class doc by @chaokunyang in https://github.com/alipay/fury/pull/640
* [Docs] Update security doc by @chaokunyang in https://github.com/alipay/fury/pull/642
* [Java] update license for Generics by @chaokunyang in https://github.com/alipay/fury/pull/644
* [Java] fix generics license length by @chaokunyang in https://github.com/alipay/fury/pull/645
* [Java] update java security doc by @chaokunyang in https://github.com/alipay/fury/pull/646
* [Go] update golang readme by @chaokunyang in https://github.com/alipay/fury/pull/648
* [Doc] replace Fury.Language by Language by @chaokunyang in https://github.com/alipay/fury/pull/650
* [Java] update java row readme by @chaokunyang in https://github.com/alipay/fury/pull/651
* [Java] register guava serializers ahead by @chaokunyang in https://github.com/alipay/fury/pull/654
* [Docs] split user guide doc into 3 parts to sync with website by @chaokunyang in https://github.com/alipay/fury/pull/665
* [Docs]  move guide docs to guide by @chaokunyang in https://github.com/alipay/fury/pull/667
* [Doc] sync files to home site by @wangweipeng2 in https://github.com/alipay/fury/pull/666
* [Java] Fix  IndexOutOfBoundsException when new fury deserialize from InputStream by @chaokunyang in https://github.com/alipay/fury/pull/671
* [Doc] support front matter by @wangweipeng2 in https://github.com/alipay/fury/pull/672
* [Doc] rename inner fury to f when creating ThreadSafeFury by @chaokunyang in https://github.com/alipay/fury/pull/676
* [Java] Support string zerocopy for jdk14+ by @chaokunyang in https://github.com/alipay/fury/pull/677
* [CI] Add deploy script by @chaokunyang in https://github.com/alipay/fury/pull/688
* [Java] Support maven release by @chaokunyang in https://github.com/alipay/fury/pull/691
* [Doc] add java release jar for v0.1.0-alpha.1 by @chaokunyang in https://github.com/alipay/fury/pull/693
* [Doc] Fix release jar doc by @chaokunyang in https://github.com/alipay/fury/pull/694
* [Doc] Refine readme for more readability  by @chaokunyang in https://github.com/alipay/fury/pull/695
* [Java] Add detailed lambda error by @chaokunyang in https://github.com/alipay/fury/pull/698
* [Doc] Fix threadsafe example by @chaokunyang in https://github.com/alipay/fury/pull/699
* [Docs] fix threadsafe fury in java guide by @chaokunyang in https://github.com/alipay/fury/pull/700
* [Docs] remove bracket from classLoader by @chaokunyang in https://github.com/alipay/fury/pull/701
* [Java] add maven source plugin by @chaokunyang in https://github.com/alipay/fury/pull/702
* [Java] Jdk serialization binary check by @chaokunyang in https://github.com/alipay/fury/pull/714
* [Java] add jdk migration doc by @chaokunyang in https://github.com/alipay/fury/pull/715
* [Java] Support jit for non public classes by @chaokunyang in https://github.com/alipay/fury/pull/719
* [Rust] rust lang initial version by @wangweipeng2 in https://github.com/alipay/fury/pull/718
* [Java] add type tag registration check by @chaokunyang in https://github.com/alipay/fury/pull/722
* [Doc] highlight warmup by @chaokunyang in https://github.com/alipay/fury/pull/723
* [Rust ] calculate the reserved space on compile time by @wangweipeng2 in https://github.com/alipay/fury/pull/725
* [Java/Python] disable reference tracking by default by @chaokunyang in https://github.com/alipay/fury/pull/727
* [Java] debug log code stats by @chaokunyang in https://github.com/alipay/fury/pull/728
* [Java] upgrade java install to 0.1.0-alpha.2 by @chaokunyang in https://github.com/alipay/fury/pull/731
* [Doc] use fury png logo by @chaokunyang in https://github.com/alipay/fury/pull/733
* [Doc] remove margin fury png logo by @chaokunyang in https://github.com/alipay/fury/pull/734
* [Doc] Refine logo and icon by @chaokunyang in https://github.com/alipay/fury/pull/735
* [ Rust ] Make the protocols of rust and js consistent by @wangweipeng2 in https://github.com/alipay/fury/pull/738
* [JavaScript] Make the protocols of rust and js consistent by @wangweipeng2 in https://github.com/alipay/fury/pull/739
* [Java] Remove guava from userdoc by @chaokunyang in https://github.com/alipay/fury/pull/740
* [Java] rename writeNonRefT to writeNonRef by @chaokunyang in https://github.com/alipay/fury/pull/743
* [Java] Optimize object array serialization by @chaokunyang in https://github.com/alipay/fury/pull/741
* [Java] avoid reflection in resolve/replace by @chaokunyang in https://github.com/alipay/fury/pull/744
* [Java] avoid reflection in writeObject/readOject/readObjectNoData by @chaokunyang in https://github.com/alipay/fury/pull/747
* [Java] optimize guava list serialization by @chaokunyang in https://github.com/alipay/fury/pull/748
* [Java] add MakeJDKFunction lambda factory by @chaokunyang in https://github.com/alipay/fury/pull/752
* [Java] Optimize guava List/Map/Set serialization by @chaokunyang in https://github.com/alipay/fury/pull/750
* [Doc] Add contributing guide doc  by @chaokunyang in https://github.com/alipay/fury/pull/759
* [Doc] Create CODE_OF_CONDUCT.md by @chaokunyang in https://github.com/alipay/fury/pull/761
* [Doc] Fix broken link in README by @tisonkun in https://github.com/alipay/fury/pull/762
* [Rust] Several Rust idioms by @tisonkun in https://github.com/alipay/fury/pull/763
* [Java] fix write replace class failure by @chaokunyang in https://github.com/alipay/fury/pull/767
* [Java] replace withSecureMode by requireClassRegistration API by @chaokunyang in https://github.com/alipay/fury/pull/768
* [Doc] Update README.md by @chaokunyang in https://github.com/alipay/fury/pull/770
* [Doc] add javadoc for FuryBuilder by @chaokunyang in https://github.com/alipay/fury/pull/775
* [Doc] add doc for fury creation reuse by @chaokunyang in https://github.com/alipay/fury/pull/777
* [Java][Python] auto deploy java/python packages by @chaokunyang in https://github.com/alipay/fury/pull/781
* [Java] refine FuryBuilder API by @chaokunyang in https://github.com/alipay/fury/pull/784
* [CI] skip release tests by @chaokunyang in https://github.com/alipay/fury/pull/785
* Corrected grammar and paraphrasing to make the README easier to read by @hieu-ht in https://github.com/alipay/fury/pull/786
* Don't let CI run when the changed files are not the code by @hieu-ht in https://github.com/alipay/fury/pull/787
* [Java] use lambda for SynchronizedSerializers factory by @chaokunyang in https://github.com/alipay/fury/pull/789
* [Java] use lambda for unmodifiable serializers factory by @chaokunyang in https://github.com/alipay/fury/pull/790
* [Python] replace alpha/beta to a/b for python by @chaokunyang in https://github.com/alipay/fury/pull/792
* [Python] fix python bump version by @chaokunyang in https://github.com/alipay/fury/pull/793
* [CI] Fix bump version by @chaokunyang in https://github.com/alipay/fury/pull/795
* [CI] Fix py release by @chaokunyang in https://github.com/alipay/fury/pull/796
* [Doc] update python and java install by @chaokunyang in https://github.com/alipay/fury/pull/797
* Update README.md by @chaokunyang in https://github.com/alipay/fury/pull/800
* [Doc] Update java install version to 0.1.0-alpah.5 by @chaokunyang in https://github.com/alipay/fury/pull/801
* [CI] Fix pypi upload by @chaokunyang in https://github.com/alipay/fury/pull/803
* [Java] Add core java developer to maven pom by @chaokunyang in https://github.com/alipay/fury/pull/802
* [Java] add core java developer to maven modules pom by @chaokunyang in https://github.com/alipay/fury/pull/804
* [Java] support decode utf8 for java string serialization by @chaokunyang in https://github.com/alipay/fury/pull/806
* Update Java Deserialization Blacklist by @s31k31 in https://github.com/alipay/fury/pull/782
* chore: apply license format by @tisonkun in https://github.com/alipay/fury/pull/783
* [Java] use soft reference to avoid duplicate codegen by @chaokunyang in https://github.com/alipay/fury/pull/809

**Full Changelog**: https://github.com/alipay/fury/commits/v0.1.0
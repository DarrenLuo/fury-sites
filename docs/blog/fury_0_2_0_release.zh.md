# Fury v0.2.0 released

Author: [chaokunyang](https://github.com/chaokunyang)

很高兴向大家宣布Fury 0.2.0的发布，`0.2.0`是一个非常重量级的版本，该版本性能提升一倍，序列化体积减少`30%~50%`，目前性能是Java序列化排行榜[JVM-Serializers](https://github.com/eishay/jvm-serializers/wiki)第一。同时我们全面支持了JDK17/21，支持了JDK17+ record JIT序列化，JDK9+ ImmutableList的JIT序列化, 具备极致的性能，并保持了`JDK8~21`跨版本之间的兼容性。同时该版本我们开源了Fury GoLang序列化框架，该框架是业界第一个支持循环引用和接口多态的golang序列化框架，欢迎使用。

## Highlights
### Java
* Support JDK17+ record JIT/Interpreter serialization
* Support JDK17+ record JIT/Interpreter serialization backward/forward compatibility
* Support jdk9+ Immutable Collections JIT/Interpreter mode serialization, much faster compared to other frameworks
* New collection serialization protocol by homogenization, 1.5x speed up, 2X space saving.
* Desgined and implemented a new long compression algorithm, with performance cost less than 10% but give 50% compresstion ratio
* Support configuring compress int/long independently, enable int/long compression by default
* Add class checker API and Whitelist/Blacklist based implementation to enhance security

### Python
* Support pyarrow6 bazel build
* Support python 3.10

### JavaScript
* [JavaScript] support fury for browser
* [JavaScript] support polymorphism
* [JavaScript] enhancement performance

### Golang
* Implement Golang serialization framework, which support reference, pointer, data serialization
* Implement serializers for string/numbers/slice/map/slice/struct/pointer

## What's Changed
* [JavaScript] enhancement performance and bugfix by @wangweipeng2 in https://github.com/alipay/fury/pull/811
* [JavaScript] support polymorphism by @wangweipeng2 in https://github.com/alipay/fury/pull/814
* Create SECURITY.md by @chaokunyang in https://github.com/alipay/fury/pull/817
* [JavaScript] fix bug #703 by @wangweipeng2 in https://github.com/alipay/fury/pull/819
* [Java] fix isSecure check for xlang in java by @chaokunyang in https://github.com/alipay/fury/pull/822
* [Doc] add  protocol wire format wip by @chaokunyang in https://github.com/alipay/fury/pull/823
* [JavaScript] write tag hash by @wangweipeng2 in https://github.com/alipay/fury/pull/825
* [JavaScript] support browser by @wangweipeng2 in https://github.com/alipay/fury/pull/830
* [Java] register empty object by default by @chaokunyang in https://github.com/alipay/fury/pull/829
* [Java] upgrade guava for CVE-2023-2976 by @chaokunyang in https://github.com/alipay/fury/pull/831
* [JavaScript]  detect platform wrong by @wangweipeng2 in https://github.com/alipay/fury/pull/832
* [JavaScript] add test by @wangweipeng2 in https://github.com/alipay/fury/pull/836
* [Java] Add compatible ci for JDK8/11/13/15/17 by @chaokunyang in https://github.com/alipay/fury/pull/835
* [Java] use java.lang.ClassValue to cache Lookup by @chaokunyang in https://github.com/alipay/fury/pull/844
* [Java] Refactor integration tests by @chaokunyang in https://github.com/alipay/fury/pull/845
* [Java] suppress maven download logs by --no-transfer-progress by @chaokunyang in https://github.com/alipay/fury/pull/846
* [Java] add missing jdk primitive function by @chaokunyang in https://github.com/alipay/fury/pull/848
* [Java] make getter lambda functions by @chaokunyang in https://github.com/alipay/fury/pull/849
* [Java] add record utils by @chaokunyang in https://github.com/alipay/fury/pull/850
* [Java] Support access record field value by @chaokunyang in https://github.com/alipay/fury/pull/851
* [Java] interpreter mode support for record serialization by @chaokunyang in https://github.com/alipay/fury/pull/852
* [CI] Fix checkstyle by @chaokunyang in https://github.com/alipay/fury/pull/853
* [Java] Support jdk record forward/backward interpreter serialization by @chaokunyang in https://github.com/alipay/fury/pull/854
* [Java] Support jdk record metashare mode by @chaokunyang in https://github.com/alipay/fury/pull/855
* [Java] move record utils to record pkg by @chaokunyang in https://github.com/alipay/fury/pull/856
* [Java] move inner functions outside by @chaokunyang in https://github.com/alipay/fury/pull/857
* [Python] Support pyarrow6 bazel build by @chaokunyang in https://github.com/alipay/fury/pull/859
* [Python] add missing shared lib for python by @chaokunyang in https://github.com/alipay/fury/pull/862
* [Python] fix python deploy by @chaokunyang in https://github.com/alipay/fury/pull/863
* [Java] Jdk record compatible jit by @chaokunyang in https://github.com/alipay/fury/pull/864
* [Java] JIT serialization for JDK record  by @chaokunyang in https://github.com/alipay/fury/pull/866
* [Java] support private record jit by @chaokunyang in https://github.com/alipay/fury/pull/869
* [Java] optimize buffer copy by @chaokunyang in https://github.com/alipay/fury/pull/870
* [Doc] Fix row format doc by @chaokunyang in https://github.com/alipay/fury/pull/873
* [Java] Support compress int long independently by @chaokunyang in https://github.com/alipay/fury/pull/875
* [Java] fix ofHashMap by @chaokunyang in https://github.com/alipay/fury/pull/877
* [Java] add jdk tools.jar for tests by @chaokunyang in https://github.com/alipay/fury/pull/881
* [Java] register common exception by @chaokunyang in https://github.com/alipay/fury/pull/879
* [Java] Fix lazy bean serializer by @chaokunyang in https://github.com/alipay/fury/pull/883
* [Java] print exception for fury creation by @chaokunyang in https://github.com/alipay/fury/pull/885
* [Java] remove getCurrentFury API by @chaokunyang in https://github.com/alipay/fury/pull/887
* [Java] Add fury map iterator api by @chaokunyang in https://github.com/alipay/fury/pull/889
* [Java] Add class checker API by @chaokunyang in https://github.com/alipay/fury/pull/890
* [Python] Fix python linux deploy missing shared library files by @chaokunyang in https://github.com/alipay/fury/pull/892
* [Java] refine AllowListChecker by @chaokunyang in https://github.com/alipay/fury/pull/893
* Update README.md by @chaokunyang in https://github.com/alipay/fury/pull/894
* [Java] support immutable collection/map jit and generics optimization by @chaokunyang in https://github.com/alipay/fury/pull/895
* [Java] cache generated guava constructor by @chaokunyang in https://github.com/alipay/fury/pull/897
* [Java] Optimize jdk9+ immutable collection serialization  by @chaokunyang in https://github.com/alipay/fury/pull/900
* [Java] add jdk20 tests by @chaokunyang in https://github.com/alipay/fury/pull/901
* [Java] optimize duplicate fields utils by @chaokunyang in https://github.com/alipay/fury/pull/905
* [Java] fix jit error for package-level field with private type by @chaokunyang in https://github.com/alipay/fury/pull/907
* [Java] update blacklist by @chaokunyang in https://github.com/alipay/fury/pull/913
* [Python] Use cloudpickle for local function serialization by @chaokunyang in https://github.com/alipay/fury/pull/914
* [Python] fix row format getter by @chaokunyang in https://github.com/alipay/fury/pull/915
* [Java] disable class check by default by @chaokunyang in https://github.com/alipay/fury/pull/917
* [Java] refine java docs by @chaokunyang in https://github.com/alipay/fury/pull/918
* Update blacklist.txt by @chaokunyang in https://github.com/alipay/fury/pull/920
* [Java] Skip `toString` in annotation invocation handler `readObject` by @chaokunyang in https://github.com/alipay/fury/pull/922
* Optimize StringBuilder/StringBuffer serialization by @pandalee99 in https://github.com/alipay/fury/pull/908
* Bump release versin to 0.1.2 by @chaokunyang in https://github.com/alipay/fury/pull/924
* [Doc] add basic type java format doc by @chaokunyang in https://github.com/alipay/fury/pull/928
* [Java] speed test codegen speed by avoid duplicate codegen by @chaokunyang in https://github.com/alipay/fury/pull/929
* [Java] Optimize collection serialization protocol by homogenization by @chaokunyang in https://github.com/alipay/fury/pull/923
* Bump org.apache.avro:avro from 1.11.1 to 1.11.3 in /java/fury-benchmark by @dependabot in https://github.com/alipay/fury/pull/931
* [Java] Rename classinfocache to classinfoholder by @chaokunyang in https://github.com/alipay/fury/pull/933
* [Java] put together all primitive serializers by @chaokunyang in https://github.com/alipay/fury/pull/934
* [Java] Fix jvm crash caused by varint out-of-bound writing by @chaokunyang in https://github.com/alipay/fury/pull/937
* [Java] enable int compression by default by @chaokunyang in https://github.com/alipay/fury/pull/935
* [Java] put together all fury related config classes into `config` package by @chaokunyang in https://github.com/alipay/fury/pull/940
* [Java] Add SLI(small long as int) long encoding algorithm by @chaokunyang in https://github.com/alipay/fury/pull/942
* [Java] use raw type serializer for getSerialzier in jit by @chaokunyang in https://github.com/alipay/fury/pull/943
* [Java] use varint for class id encoding to reduce space cost by @chaokunyang in https://github.com/alipay/fury/pull/945
* [Java] Fix Collection/Map jit/interpreter protocol inconsisitency for generics instantiated subclass by @chaokunyang in https://github.com/alipay/fury/pull/947
* [Go] add fury go util and ci tests by @chaokunyang in https://github.com/alipay/fury/pull/950
* [Go] add fury go buffer implementation by @chaokunyang in https://github.com/alipay/fury/pull/952
* [Go] add fury go serialization framework by @chaokunyang in https://github.com/alipay/fury/pull/954
* [Go] add serializers for common go types by @chaokunyang in https://github.com/alipay/fury/pull/956
* [Java] fix varint writeindex grow for jit by @chaokunyang in https://github.com/alipay/fury/pull/957
* [Go] add fury go map serializer by @chaokunyang in https://github.com/alipay/fury/pull/959
* [Go] add slice serializer for fury go by @chaokunyang in https://github.com/alipay/fury/pull/961
* [Go] add set serializer for fury go by @chaokunyang in https://github.com/alipay/fury/pull/963
* [Go] Add struct serializer for fury go  by @chaokunyang in https://github.com/alipay/fury/pull/965
* [Go] add ref tracking tests by @chaokunyang in https://github.com/alipay/fury/pull/967
* [Go] add fury type dispatch tests by @chaokunyang in https://github.com/alipay/fury/pull/969
* [Go] add fury serialization tests by @chaokunyang in https://github.com/alipay/fury/pull/971
* [Go] Add fury xlang tests by @chaokunyang in https://github.com/alipay/fury/pull/973
* [Go] rename Reference to Ref by @chaokunyang in https://github.com/alipay/fury/pull/975
* [Java] add jdk 21 tests by @chaokunyang in https://github.com/alipay/fury/pull/977
* [Java] add jdk 21 tests ci by @chaokunyang in https://github.com/alipay/fury/pull/978
* [Java] Optimize sli long read/write by @chaokunyang in https://github.com/alipay/fury/pull/981
* [Doc] upgrade docs by @chaokunyang in https://github.com/alipay/fury/pull/985  https://github.com/alipay/fury/pull/986 https://github.com/alipay/fury/pull/987
* [Java] add serializeJavaObject API to ThreadSafeFury by @chaokunyang in https://github.com/alipay/fury/pull/988
* [Java] fix jdk17/21 ci latest_jdk_tests skip by @chaokunyang in https://github.com/alipay/fury/pull/989

## New Contributors
* @pandalee99 made their first contribution in https://github.com/alipay/fury/pull/908
* @ilxqx made their first contribution in https://github.com/fury-project/dubbo-serialization-fury/pull/1
* @T-baby made their first contribution in https://github.com/fury-project/dubbo-serialization-fury/pull/13

**Full Changelog**: https://github.com/alipay/fury/compare/v0.1.0...v0.2.0

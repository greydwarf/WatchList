# WatchList
This is a list of open source tools and libraries I have used, want to use, or at least are worth thinking about. 
Originally, I was using "stars" for this, but I really wanted to be able to group them.

## C++ Libraries
### Core
I will usually use one of these two sets of core libraries. I use Abseil when I am working on a system that is worried about minimizing dependendencies. Otherwise, I use several libraries:
* [abseil](https://abseil.io/) - Abseil is an open-source collection of C++ code (compliant to C++11) designed to augment the C++ standard library. 

_or_
* [cxxopts](https://github.com/jarro2783/cxxopts) -  Lightweight C++ command line option parser.
* [{fmt}](https://fmt.dev) - Small, safe and fast formatting library.
* [parallel-hashmap](https://github.com/greg7mdp/parallel-hashmap) Essentially a reqrite of the Abseil hashmaps and btree implementations, but it has a wrapper around X of them, thus increasing the parallelization significantly.

Then I pick and choose from these, depending on the actual needs:
* [spdlog](https://github.com/gabime/spdlog) - Commonly used logging library
* [libucl](https://github.com/vstakhov/libucl) - Beautiful configuration parser
* [Googletest](https://github.com/google/googletest) - Google Testing and Mocking Framework
* [Google Benchmark](https://github.com/google/benchmark) - A microbenchmark support library
* [backward-cpp](https://github.com/bombela/backward-cpp) - A beautiful stack trace pretty printer for C++. [MIT]
* [Eigen](http://eigen.tuxfamily.org/) - A high-level C++ library of template headers for linear algebra, matrix and vector operations, numerical solvers and related algorithms. [MPL2]
* [PCRE](http://pcre.org/) - A regular expression C library inspired by the regular expression capabilities in Perl. [BSD]

### Compression Libraries
* [bzip2](http://www.bzip.org/) - A freely available, patent free, high-quality data compressor. [BSD]
* [LZ4](https://github.com/lz4/lz4) - Extremely Fast Compression algorithm. [BSD] [website](http://www.lz4.org/)
* [LZMA](http://www.7-zip.org/sdk.html) - The default and general compression method of 7z format. [PublicDomain]
* [Snappy](https://google.github.io/snappy/) - A fast compressor/decompressor. [BSD]
* [zstd](https://github.com/facebook/zstd) - Zstandard - Fast real-time compression algorithm. Developed by Facebook. [BSD]

### Serialization
Most of the time, protobuf is a good balance of features, ease of use, and perfomance. Sometimes though, you just want your data to be human readable and widely adoptable. In that case, reach for JSON. Sometimes you want performance above all else. Flatbuffers is for these cases.
* [FlatBuffers](https://github.com/google/flatbuffers) - A Memory efficient serialization library. [Apache2]
* [protobuf](https://github.com/protocolbuffers/protobuf) - Protocol Buffers - Google's data interchange format. [BSD]
* [json](https://github.com/nlohmann/json) - JSON for Modern C++.

### Threading, Async, etc.
* [Intel TBB](https://www.threadingbuildingblocks.org/) - Intel® Threading Building Blocks. [Apache2]
* [Asio](https://github.com/chriskohlhoff/asio/) - A cross-platform C++ library for network and low-level I/O programming that provides developers with a consistent asynchronous model using a modern C++ approach. [Boost] [website](http://think-async.com/)
* [libuv](https://github.com/libuv/libuv) - Cross-platform asynchronous I/O. [BSD]
* [uvw](https://github.com/skypjack/uvw) - C++ wrapper for libuv. [MIT]


### Database
* [SQLite](http://www.sqlite.org/) - A completely embedded, full-featured relational database in a few 100k that you can include right into your project. [PublicDomain]
* [RocksDB](https://github.com/facebook/rocksdb) - Embedded key-value store for fast storage from facebook. [BSD]
* [Hiredis](https://github.com/redis/hiredis) - A minimalistic C client library for the Redis database. [BSD]
* [libpqxx](https://github.com/jtv/libpqxx) - C++ interface to PostgreSQL [BSD-3]

### IPC
* [cpr](https://github.com/whoshuu/cpr) - C++ Requests: Curl for People, a spiritual port of Python Requests.
* [libcurl](http://curl.haxx.se/libcurl/) - Multiprotocol file transfer library. [MIT/X derivate license]
* [gRPC](https://github.com/grpc/grpc) - A high performance, open source, general-purpose RPC framework. [BSD] [website](http://www.grpc.io/)
* [ZeroMQ](https://github.com/zeromq/libzmq) - High-speed, modular asynchronous communication library. [LGPL] [website](http://zeromq.org/)
* [NATS-C](https://github.com/nats-io/nats.c) - Ultra lightweight messaging system
* [rdkafka](https://github.com/edenhill/librdkafka) - C++ client library for Apache Kafka
* [RabbitMQ](https://github.com/alanxz/rabbitmq-c) - Interact with the RabbitMQ messaging queue in C++

## C++ Tools
* [clang-format](http://clang.llvm.org/docs/ClangFormat.html) - A tool to format C++ code.
* [clangd](https://clang.llvm.org/extra/clangd/) - understands your C++ code and adds smart features to your editor: code completion, compile errors, go-to-definition and more.
* [Compiler Explorer](https://gcc.godbolt.org/) - Interactively explore the assembly output of your C++ code.
* [Valgrind](http://www.valgrind.org/) - is an instrumentation framework for building dynamic analysis tools. There are Valgrind tools that can automatically detect many memory management and threading bugs, and profile your programs in detail. You can also use Valgrind to build new tools.
* [cppcheck](http://cppcheck.sourceforge.net/) - is a static analysis tool for C/C++ code. It provides unique code analysis to detect bugs and focuses on detecting undefined behaviour and dangerous coding constructs. 
* [clang-tidy](http://clang.llvm.org/extra/clang-tidy/) - is a clang-based C++ “linter” tool. Its purpose is to provide an extensible framework for diagnosing and fixing typical programming errors, like style violations, interface misuse, or bugs that can be deduced via static analysis. clang-tidy is modular and provides a convenient interface for writing new checks.
* [clang-analyzer](https://clang.llvm.org/docs/ClangStaticAnalyzer.html) - is a source code analysis tool that finds bugs in C, C++, and Objective-C programs. It implements path-sensitive, inter-procedural analysis based on symbolic execution technique.
* [CMake](https://cmake.org/) - Cross-platform family of tools designed to build, test and package software.
* [Ninja](https://ninja-build.org/) - A small build system with a focus on speed.
* [GCC](https://gcc.gnu.org/) - GNU Compiler Collection. Supports C++11/14/1z C11 and OpenMP. [GNU GPL3]
* [GDB](https://www.gnu.org/software/gdb/) - GNU Debugger.
* [Compiler Explorer](http://gcc.godbolt.org/) - An interactive compiler with assembly output available.

## Developer Tools
* [Jenkins](https://jenkins.io)
* [ripgrep](https://github.com/BurntSushi/ripgrep)
* [fd](https://github.com/sharkdp/fd) - find replacement
* [fzf](https://github.com/junegunn/fzf) - fuzzy searcher plugin for vim, bash, etc.
* [Visual Studio Code](https://code.visualstudio.com/)
* [vim](https://www.vim.org/)
* [tmux](https://github.com/tmux/tmux)

## System Monitoring
* [Telegraf](https://www.influxdata.com/time-series-platform/telegraf) - An open source server agent to help you collect metrics from your stacks, sensors and systems.  The influxdb folks expect you to use influxdb as the backend, but I prefer postgresql (and timescaledb) because I don't want to maintain another DB.
* [Prometheus](https://prometheus.io/) - An open-source systems monitoring and alerting toolkit originally built at SoundCloud.
* [Grafana](https://grafana.com/) - Used by thousands of companies to monitor everything from infrastructure, applications, and power plants to beehives
* [Jaeger](https://www.jaegertracing.io) - Monitor and troubleshoot transactions in complex distributed systems.  Honestly, I haven't ever needed this - simply writing stats out to prometheus has always been good enough.  Its good to know that this is out there, though.

## Cloud
* [Docker](http://docker.com)
* [Consul](https://www.consul.io/docs/platform/k8s/index.html)
* [Envoy](https://www.envoyproxy.io/)
* [Nomad](https://www.hashicorp.com/products/nomad)
* [RancherOS](https://rancher.com) - A lightweight, secure Linux distribution, built from containers to run containers well.

## Database
* [PostgreSQL](https://www.postgresql.org/) - The World's Most Advanced Open Source Relational Database
* [PostGIS](https://postgis.net/) - PostGIS is a spatial database extender for PostgreSQL object-relational database.
* [Timescaledb](https://www.timescale.com/) - Store time correlated data in postgresql quickly
* [Redis](https://redis.io/) - In memory remote data structure store

## Message Queues
* [NATS](https://nats.io) - A simple, secure and high performance open source messaging system for cloud native applications, IoT messaging, and microservices architectures.
* [Kafka](https://kafka.apache.org) - A Distributed streaming platform
* [RabbitMQ](https://www.rabbitmq.com/) - The most widely deployed open source AMPQ broker.

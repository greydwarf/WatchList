# WatchList
This is a list of open source tools and libraries I have used, want to use, or at least are worth thinking about. 
Originally, I was using "stars" for this, but I really wanted to be able to group them.

## C++ Libraries
### Core
* [abseil](https://abseil.io/) - Abseil is an open-source collection of C++ code (compliant to C++11) designed to augment the C++ standard library.  I mostly use this for the B+Tree and hashmap implementations, but the string routines are great, too.
* [cxxopts](https://github.com/jarro2783/cxxopts) -  Lightweight C++ command line option parser.
* [{fmt}](https://fmt.dev) - Small, safe and fast formatting library.
* [loguru](https://github.com/emilk/loguru) - Simple logging library that doe what you expect it to and nothing else.
* [libucl](https://github.com/vstakhov/libucl) - Beautiful configuration parser
* [Googletest](https://github.com/google/googletest) - Google Testing and Mocking Framework.
* [Google Benchmark](https://github.com/google/benchmark) - A microbenchmark support library.
* [backward-cpp](https://github.com/bombela/backward-cpp) - A beautiful stack trace pretty printer for C++. [MIT]
* [Eigen](http://eigen.tuxfamily.org/) - A high-level C++ library of template headers for linear algebra, matrix and vector operations, numerical solvers and related algorithms. [MPL2]
* [PCRE](http://pcre.org/) - A regular expression C library inspired by the regular expression capabilities in Perl. [BSD]


### C++ Compression Libraries
* [bzip2](http://www.bzip.org/) - A freely available, patent free, high-quality data compressor. [BSD]
* [LZ4](https://github.com/lz4/lz4) - Extremely Fast Compression algorithm. [BSD] [website](http://www.lz4.org/)
* [LZMA](http://www.7-zip.org/sdk.html) :zap: - The default and general compression method of 7z format. [PublicDomain]
* [Snappy](https://google.github.io/snappy/) - A fast compressor/decompressor. [BSD]
* [zstd](https://github.com/facebook/zstd) - Zstandard - Fast real-time compression algorithm. Developed by Facebook. [BSD]

### Serialization
* [FlatBuffers](https://github.com/google/flatbuffers) - A Memory efficient serialization library. [Apache2]
* [protobuf](https://github.com/protocolbuffers/protobuf) - Protocol Buffers - Google's data interchange format. [BSD]
* [json](https://github.com/nlohmann/json) - JSON for Modern C++.
* [Vince's CSV Parser](https://github.com/vincentlaucsb/csv-parser) - A fast, self-contained, streaming C++17 CSV parser with optional type-casting and statistics. [MIT]
* [Libxml2](http://xmlsoft.org/) - The XML C parser and toolkit of Gnome. [MIT]


### Threading, Async, etc.
* [Intel TBB](https://www.threadingbuildingblocks.org/) - Intel® Threading Building Blocks. [Apache2]
* [Asio](https://github.com/chriskohlhoff/asio/) - A cross-platform C++ library for network and low-level I/O programming that provides developers with a consistent asynchronous model using a modern C++ approach. [Boost] [website](http://think-async.com/)
* [libuv](https://github.com/libuv/libuv) - Cross-platform asynchronous I/O. [BSD]
* [uvw](https://github.com/skypjack/uvw) - C++ wrapper for libuv. [MIT]


### Database
* [Hiredis](https://github.com/redis/hiredis) - A minimalistic C client library for the Redis database. [BSD]
* [LMDB](http://symas.com/mdb/) - Very fast embedded key/value store with full ACID semantics. [OpenLDAP]
* [LMDB++](https://github.com/bendiken/lmdbxx) - C++11 wrapper for the LMDB embedded database library. [PublicDomain]
* [RocksDB](https://github.com/facebook/rocksdb) - Embedded key-value store for fast storage from facebook. [BSD]
* [SimDB](https://github.com/LiveAsynchronousVisualizedArchitecture/simdb) - High performance, shared memory, lock free, cross platform, single file, minimal dependencies, C++11 key-value store (This is Alpha, but worth keeping an eye on) [Apache2]
* [SQLite](http://www.sqlite.org/) - A completely embedded, full-featured relational database in a few 100k that you can include right into your project. [PublicDomain]

### IPC
* [cpr](https://github.com/whoshuu/cpr) - C++ Requests: Curl for People, a spiritual port of Python Requests.
* [libcurl](http://curl.haxx.se/libcurl/) - Multiprotocol file transfer library. [MIT/X derivate license]
* [gRPC](https://github.com/grpc/grpc) - A high performance, open source, general-purpose RPC framework. [BSD] [website](http://www.grpc.io/)
* [ZeroMQ](https://github.com/zeromq/libzmq) - High-speed, modular asynchronous communication library. [LGPL] [website](http://zeromq.org/)
* [NATS-C](https://github.com/nats-io/nats.c) - Ultra lightweight messaging system
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

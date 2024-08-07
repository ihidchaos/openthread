# c-ares

A C library for asynchronous DNS requests

## URL

https://github.com/c-ares/c-ares/releases/tag/v1.33.0

## Version

v1.33.0

## License

MIT License

## License File

[LICENSE](repo/LICENSE.md)

## Description

c-ares is a modern DNS (stub) resolver library, written in C. It provides interfaces for asynchronous queries while trying to abstract the intricacies of the underlying DNS protocol. It was originally intended for applications which need to perform DNS queries without blocking, or need to perform multiple DNS queries in parallel.

One of the goals of c-ares is to be a better DNS resolver than is provided by your system, regardless of which system you use. We recommend using the c-ares library in all network applications even if the initial goal of asynchronous resolution is not necessary to your application.

c-ares will build with any C89 compiler and is MIT licensed, which makes it suitable for both free and commercial software. c-ares runs on Linux, FreeBSD, OpenBSD, MacOS, Solaris, AIX, Windows, Android, iOS and many more operating systems.

c-ares has a strong focus on security, implementing safe parsers and data builders used throughout the code, thus avoiding many of the common pitfalls of other C libraries. Through automated testing with our extensive testing framework, c-ares is constantly validated with a range of static and dynamic analyzers, as well as being constantly fuzzed by OSS Fuzz.

While c-ares has been around for over 20 years, it has been actively maintained both in regards to the latest DNS RFCs as well as updated to follow the latest best practices in regards to C coding standards.

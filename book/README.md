# Notes on Time Series Database, unpublished edition

The layout is subject to change, and need to merge w/ libtsdb-go

- [01 Overview](01-overview)
  - what is time series data and why we need time series database
- [02 Basic](02-basic)
  - ? might move it into/before storage chapter
  - [Primitive Types](02-basic/primitive/README.md)
    - [Endianess](02-basic/primitive/endianness.md) How to store larger than one byte value
    - [Integer](02-basic/primitive/integer.md) Unsigned and Signed Integer
    - float number and their machine representation (basic for working on compression)
  - statistic, distribution, random etc.
  - maybe information theory
- [03 Data Model](03-data-model)
  - should also contains some basic survey, or link to survey
- [04 Query Language](04-query-language)
  - complex query execution would also be interesting
  - SQL
  - continuous query, prometheus ppl also has an article about it
  - ?query execution? a dedicated chapter?
- [05 Storage](05-storage)
  - [Compression](05-storage/compression)
  - [Index](05-storage/index)
  - local and remote backend (other db, s3 etc.)
  - distributed
- [06 Benchmark](06-benchmark)
  - components
    - workload generator
    - stats collector
    - basic math, distribution
    - historgram and lhdr (forgot what's the name ...)
  - existing tools, their pro can cons
- [07 Analysis](07-analysis) (a.k.a ml a.k.a import ts as tf)
  - prediction
  - anomaly detection
- [08 Monitoring](08-monitoring)
  - ? include log?
- [09 Tracing](09-tracing)
  - (keep it in this repo for now)
- ? IoT and Logging
- 09 OLAP, MPP
- [10 Build](10-build) How to Build a Time Series Database
  - features and components (like how to build relational db/search engine/operating system/programming language etc.)
  - failure injection and correctness validation
  - continuous benchmark

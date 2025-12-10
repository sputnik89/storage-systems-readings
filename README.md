# storage-systems-readings
***This is a copy of the `storage.md` by [debasishg](https://gist.github.com/debasishg) on Gist. A temporary fork is created here for personal uses.***

## Basics

1. [The Log-Structured Merge-Tree (LSM-Tree)](https://www.cs.umb.edu/~poneil/lsmtree.pdf)
2. [B-Tree vs Log-Structured Merge-Tree](https://tikv.github.io/deep-dive-tikv/key-value-engine/B-Tree-vs-Log-Structured-Merge-Tree.html)
3. [Modern B-tree techniques](https://w6113.github.io/files/papers/btreesurvey-graefe.pdf)
4. [More Modern B-Tree Techniques](https://nowpublishers.com/article/Details/DBS-070)
5. [LSM-based Storage Techniques: A Survey](https://arxiv.org/abs/1812.07527)

## B-trees and CPU Caches

1. [B-tree Indexes and CPU Caches](https://cse.unt.edu/~huangyan/6330/Papers/B-tree-Cache-ICDE2001.pdf) by Goetz Graefe and Per-Åke Larson
2. [Cache-Conscious Index Structures for Main-Memory Databases](https://helda.helsinki.fi/server/api/core/bitstreams/eb4ad613-099d-4ba5-bdae-52f7e86ec6d3/content) by Vilho Raatikka
3. [Making B+-Trees Cache Conscious in Main Memory](http://cs.columbia.edu/~kar/pubsk/csbplustrees.ps) by Jun Rao and Kenneth Ross

## Scaling write intensive key-value LSM trees

1. [Monkey: Optimal Navigable Key-Value Store](https://dl.acm.org/doi/10.1145/3035918.3064054) by Niv Dayan et. al.
2. [Dostoevsky: Better Space-Time Trade-Offs for LSM-Tree Based Key-Value Stores via Adaptive Removal of Superfluous Merging](https://dl.acm.org/doi/10.1145/3183713.3196927) by Niv Dayan et. al.
3. [The Log-Structured Merge-Bush & the Wacky Continuum](https://dl.acm.org/doi/10.1145/3299869.3319903) by Niv Dayan et. al.
4. [Scaling Write-Intensive Key-Value Stores](https://youtu.be/b6SI8VbcT4w?si=9g6a7RxpmPhhuNCq) by Niv Dayan

## KV separation in LSM tree based storage engines

1. [Key-Value Separation in LSM Storage Engines](https://www.skyzh.dev/blog/2023-12-31-lsm-kv-separation-overview/)
2. [WiscKey: Separating Keys from Values in SSD-conscious Storage](https://www.usenix.org/conference/fast16/technical-sessions/presentation/lu)
3. [Wayfinder: Speeding up Key-Value Separation by Avoiding I/O Based Indirection](https://dl.acm.org/doi/abs/10.1145/3663351.3663880)
4. [SplitKV: Improve key-value separation store performance by splitting operations](https://ieeexplore.ieee.org/document/10109942)
5. [DumpKV: Learning based lifetime aware garbage collection for key value separation in LSM-tree](https://arxiv.org/abs/2406.01250)
6. [SplitKV: splitting IO paths for different sized key-value items with advanced storage devices](https://dl.acm.org/doi/10.5555/3488733.3488751)

## Variants on LSM Trees

1. [LavaStore: ByteDance’s Purpose-built, High-performance, Cost-effective Local Storage Engine for Cloud Services](https://www.vldb.org/pvldb/vol17/p3799-jiao.pdf)
2. [WALTZ: Leveraging Zone Append to Tighten the Tail Latency of LSM Tree on ZNS SSD](https://www.vldb.org/pvldb/vol16/p2884-lee.pdf)

## Variants on B-Trees

1. [BP-tree: Overcoming the Point-Range Operation Tradeo￿ for In-Memory B-trees](https://www.vldb.org/pvldb/vol16/p2976-xu.pdf)
2. [Bf-Tree: A Modern Read-Write-Optimized Concurrent Larger-Than-Memory Range Index](https://vldb.org/pvldb/vol17/p3442-hao.pdf)

## Research Articles

1. [Stratified B-trees and versioning dictionaries](https://arxiv.org/abs/1103.4282)
2. [Reducing Bloom Filter CPU Overhead in LSM-Trees on Modern Storage Devices](https://dl.acm.org/doi/10.1145/3465998.3466002)
3. [Optimal Bloom Filters and Adaptive Merging for LSM-Trees](https://stratos.seas.harvard.edu/publications/optimal-bloom-filters-and-adaptive-merging-lsm-trees)
4. [SHaMBa: Reducing Bloom Filter Overhead in LSM Trees](https://cs-people.bu.edu/zczhu/files/SHaMBa-VLDB-PhD-Workshop.pdf)
5. [A Comprehensive Performance Evaluation of Modern in-Memory Indices](https://www.comp.nus.edu.sg/~dbsystem/download/xie-icde18-paper.pdf)
6. [FPGA-Accelerated Compactions for LSM-based Key-Value Store](https://www.usenix.org/system/files/fast20-zhang_teng.pdf)
7. [Revisiting the design of LSM-tree Based OLTP storage engine with persistent memory](https://dl.acm.org/doi/abs/10.14778/3467861.3467875)
8. [LB+Trees: optimizing persistent index performance on 3DXPoint memory](https://dl.acm.org/doi/abs/10.14778/3384345.3384355)
9. [SLM-DB: Single-Level Key-Value Store with Persistent Memory](https://www.usenix.org/conference/fast19/presentation/kaiyrakhmet) - this inspired LotusDB
10. [Small Refinements to the DAM Can Have Big Consequences for Data-Structure Design](https://dl.acm.org/doi/10.1145/3323165.3323210) 
11. [External-memory Dictionaries in the Affine and PDAM Models](https://dl.acm.org/doi/10.1145/3470635)
12. [A High Throughput B+tree for SIMD Architectures](https://www.ece.lsu.edu/lpeng/papers/tpds-20-1.pdf)
13. [TreeLine: An Update-In-Place Key-Value Store for Modern Storage](https://www.vldb.org/pvldb/vol16/p99-yu.pdf)
14. [FD-Tree: a Tree Index on Solid State Drives](https://pages.cs.wisc.edu/~yinan/fdtree.html)
15. [Tree Indexing on Solid State Drives](https://pages.cs.wisc.edu/~yinan/paper/fdtree_pvldb.pdf)
16. [Tree Indexing on Flash Disks](https://cse.hkust.edu.hk/catalac/users/yinanli/paper/fdtree_icde09.pdf)
17. [Revisiting B+-tree vs. LSM-tree](https://www.usenix.org/publications/loginonline/revisit-b-tree-vs-lsm-tree-upon-arrival-modern-storage-hardware-built)
18. [Toward a Better Understanding and Evaluation of Tree Structures on Flash SSDs](http://www.vldb.org/pvldb/vol14/p364-didona.pdf)

## Cassandra

1. [Trie Memtables in Cassandra](https://www.vldb.org/pvldb/vol15/p3359-lambov.pdf)
2. [How Cassandra Stores Data: An Exploration of Log Structured Merge Trees](https://hackernoon.com/how-cassandra-stores-data-an-exploration-of-log-structured-merge-trees)

## Percona / TokuDB
Percona XtraDB is an enhanced version of the InnoDB storage engine, designed to better scale on modern hardware.
 
1. [Write Optimization: Myths, Comparison, Clarifications](https://www.percona.com/blog/write-optimization-myths-comparison-clarifications/)<br />
2. [Write Optimization: Myths, Comparison, Clarifications - Part 2](https://www.percona.com/blog/write-optimization-myths-comparison-clarifications-part-2/)<br />
3. [How TokuDB Fractal Tree Indexes work](http://www-db.deis.unibo.it/courses/TBD/Lezioni/mysqluc-2010-fractal-trees.pdf)<br />
4. [TokuMX Fractal Tree(R) indexes, what are they?](https://www.percona.com/blog/tokumx-fractal-treer-indexes-what-are-they/)<br />
5. [A Comparison of Fractal Trees to LSM Trees](http://www.pandademo.com/wp-content/uploads/2017/12/A-Comparison-of-Fractal-Trees-to-Log-Structured-Merge-LSM-Trees.pdf)<br />
6. [Percona Live Slides and Video Available: The Right Read Optimization is Actually Write Optimization](https://www.percona.com/blog/percona-live-slides-and-video-available-the-right-read-optimization-is-actually-write-optimization/)
7. [An article explaining B-trees, LSM trees and Fractal tree indexes](https://dzone.com/articles/how-three-fundamental-data-structures-impact-stora)

## ScyllaDB
An open-source distributed NoSQL wide-column data store. It was designed to be compatible with Apache Cassandra while achieving significantly higher throughputs and lower latencies.

1. [The taming of the B-Trees](https://www.scylladb.com/2021/11/23/the-taming-of-the-b-trees/)

## DuckDB
An in-process SQL OLAP database management system, in process, serverless and optimized for analytics.

1. [Persistent Storage of Adaptive Radix Trees in DuckDB](https://duckdb.org/2022/07/27/art-storage.html)

## SplinterDB
SplinterDB is a key-value store from vmware designed for high performance on fast storage devices.

1. [SplinterDB: Closing the Bandwidth Gap for NVMe Key-Value Stores](https://www.usenix.org/system/files/atc20-conway.pdf)
2. [SplinterDB and Maplets: Improving the Tradeoffs in Key-Value Store Compaction Policy](https://dl.acm.org/doi/abs/10.1145/3588726)
3. [SplinterDB - a key-value store designed for high performance on fast storage devices from vmware](https://github.com/vmware/splinterdb)

## PolarDB
Alibaba Cloud PolarDB is a cloud-native relational database service that decouples computing resources from storage resources and uses integrated software and hardware to provide secure and reliable services with high performance, auto scaling capabilities within seconds, and a large storage capacity.

1. [PolarDB-IMCI: A Cloud-Native HTAP Database System at Alibaba](https://dl.acm.org/doi/10.1145/3589785)
2. [Review: PolarDB-SCC: A Cloud-Native Database Ensuring Low Latency for Strongly Consistent Reads](https://emptysqua.re/blog/review-polardb-scc/)
3. [PolarDB - cloud native distributed sql database from ali baba](https://github.com/polardb)

## LotusDB
LotusDB is the most advanced key-value store written in Go, extremely fast, compatible with LSM tree and B+ tree, and optimization of badger and bbolt.

1. [LotusDB—A fast kv database in Go](https://medium.com/@roseduan520/lotusdb-a-fast-kv-database-in-go-60ea93b2387b)

## FoundationDB
An open source transactional key value store created more than ten years ago. It is one of the first systems to combine the flexibility and scalability of NoSQL architectures with the power of ACID transactions.

1. [FoundationDB: A Distributed Unbundled Transactional Key Value Store](https://dl.acm.org/doi/10.1145/3448016.3457559)
2. [How FoundationDB works and why it works](https://blog.the-pans.com/notes-on-the-foundationdb-paper/)

## OrioleDB
OrioleDB is a new storage engine for PostgreSQL, bringing a modern approach to database capacity, capabilities and performance to the world's most-loved database platform.

1. [OrioleDB – building a modern cloud-native storage engine](https://github.com/orioledb/orioledb) 

## RocksDB
RocksDB is a key-value store targeting large-scale distributed systems and optimized for Solid State Drives (SSDs)

1. [Disaggregating RocksDB: A Production Experience](https://dl.acm.org/doi/10.1145/3589772)
2. [Evolution of Development Priorities in Key-value Stores Serving Large-scale Applications: The RocksDB Experience](https://www.usenix.org/system/files/fast21-dong.pdf)

## VectorDB / Astra(Cassandra)
Vector search integrated with Astra

1. [What is a Vector Database](https://www.datastax.com/guides/what-is-a-vector-database)
2. [5 Hard Problems in Vector Search, and How Cassandra Solves Them](https://thenewstack.io/5-hard-problems-in-vector-search-and-how-cassandra-solves-them/)
3. [Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs](https://arxiv.org/abs/1603.09320)
4. [FreshDiskANN: A Fast and Accurate Graph-Based ANN Index for Streaming Similarity Search]( https://arxiv.org/abs/2105.09613)

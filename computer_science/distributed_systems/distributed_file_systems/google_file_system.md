# Google File System

## Basic idea

Single-master, many-chunkserver design for huge sequential reads/writes over commodity hardware in one datacentre (2003). Trades strict POSIX semantics for simplicity, scalability, and automatic recovery from frequent disk failures.

## Key facts

- Chunk size: 64 MB; replication factor: 3 by default.
- Master holds metadata in memory: namespace, chunk locations, leases.
- Append-mostly workload; relaxed consistency for concurrent writers.
- Heartbeat + checksum + re-replication give automatic fault tolerance.

## Requirements in GFS

* Big
* Fast
* Sharding 
* Automatic recovery
* Single Data center
* Internal use
* big sequential reads and writes

## Architecture

100s of clients 1 Master Chunk Servers \(CS\) each with one or two disks The naster knows where the chunks are the master keeps a list of files and their chunk information

## Master Data

Two main tables that are important. One maps filenames to array of chunk handles another maps chunk handles to a list of chunk servers, version \#, primary chunk, lease expiration A log and checkpoint on disk


# distributed\_file\_systems

## Basic idea

File systems whose data and metadata are spread across many networked machines while still presenting a unified namespace and POSIX-ish semantics (or a deliberately weaker model). Hard because performance, consistency, and fault-tolerance pull against each other.

## Key facts

- Examples: GFS, HDFS, Ceph, Lustre, AFS, NFS.
- Replication factor $r$ tolerates $r-1$ node failures.
- Consistency models range from strict (linearisable) to close-to-open (NFS) to eventually consistent.


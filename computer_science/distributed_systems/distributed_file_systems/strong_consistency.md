# Strong Consistency

## Basic idea

After any write completes, every subsequent read on any replica returns that write (or a later one). Equivalent to the system *appearing* to be a single, ordered sequence of operations. Requires consensus across replicas.

## Key formulas

- Quorum condition: $R + W > N$ (read sees most recent committed write)
- Linearisability: every op takes effect atomically at some point between invocation and response.
- Consensus protocols (Paxos, Raft) implement this with $\lceil N/2 \rceil + 1$ acks.

## Consider the following case in a single server scenario

In a KV store given this transaction initially C1 Wx1 C2 Wx2

What should C3, C4 read? C3 Rx? C4 Rx?

Not enough to answer this question, but C3 and C4 should see the same value.

C3 Rxy C4 Rxy

## The above example becomes even harder under multiple server scenarios, without some underlying concensus, this becomes disastrous.


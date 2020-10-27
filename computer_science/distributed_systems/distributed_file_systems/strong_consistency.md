# Strong Consistency

## Consider the following case in a single server scenario

In a KV store given this transaction initially C1 Wx1 C2 Wx2

What should C3, C4 read? C3 Rx? C4 Rx?

Not enough to answer this question, but C3 and C4 should see the same value.

C3 Rxy C4 Rxy

## The above example becomes even harder under multiple server scenarios, without some underlying concensus, this becomes disastrous.


# Communication paradigms

## Basic idea

Three layers of communication abstraction: low-level IPC primitives, request-reply / RPC / RMI, and indirect (decoupled) communication such as pub/sub, message queues, and tuple spaces.

## Key facts

- Direct: tightly couples sender and receiver in identity and time.
- Indirect: space-uncoupled (sender doesn't know receiver) and/or time-uncoupled (parties needn't coexist).
- Examples: pub/sub, message queues, tuple spaces, group communication.

## Communication paradigms 
From low to high level:
  * Interprocess communication are the underlying primitives -- relatively low level
  * Remote invocation -- based on a two way exchange between communicating entities in a distributed system, e.g. request-reply protocols, RPC, RMI
  * Indirect communication
    * Space uncoupling -- senders do not need to know who they are sending to.
    * Time uncoupling -- senders and receivers do not need to exist at the same time.
  
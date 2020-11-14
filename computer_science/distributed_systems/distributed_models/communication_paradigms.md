## Communication paradigms 
From low to high level:
  * Interprocess communication are the underlying primitives -- relatively low level
  * Remote invocation -- based on a two way exchange between communicating entities in a distributed system, e.g. request-reply protocols, RPC, RMI
  * Indirect communication
    * Space uncoupling -- senders do not need to know who they are sending to.
    * Time uncoupling -- senders and receivers do not need to exist at the same time.
  
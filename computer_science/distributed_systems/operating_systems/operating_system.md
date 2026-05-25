# Operating System

## Basic idea

The OS layer that interacts with a network either as a participant (networked OS) or as something to be abstracted away (distributed OS). The distinction is *who* knows about the network: the user or the OS.

## Key facts

- Networked OS: hosts are autonomous; user explicitly invokes network ops.
- Distributed OS: location transparency — the OS schedules and migrates as needed.
- Real-world systems are mostly networked; true distributed OSes (Plan 9, Amoeba) remained research artefacts.

Networking versus Distributed OS

**Networked OS**

A networked operating system provides support for network operations. The users manage the networked applications and commands. Each host is autonomous.

**Distributed OS**

Tries to abstract the network from the user and thereby remove the need for the user to specify how the networking commands and operations should be undertaken.


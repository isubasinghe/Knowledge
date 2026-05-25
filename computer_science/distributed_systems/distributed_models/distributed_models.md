# Distributed Models

## Basic idea

Three layers of abstraction used to describe and reason about distributed systems: physical (hardware), architectural (components + patterns + middleware), and fundamental (non-functional properties such as reliability, security, performance).

## Key facts

- Synchronous: known bounds on execution time, message delay, and clock drift.
- Asynchronous: no bounds on any of the above — much weaker but matches the open Internet.
- Real systems are usually *partially* synchronous: bounds exist but are unknown or hold only eventually.

A **physical model** considers: underlying hardware elements

An **architectural** model considers:

* Architectural elements - components of the system that interact with each other. 
* Architectural paterns 
* Associated middleware solutions

**Fundemental models** define: The non functional aspects such as:

* Reliability
* Security
* Performance

## Variations of interaction models

Two simple models of distributed system interaction are:

* Synchronous system model - assumes known bounds on:
  * The time to execute
  * Message transmission delay
  * Local clock drift rate
* Asynchronous system model - assumes no bound on:
  * Process execution speed
  * Message transmission delays
  * Clock drift rates


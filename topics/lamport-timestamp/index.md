# Lamport timestamp

A Lamport timestamp, named after its inventor Leslie Lamport, is a mechanism used to provide a partial ordering of events in a distributed system. It is commonly used in databases, distributed systems, and network protocols.

In a distributed system, events can occur concurrently across multiple nodes, and there is no global clock that can be used to accurately order these events. Lamport timestamps address this problem by assigning a unique timestamp to each event based on a logical clock, which is a counter that is incremented each time an event occurs.

The Lamport timestamp is represented as an integer, and it consists of two parts: a timestamp value and an identifier for the process that generated the event. Each process maintains its own Lamport clock, which is used to generate timestamps for events that it generates. When a process sends a message to another process, it includes its Lamport timestamp in the message. When the receiving process receives the message, it updates its own Lamport clock to reflect the latest timestamp it has seen, and then assigns a new Lamport timestamp to any subsequent events it generates.

Lamport timestamps have two key properties: causality and consistency. Causality ensures that events that are causally related are ordered correctly, while consistency ensures that concurrent events are not ordered incorrectly. However, Lamport timestamps do not provide a global ordering of events, as events that are not causally related may still be ordered differently on different nodes.

Lamport clocks cannot tell us if a message was concurrent, and cannot be used to infer causality between events. Vector clocks are a more sophisticated variant which gives us more guarantees, including knowledge of concurrency & causal history, at the cost of overhead proportional to the number of nodes.

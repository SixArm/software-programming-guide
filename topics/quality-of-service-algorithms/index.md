# Quality of Service (QoS) algorithms

Quality of Service (QoS) algorithms and mechanisms are essential in telecommunications to  prioritize, manage, and control network traffic, allowing for better service delivery, especially in environments where multiple applications with different requirements share the same network infrastructure.

Some common ones:

* Traffic Shaping: Regulate the rate at which packets are transmitted.

* Prioritization: Give preferential treatment to specific types of traffic, such as voice or video, to ensure low latency and jitter.

* Queue Management Algorithms: Prioritize and manage packet queues. Common algorithms include Weighted Fair Queuing (WFQ), Stochastic Fairness Queuing (SFQ), and Random Early Detection (RED).

* Admission Control: Assess whether new traffic flows can be admitted into the network.

* Packet Classification and Marking: These techniques are used to classify incoming packets based on specific criteria, such as source or destination IP addresses, port numbers, or DSCP values.

* Congestion Avoidance: Monitor network conditions and adjust traffic behavior to prevent congestion. These include Transmission Control Protocol (TCP) congestion control algorithms, such as TCP Vegas and TCP Cubic.

* Bandwidth Reservation: Allocate a specific amount of network bandwidth to critical applications or services. For example, RSVP can be used to reserve bandwidth for multimedia applications.

* Scheduling Algorithms: Determine the order in which packets are transmitted from queues. Use algorithms like Weighted Round Robin and Priority Queuing.

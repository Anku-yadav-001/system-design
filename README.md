# system-design

## Scalability
it is a ability of a system to handle increasing amount of workload  or requests without any performace and cost issue.

it is a crutial to understand the scalability in system design because it directly impacts the systems ability to grow and adapt to changing requirements over time.

### types of scalability 
==> vertical - stand up
==> horizontal - stand out

vertical - increasing the capacity(BUY BIGGER MACHINE)
 - no load balancing required
 - single point of failure
 - inter process 
 - data consistency
 - scaling limit

horizontal - increasing the machines(BUY MORE MACHINE)
 - load balancing required
 - resielent
 - inter process communication
 - network call(RPC - remote procedural call)
 - data inconsistency
 - scales well

## Capacity estimation
capacity estimation in system design is a process to predicting and determining the maximum load that the machine can handle within the operation parameters.

analyzing various aspects
 - hardware capability 
 - software performance
 - network bandwidth
 - user behavior

factors that affects capacity estimation
 - hardware resources
 - software efficiency
 - workload
 - user behaviour
 - scalability 
 - performance metrics
 - failure scenarios

matrics for capacity estimation
 - daily active users(DAU)
 - queries per second(QPS)
 - storage requirement
 - error rates
 - response time
 - concurrency
 - peak load handling
 
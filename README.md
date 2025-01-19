# system-design

## Scalability
it is a ability of a system to handle increasing amount of workload or requests without any performace and cost issue.

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
 

## HTTP
 - hypertext transfer protocol
 - works on application layer 
 - connectionless == for each request it eastablish different connection - it not uses the same connection for other requests
 - stateless == it dont know the details about the client and server after the connection termination
 - port == 80
 - media independent - it can send any sort of data that the client and server can understand how to process the data 

## HTTPS
 - hyper text transfer protocol 
 - secure
 - it encrypt the sensitive data such as login credentials
 - it uses Transfer Layer Security(TLS) known as Secure Socket Layer(SSL)

## Indexing
 - indexing is used to optimize the performance of database by minimizing the number of disk accesses required when query is processed
 - it is a type of data structure used to locate and access the data from db

1. primary index - if the index is created on the basis of the primary key of the table then it is known as primary index.
2. dense index - it contains an index record for every search value  in the data file, it makes search faster.
3. sparse index 
4. cluster index   

SELECT * FROM table_name WHERE country="india" and gender="country" sort by city
SELECT * FROM table_name WHERE sort_id LIKE "india+gender%"

## databases uses
1. SQL 
    - stackoverflow
    - youtube
    - instagram
    - facebook
    - uber
    - airBnB

2. noSQL
    - netflix
    - amazon
    - google
    - twitter
    - linkdin

## Cassandra
 -  it is a open source no-sql database that stores and manages large amounts of data 
 - developed by facebook (2008)
 - inspired by amazon dynamodb
 - it used hybrid design between a tabular and key value store
 - data is organized in keyspace and tables

## Quroum 
 -  minimum number of replicates that must be respond to a read or write operation for that operation to be considered successfully.

 - quroum is calculated as `(replication factor+1)/2`
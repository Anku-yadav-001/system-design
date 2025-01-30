## Load Balancing
techinque used in distributed system extensively.
Load balancing is a technique used to distribute network traffic evenly across multiple servers.

- This helps to prevent any single server from becoming overloaded, which can lead to slow performance or even downtime. 

- Load balancing can also be used to improve the availability of a website or application by ensuring that there are always enough servers available to handle requests.

x/n - load
1/n - balance
n - number of servers
m1 - request ids
h - hash

request id(m) = 1 to m-1
hash request[h(r1)] = m1%n 

### How is load balancing implemented?
Load balancing can be implemented using various techinques and algorithms

- Round Robin
- IP Hash
-Least Response Time

`the problem is not actually load balancing, the problem is removing and adding the servers and because of that we are completly changing our local data`

## Consistent Hashing
Consistent hashing is a technique used in distributed systems to distribute data across a dynamic set of nodes (servers) in a way that minimizes the amount of data that needs to be moved when nodes are added or removed. This helps to maintain a balanced load and ensures that the system can scale efficiently.

## Sharding
Database sharding is a technique for horizontal scaling of databases, where the data is split across multiple database instances, or shards, to improve performance and reduce the impact of large amounts of data on a single database.

## Memcached
Memcached is a powerful tool used in system design to speed up web applications by storing data in memory. It works as a caching layer, reducing the time needed to access frequently requested information.

Memcached is a distributed memory caching system used to enhance the performance and scalability of web applications by reducing the load on databases. It stores frequently accessed data in memory, allowing for faster retrieval compared to traditional storage methods like disk-based databases. 
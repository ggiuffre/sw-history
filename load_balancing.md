# History of load balancing


## Round-robin DNS routing

For every DNS query, name servers return a list of IP addresses in a different order.

Problems that it solves:
* scalability: a single web server struggles to handle an increasing volume of requests

Open problems:
* DNS name servers don't know if an instance at an IP address is down
* web clients tend to cache DNS queries


## Load balancing

Traffic is handled by a reverse proxy that represents a cluster of web servers.
For each server, the proxy has knowledge of whether it's up or down.

Problems that it solves:
* scalability: a single web server struggles to handle an increasing volume of requests
* high availability: the failure of an individual server shouldn't bring down the service for any user
* zero-downtime deployments are difficult to do with just a single web server

Icing on the cake:
* can be done at different levels of the OSI stack (application, network or physical)
* can take care of TLS termination
* can protect against SYN flood attacks or DDoS attacks

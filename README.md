# Redis lab

In this example:

* KeyDB cluster is deployed using custom operator, since no decent operator
  is available for vanilla Redis and KeyDB supports operating in multi-master mode
* Redis Commander is deployed to inspect the contents of the KeyDB cluster

Tasks:

0. Adjust sandbox name `3nk45yqd6e` as necessary for your sandbox
1. Using kubectl forward 6379 TCP port of any of the pods to your local laptop
   and attempt to connect using Redis command line utilities

Questions:

* What could be other options for KeyDB cluster pod anti affinity topology key?
* Where/how can you figure out current cluster status?
* Which pod is the current primary?
* What are the options for monitoring the KeyDB cluster?
* What are the benefits and drawbacks of managing KeyDB clusters yourself
  versus using SaaS offering such as AWS RDS?
* How does https://crossplane.io/ fit in the picture?
* How large instances to consider? When is sharding applicable?
* When is data persistence applicable?
* What options are there to migrate legacy Redis deployment into KeyDB?

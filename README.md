# Redis lab

In this example:

* Since no decent operator is available for vanilla Redis,
  custom operator that sets up the cluster is used in this example
* Additionally KeyDB is used instead of Redis because it provider
* Redis Commander is deployed to inspect the contents of the cluster

Tasks:

0. Adjust username `laurivosandi` as necessary for deployment
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
* How large instances to consider?
* When is data persistence applicable?
* What options are there to migrate legacy Redis deployment into KeyDB?

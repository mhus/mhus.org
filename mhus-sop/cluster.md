
## SOP Cluster

### Overview

The cluster framework allows to survive in cluster environment. Functions like locking and caching over the cluster are implemented.

I need the framework to duplicate karaf servers in a docker swarm or kubernetes environment. Most services are not able to coexist multiple times or must not executed in multiple instances in the same time.

The main purpose of the framework is to block multiple executions of the same function (cron and timer jobs), work with caches (invalidation and distribution) and locking.

###

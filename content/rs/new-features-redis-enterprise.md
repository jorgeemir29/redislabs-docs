---
Title: What's new in Redis Enterprise Software 5.0?
description: $description
weight: $weight
alwaysopen: false
---
Below are detailed a few of the major features of this release of Redis
Enterprise Software along with bug fixes and patches.

Geo-Distributed Active-Active Conflict-free Replicated Databases (CRDB)
-----------------------------------------------------------------------

Developing globally distributed applications can be challenging, as
developers have to think about race conditions and complex combinations
of events under geo-failovers and cross-region write conflicts. CRDBs
simplify developing such applications by directly using built-in smarts
for handling conflicting writes based on the data type in use. Instead
of depending on just simplistic "last-writer-wins" type conflict
resolution, geo-distributed CRDBs combines techniques defined in CRDT
(conflict-free replicated data types) research with Redis types to
provide smart and automatic conflict resolution based on the data type's
intent.

For more information, go here. For information, go to [Developing with
CRDBs](/redis-enterprise-documentation/developing/crdbs/).

Redis Modules
-------------

Redis Modules enable you to extend the functionality of Redis Enterprise
Software. One can add new data types, capabilities, etc. to tailor the
cluster to a specific use case or need. Once installed, modules benefit
from the high performance, scalability, and high availability that Redis
Enterprise is known for.

### Redis Labs' Modules

There are three modules Redis Labs has developed and certified with
Redis Enterprise Software (RS). The modules are:

-   [RediSearch](/redis-enterprise-documentation/developing/redisearch/)
    -- This module turns RS into a supercharged distributed in-memory
    full-text indexing and search beast.
-   [ReJSON](/redis-enterprise-documentation/developing/rejson/) -- Now
    you have the convenience JSON as a built-in data type and easily
    able to address nested data via a path.
-   [ReBloom](/redis-enterprise-documentation/developing/modules/bloom-filters/)
    -- Enables RS to have a scalable bloom filter as a data type. Bloom
    filters are probabilistic data structures that do a very good job at
    quickly determining if something is contained within a set.

### Custom Modules

In addition, Redis Enterprise Software provides the ability to load and
use custom modules from [redismodules.com](http://redismodules.com/) or
of your own creation.

Support for Docker in Production
--------------------------------

Deploying and running your Redis Enterprise Software cluster on Docker
containers is now officially supported in production systems and
available to pull from Docker hub. With the official image, you can
easily and quickly deploy several containers to start running a scalable
and highly available cluster Redis Enterprise Software is famous for.

For more information go to [quick start with Redis Enterprise Software
on Docker.](/redis-enterprise-documentation/getting-started/docker/)

LDAP Integration
----------------

As part of our continued emphasis on security, administrative user
accounts in Redis Enterprise Software can now use either built-in
authentication or authenticate externally via LDAP with saslauthd. The
accounts can be used for administering resources on the cluster via
command line, Rest API, or Web UI.

For more information see [LDAP
Integration](/redis-enterprise-documentation/administering/security/ldap-integration/).


### Enterprise WAN Replication Additional Information

Each cluster in WAN topology has to have a unique `group-name` property for a proper handling of forwarded events.
 
Starting from 3.6, Enterprise WAN replication backups its WAN replication event queues to other nodes to prevent event loss in case of node failure scenarios.
Enterprise WAN replication's backup mechanism depends on the related data structures' backup operations. (WAN replication is only supported for Map and Cache)
That means, as far as you set a backup count for your data structure, wan replication events generated by this data structure is also replicated.
 
There is no additional configuration to enable/disable WAN replication event backups.

*Please refer to the [Enterprise WAN Replication Configuration section](#enterprise-wan-replication-configuration) for a full description of Hazelcast WAN Replication configuration.*




<img width="825" alt="image" src="https://github.com/user-attachments/assets/f4fbad65-2bfb-461c-840d-10afe39268e2" />


# Write-Heavy Workloads

- If you have a write-heavy workload, we strongly recommend a database that stores data in immutable files (e.g., Cassandra, ScyllaDB, and others that use LSM trees).2 These databases optimize write speed because:
  - Writes are sequential, which is faster in terms of disk I/O
  - Writes are performed immediately, without first worrying about reading or updating existing values (like databases that rely on B-trees do).
## However, if you opt for a write-optimized database, be prepared for higher storage requirements and the potential for slower reads.
- **NOTE: Write-optimized databases can improve read latency via internal caching


# Read-Heavy Workloads

Looking for
- Strong consistency
- Eventual consistency


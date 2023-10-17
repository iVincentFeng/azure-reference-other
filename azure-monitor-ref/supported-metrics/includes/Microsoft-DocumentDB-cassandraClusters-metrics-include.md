---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/02/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.DocumentDB/cassandraClusters, naam
---
  
  
|Metric|Name|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|cache capacity<p><p>Cache capacity (bytes). |`cassandra_cache_capacity` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|cache entries<p><p>Total number of cache entries. |`cassandra_cache_entries` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|cache hit rate<p><p>All time cache hit rate. |`cassandra_cache_hit_rate` |Percent |Average |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|cache hits<p><p>Number of cache hits. |`cassandra_cache_hits` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|cache miss latency average (microseconds)<p><p>Average cache miss latency (microseconds). |`cassandra_cache_miss_latency_histogram` |Count |Average |cassandra_datacenter, cassandra_node, quantile|PT1M |No|
|cache miss latency p99 (microseconds)<p><p>p99 latency of misses. |`cassandra_cache_miss_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|cache requests<p><p>Number of cache requests. |`cassandra_cache_requests` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|occupied cache size<p><p>Size of occupied cache (bytes). |`cassandra_cache_size` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, cache_name|PT1M |No|
|auth failure (deprecated)<p><p>Number of failed client authentication requests. |`cassandra_client_auth_failure` |Count |Total |cassandra_datacenter, cassandra_node|PT1M |No|
|auth failure (deprecated)<p><p>Number of failed client authentication requests. |`cassandra_client_auth_failure2` |Count |Total |cassandra_datacenter, cassandra_node|PT1M |No|
|client auth failure<p><p>Number of failed client authentication requests. |`cassandra_client_auth_failure3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|client auth success<p><p>Number of successful client authentication requests. |`cassandra_client_auth_success` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|connected native clients<p><p>Number of connected native clients. |`cassandra_client_connected_native_clients` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|condition not met<p><p>Cumulative number of transaction preconditions did not match current values. |`cassandra_client_request_condition_not_met` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|contention average<p><p>How many contended reads/writes were encountered in average. |`cassandra_client_request_contention_histogram` |Count |Average |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|contention p99<p><p>p99 how many contended writes were encountered. |`cassandra_client_request_contention_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|failures (deprecated)<p><p>Number of transaction failures encountered. |`cassandra_client_request_failures` |Count |Total |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|failures (deprecated)<p><p>Number of transaction failures encountered. |`cassandra_client_request_failures2` |Count |Total |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|client failures<p><p>Cumulative number of transaction failures encountered. |`cassandra_client_request_failures3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|client request latency average (microseconds)<p><p>Average client request latency (microseconds). |`cassandra_client_request_latency_histogram` |Count |Average |cassandra_datacenter, cassandra_node, quantile, request_type|PT1M |No|
|client request latency max (microseconds)<p><p>Maximum client request latency (microseconds). |`cassandra_client_request_latency_max` |Count |Maximum |ClusterResourceName, DataCenterResourceName, Address, request_type|PT1M |No|
|client request latency p99 (microseconds)<p><p>p99 client request latency (microseconds). |`cassandra_client_request_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|timeouts (deprecated)<p><p>Number of timeouts encountered. |`cassandra_client_request_timeouts` |Count |Total |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|timeouts (deprecated)<p><p>Number of timeouts encountered. |`cassandra_client_request_timeouts2` |Count |Total |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|client timeouts<p><p>Cumulative number of timeouts encountered in client requests. |`cassandra_client_request_timeouts3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|unfinished commit<p><p>Cumulative number of transactions that were committed on write. |`cassandra_client_request_unfinished_commit` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, request_type|PT1M |No|
|Commit latency on waiting average (microseconds).<p><p>Average time spent waiting on CL fsync (microseconds); for Periodic this is only occurs when the sync is lagging its sync interval. |`cassandra_commit_log_waiting_on_commit_latency_histogram` |Count |Average |cassandra_datacenter, cassandra_node, quantile|PT1M |No|
|prepared statements executed<p><p>Total number of prepared statements executed. |`cassandra_cql_prepared_statements_executed` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|regular statements executed<p><p>Total number of non prepared statements executed. |`cassandra_cql_regular_statements_executed` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|jvm gc count<p><p>Total number of collections that have occurred. |`cassandra_jvm_gc_count` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|jvm gc time<p><p>Approximate accumulated collection elapsed time. |`cassandra_jvm_gc_time` |MilliSeconds |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node|PT1M |No|
|all memtables live data size<p><p>Total amount of live data stored in the memtables (2i and pending flush memtables included) that resides off-heap, excluding any data structure overhead. |`cassandra_table_all_memtables_live_data_size` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|all memtables off heap size<p><p>Total amount of data stored in the memtables (2i and pending flush memtables included) that resides off-heap. |`cassandra_table_all_memtables_off_heap_size` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|bloom filter disk space used<p><p>Disk space used by bloom filter (bytes). |`cassandra_table_bloom_filter_disk_space_used` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|bloom filter false positives<p><p>Number of false positives on table's bloom filter. |`cassandra_table_bloom_filter_false_positives` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|bloom filter false ratio<p><p>False positive ratio of table's bloom filter. |`cassandra_table_bloom_filter_false_ratio` |Percent |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|bloom filter off-heap memory used<p><p>Off-heap memory used by bloom filter. |`cassandra_table_bloom_filter_off_heap_memory_used` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|bytes flushed<p><p>Total number of bytes flushed since server [re]start. |`cassandra_table_bytes_flushed` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas commit average (microseconds)<p><p>Average latency of paxos commit round. |`cassandra_table_cas_commit` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas commit p99 (microseconds)<p><p>p99 latency of paxos commit round. |`cassandra_table_cas_commit_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas prepare average (microseconds)<p><p>Average latency of paxos prepare round. |`cassandra_table_cas_prepare` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas prepare p99 (microseconds)<p><p>p99 latency of paxos prepare round. |`cassandra_table_cas_prepare_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas propose average (microseconds)<p><p>Average latency of paxos propose round. |`cassandra_table_cas_propose` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|cas propose p99 (microseconds)<p><p>p99 latency of paxos propose round. |`cassandra_table_cas_propose_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|col update time delta average<p><p>Average column update time delta on this table. |`cassandra_table_col_update_time_delta_histogram` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|col update time delta p99<p><p>p99 column update time delta on this table. |`cassandra_table_col_update_time_delta_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|compaction bytes written<p><p>Total number of bytes written by compaction since server [re]start. |`cassandra_table_compaction_bytes_written` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|compression metadata off-heap memory used<p><p>Off-heap memory used by compression metadata. |`cassandra_table_compression_metadata_off_heap_memory_used` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|compression ratio<p><p>Current compression ratio for all SSTables. |`cassandra_table_compression_ratio` |Percent |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|coordinator read latency average (microseconds)<p><p>Average coordinator read latency for this table. |`cassandra_table_coordinator_read_latency` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|coordinator read latency p99 (microseconds)<p><p>p99 coordinator read latency for this table. |`cassandra_table_coordinator_read_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|coordinator scan latency average (microseconds)<p><p>Average coordinator range scan latency for this table. |`cassandra_table_coordinator_scan_latency` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|coordinator scan latency p99 (microseconds)<p><p>p99 coordinator range scan latency for this table. |`cassandra_table_coordinator_scan_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|dropped mutations (deprecated)<p><p>Number of dropped mutations on this table. |`cassandra_table_dropped_mutations` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|dropped mutations (deprecated)<p><p>Number of dropped mutations on this table. |`cassandra_table_dropped_mutations2` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|dropped mutations<p><p>Total number of dropped mutations on this table. |`cassandra_table_dropped_mutations3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|estimated column count average<p><p>Estimated number of columns in average. |`cassandra_table_estimated_column_count_histogram` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|estimated column count p99<p><p>p99 estimated number of columns. |`cassandra_table_estimated_column_count_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|estimated partition count<p><p>Approximate number of keys in table. |`cassandra_table_estimated_partition_count` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|estimated partition size average<p><p>Estimated partition size in average. |`cassandra_table_estimated_partition_size_histogram` |Bytes |Average |cassandra_datacenter, cassandra_node, quantile, table, keyspace|PT1M |No|
|estimated partition size p99<p><p>p99 estimated partition size (bytes). |`cassandra_table_estimated_partition_size_histogram_p99` |Bytes |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|index summary off-heap memory used<p><p>Off-heap memory used by index summary. |`cassandra_table_index_summary_off_heap_memory_used` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|key cache hit rate<p><p>Key cache hit rate for this table. |`cassandra_table_key_cache_hit_rate` |Percent |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|live disk space used<p><p>Disk space used by SSTables belonging to this table (bytes). |`cassandra_table_live_disk_space_used` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|live scanned average<p><p>Average live cells scanned in queries on this table. |`cassandra_table_live_scanned_histogram` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|live scanned p99<p><p>p99 live cells scanned in queries on this table. |`cassandra_table_live_scanned_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|live sstable count<p><p>Number of SSTables on disk for this table. |`cassandra_table_live_sstable_count` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|max partition size<p><p>Size of the largest compacted partition (bytes). |`cassandra_table_max_partition_size` |Bytes |Maximum |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|mean partition size<p><p>Size of the average compacted partition (bytes). |`cassandra_table_mean_partition_size` |Bytes |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|memtable columns count<p><p>Total number of columns present in the memtable. |`cassandra_table_memtable_columns_count` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|memtable off heap size<p><p>Total amount of data stored in the memtable that resides off-heap, including column related overhead and partitions overwritten. |`cassandra_table_memtable_off_heap_size` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|memtable on heap size<p><p>Total amount of data stored in the memtable that resides on-heap, including column related overhead and partitions overwritten. |`cassandra_table_memtable_on_heap_size` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|memtable switch count<p><p>Number of times flush has resulted in the memtable being switched out. |`cassandra_table_memtable_switch_count` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|min partition size<p><p>Size of the smallest compacted partition (bytes). |`cassandra_table_min_partition_size` |Bytes |Minimum |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending compactions (deprecated)<p><p>Estimate of number of pending compactions for this table. |`cassandra_table_pending_compactions` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending compactions (deprecated)<p><p>Estimate of number of pending compactions for this table. |`cassandra_table_pending_compactions2` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending compactions<p><p>Estimate of number of pending compactions for this table. |`cassandra_table_pending_compactions3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending flushes (deprecated)<p><p>Estimated number of flush tasks pending for this table. |`cassandra_table_pending_flushes` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending flushes (deprecated)<p><p>Estimated number of flush tasks pending for this table. |`cassandra_table_pending_flushes2` |Count |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|pending flushes<p><p>Estimated number of flush tasks pending for this table. |`cassandra_table_pending_flushes3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|percent repaired<p><p>Percent of table data that is repaired on disk. |`cassandra_table_percent_repaired` |Percent |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|range latency average (microseconds)<p><p>Average local range scan latency for this table. |`cassandra_table_range_latency` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|range latency p99 (microseconds)<p><p>p99 local range scan latency for this table. |`cassandra_table_range_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|read latency average (microseconds)<p><p>Average local read latency for this table. |`cassandra_table_read_latency` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|read latency p99 (microseconds)<p><p>p99 local read latency for this table. |`cassandra_table_read_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|row cache hit<p><p>Number of table row cache hits. |`cassandra_table_row_cache_hit` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|row cache hit out of range<p><p>Number of table row cache hits that do not satisfy the query filter, thus went to disk. |`cassandra_table_row_cache_hit_out_of_range` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|row cache miss<p><p>Number of table row cache misses. |`cassandra_table_row_cache_miss` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|speculative retries<p><p>Number of times speculative retries were sent for this table. |`cassandra_table_speculative_retries` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|sstables per read average<p><p>Average number of sstable data files accessed per single partition read. SSTables skipped due to Bloom Filters, min-max key or partition index lookup are not taken into account. |`cassandra_table_sstables_per_read_histogram` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|sstables per read p99<p><p>p99 number of sstable data files accessed per single partition read. SSTables skipped due to Bloom Filters, min-max key or partition index lookup are not taken into account. |`cassandra_table_sstables_per_read_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|tombstone scanned average<p><p>Average tombstones scanned in queries on this table. |`cassandra_table_tombstone_scanned_histogram` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|tombstone scanned p99<p><p>p99 tombstones scanned in queries on this table. |`cassandra_table_tombstone_scanned_histogram_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|total disk space used (deprecated)<p><p>Total disk space used by SSTables belonging to this table, including obsolete ones waiting to be GC'd. |`cassandra_table_total_disk_space_used` |Bytes |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M, PT5M, PT15M, PT30M, PT1H, PT6H, PT12H, P1D |No|
|total disk space used (deprecated)<p><p>Total disk space used by SSTables belonging to this table, including obsolete ones waiting to be GC'd. |`cassandra_table_total_disk_space_used2` |Bytes |Total |cassandra_datacenter, cassandra_node, table, keyspace|PT1M, PT5M, PT15M, PT30M, PT1H, PT6H, PT12H, P1D |No|
|total disk space used<p><p>Total disk space used by SSTables belonging to this table, including obsolete ones waiting to be GC'd. |`cassandra_table_total_disk_space_used3` |Bytes |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|view lock acquire time average<p><p>Average time taken acquiring a partition lock for materialized view updates on this table. |`cassandra_table_view_lock_acquire_time` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|view lock acquire time p99<p><p>p99 time taken acquiring a partition lock for materialized view updates on this table. |`cassandra_table_view_lock_acquire_time_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|view read time average<p><p>Average time taken during the local read of a materialized view update. |`cassandra_table_view_read_time` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|view read time p99<p><p>p99 time taken during the local read of a materialized view update. |`cassandra_table_view_read_time_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|waiting on free memtable space average<p><p>Average time spent waiting for free memtable space, either on- or off-heap. |`cassandra_table_waiting_on_free_memtable_space` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|waiting on free memtable space p99<p><p>p99 time spent waiting for free memtable space, either on- or off-heap. |`cassandra_table_waiting_on_free_memtable_space_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|write latency average (microseconds)<p><p>Average local write latency for this table. |`cassandra_table_write_latency` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|write latency p99 (microseconds)<p><p>p99 local write latency for this table. |`cassandra_table_write_latency_p99` |Count |Average |cassandra_datacenter, cassandra_node, table, keyspace|PT1M |No|
|active tasks<p><p>Number of tasks being actively worked on by this pool. |`cassandra_thread_pools_active_tasks` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|currently blocked tasks (deprecated)<p><p>Number of tasks that are currently blocked due to queue saturation but on retry will become unblocked. |`cassandra_thread_pools_currently_blocked_tasks` |Count |Total |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|currently blocked tasks (deprecated)<p><p>Number of tasks that are currently blocked due to queue saturation but on retry will become unblocked. |`cassandra_thread_pools_currently_blocked_tasks2` |Count |Total |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|currently blocked tasks<p><p>Number of tasks that are currently blocked due to queue saturation but on retry will become unblocked. |`cassandra_thread_pools_currently_blocked_tasks3` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|max pool size<p><p>Maximum number of threads in this pool. |`cassandra_thread_pools_max_pool_size` |Count |Maximum |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|pending tasks<p><p>Number of queued tasks queued up on this pool. |`cassandra_thread_pools_pending_tasks` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|total blocked tasks<p><p>Total number of tasks that were blocked due to queue saturation. |`cassandra_thread_pools_total_blocked_tasks` |Count |Average, Minimum, Maximum, Count |cassandra_datacenter, cassandra_node, pool_name, pool_type|PT1M |No|
|CPU usage active<p><p>CPU usage (active). |`cpu` |Percent |Average |ClusterResourceName, DataCenterResourceName, Address, Kind, CPU|PT1M |Yes|
|disk utilization<p><p>Disk utilization rate. |`disk_utilization` |Percent |Average |ClusterResourceName, DataCenterResourceName, Address|PT1M |Yes|
|disk I/O merged reads<p><p>Cumulative disk I/O merged reads. |`diskio_merged_reads` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O merged writes<p><p>Cumulative disk I/O merged writes. |`diskio_merged_writes` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O read bytes<p><p>Cumulative disk I/O read bytes. |`diskio_read_bytes` |Bytes |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O read time (milliseconds)<p><p>Cumulative disk I/O read time (milliseconds). |`diskio_read_time` |MilliSeconds |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O read counts<p><p>Cumulative disk I/O read counts. |`diskio_reads` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O write bytes<p><p>Cumulative disk I/O write bytes. |`diskio_write_bytes` |Bytes |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O write time (milliseconds)<p><p>Cumulative disk I/O write time (milliseconds). |`diskio_write_time` |MilliSeconds |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|disk I/O write counts<p><p>Cumulative disk I/O write counts. |`diskio_writes` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|network received bytes<p><p>Cumulative network received bytes. |`ethtool_rx_bytes` |Bytes |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|network received packets<p><p>Cumulative network received packets. |`ethtool_rx_packets` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|network transmitted bytes<p><p>Cumulative network transmitted bytes. |`ethtool_tx_bytes` |Bytes |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|network transmitted packets<p><p>Cumulative network transmitted packets. |`ethtool_tx_packets` |Count |Average, Minimum, Maximum, Count |ClusterResourceName, DataCenterResourceName, Address, Kind|PT1M |No|
|memory utilization<p><p>Memory utilization rate. |`percent_mem` |Percent |Average |ClusterResourceName, DataCenterResourceName, Address|PT1M |Yes|
cc_library(
  name = 'rocksdb',
  export_incs = './include',
  incs = [
    '.',
    './include',
  ],
  defs = [
    'OS_LINUX',
    'ROCKSDB_ATOMIC_PRESENT',
    'ROCKSDB_PLATFORM_POSIX',
    'SNAPPY',
    'ZLIB',
  ],
  extra_cppflags = [
    '-Wno-float-equal',
    '-Wno-non-virtual-dtor',
    '-Wno-return-type',
    '-Wno-vla',
  ],
  srcs = [
    'db/builder.cc',
    'db/c.cc',
    'db/column_family.cc',
    'db/compaction.cc',
    'db/compaction_picker.cc',
    'db/db_filesnapshot.cc',
    'db/dbformat.cc',
    'db/db_impl.cc',
    'db/db_impl_debug.cc',
    'db/db_impl_readonly.cc',
    'db/db_iter.cc',
    'db/file_indexer.cc',
    'db/filename.cc',
    'db/forward_iterator.cc',
    'db/internal_stats.cc',
    'db/log_reader.cc',
    'db/log_writer.cc',
    'db/memtable.cc',
    'db/memtable_list.cc',
    'db/merge_helper.cc',
    'db/merge_operator.cc',
    'db/repair.cc',
    'db/table_cache.cc',
    'db/table_properties_collector.cc',
    'db/tailing_iter.cc',
    'db/transaction_log_impl.cc',
    'db/version_edit.cc',
    'db/version_set.cc',
    'db/write_batch.cc',
    'helpers/memenv/memenv.cc',
    'port/port_posix.cc',
    'port/stack_trace.cc',
    'table/adaptive_table_factory.cc',
    'table/block_based_table_builder.cc',
    'table/block_based_table_factory.cc',
    'table/block_based_table_reader.cc',
    'table/block_builder.cc',
    'table/block.cc',
    'table/block_hash_index.cc',
    'table/block_prefix_index.cc',
    'table/bloom_block.cc',
    'table/cuckoo_table_builder.cc',
    'table/cuckoo_table_reader.cc',
    'table/filter_block.cc',
    'table/flush_block_policy.cc',
    'table/format.cc',
    'table/iterator.cc',
    'table/merger.cc',
    'table/meta_blocks.cc',
    'table/plain_table_builder.cc',
    'table/plain_table_factory.cc',
    'table/plain_table_index.cc',
    'table/plain_table_key_coding.cc',
    'table/plain_table_reader.cc',
    'table/table_properties.cc',
    'table/two_level_iterator.cc',
    'util/arena.cc',
    'util/auto_roll_logger.cc',
    'util/blob_store.cc',
    'util/bloom.cc',
    'util/build_version.cc',
    'util/cache.cc',
    'util/coding.cc',
    'util/comparator.cc',
    'util/crc32c.cc',
    'util/dynamic_bloom.cc',
    'util/env.cc',
    'util/env_hdfs.cc',
    'util/env_posix.cc',
    'util/filter_policy.cc',
    'util/hash.cc',
    'util/hash_cuckoo_rep.cc',
    'util/hash_linklist_rep.cc',
    'util/hash_skiplist_rep.cc',
    'util/histogram.cc',
    'util/iostats_context.cc',
    'util/ldb_cmd.cc',
    'util/ldb_tool.cc',
    'util/log_buffer.cc',
    'util/logging.cc',
    'util/murmurhash.cc',
    'util/options_builder.cc',
    'util/options.cc',
    'util/perf_context.cc',
    'util/rate_limiter.cc',
    'util/skiplistrep.cc',
    'util/slice.cc',
    'util/statistics.cc',
    'util/status.cc',
    'util/string_util.cc',
    'util/sync_point.cc',
    'util/testharness.cc',
    'util/testutil.cc',
    'util/thread_local.cc',
    'util/vectorrep.cc',
    'util/xxhash.cc',
    'utilities/backupable/backupable_db.cc',
    'utilities/document/document_db.cc',
    'utilities/document/json_document.cc',
    'utilities/geodb/geodb_impl.cc',
    'utilities/merge_operators/put.cc',
    'utilities/merge_operators/uint64add.cc',
    'utilities/redis/redis_lists.cc',
    'utilities/spatialdb/spatial_db.cc',
    'utilities/ttl/db_ttl_impl.cc',
  ],
  deps = [
    '#pthread',
    '#rt',
    '//snappy:snappy',
    '//thirdparty/gflags:gflags',
    '//zlib:zlib',
  ],
)

cc_binary(
  name = 'unity',
  incs = [
    '.',
    './include',
  ],
  defs = [
    'OS_LINUX',
    'ROCKSDB_ATOMIC_PRESENT',
    'ROCKSDB_PLATFORM_POSIX',
    'SNAPPY',
    'ZLIB',
  ],
  extra_cppflags = [
    '-Wno-float-equal',
    '-Wno-non-virtual-dtor',
    '-Wno-return-type',
    '-Wno-vla',
  ],
  srcs = 'unity.cc',
  deps = [
    '#pthread',
    '#rt',
    '//snappy:snappy',
    '//thirdparty/gflags:gflags',
    '//zlib:zlib',
  ],
)

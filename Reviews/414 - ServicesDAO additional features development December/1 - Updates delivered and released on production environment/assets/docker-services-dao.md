```
yusuf@ubuntu:~/crdao/ServicesDAO$ docker compose up
[+] Running 9/0
 ⠿ Container servicesdao-dao_logsdb-1               Recreated              0.0s
 ⠿ Container dao_rabbitmq                           Recreated              0.0s
 ⠿ Container servicesdao-dao_db-1                   Recreated              0.0s
 ⠿ Container servicesdao-dao_dbservice-1            Recreated              0.0s
 ⠿ Container servicesdao-dao_apigateway-1           Recreated              0.0s
 ⠿ Container servicesdao-dao_webportal-1            Recreated              0.0s
 ⠿ Container servicesdao-dao_notificationservice-1  Recreated              0.0s
 ⠿ Container servicesdao-dao_logservice-1           Recreated              0.0s
 ⠿ Container servicesdao-dao_identityservice-1      Recreated              0.0s
Attaching to dao_rabbitmq, servicesdao-dao_apigateway-1, servicesdao-dao_db-1, servicesdao-dao_dbservice-1, servicesdao-dao_identityservice-1, servicesdao-dao_logsdb-1, servicesdao-dao_logservice-1, servicesdao-dao_notificationservice-1, servicesdao-dao_webportal-1
servicesdao-dao_logsdb-1               | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao-dao_logsdb-1               | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
servicesdao-dao_db-1                   | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao-dao_logsdb-1               | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao-dao_db-1                   | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
servicesdao-dao_db-1                   | 2022-04-24 10:29:50+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.37-1debian10 started.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.131322Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.132420Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 1 ...
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133959Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133979Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133981Z 0 [Note] InnoDB: Uses event mutexes
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133982Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133983Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.133984Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.134096Z 0 [Note] InnoDB: Number of pools: 1
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.134244Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.135245Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.138959Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.140385Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.154190Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.168490Z 0 [Note] InnoDB: Log scan progressed past the checkpoint lsn 12690972
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.168514Z 0 [Note] InnoDB: Doing recovery: scanned up to log sequence number 12690981
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.168518Z 0 [Note] InnoDB: Database was not shutdown normally!
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.168519Z 0 [Note] InnoDB: Starting crash recovery.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.177387Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.178326Z 0 [Note] mysqld (mysqld 5.7.37) starting as process 1 ...
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179857Z 0 [Note] InnoDB: PUNCH HOLE support available
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179865Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179867Z 0 [Note] InnoDB: Uses event mutexes
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179868Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179869Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179870Z 0 [Note] InnoDB: Using Linux native AIO
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.179974Z 0 [Note] InnoDB: Number of pools: 1
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.180030Z 0 [Note] InnoDB: Using CPU crc32 instructions
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.181386Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.185348Z 0 [Note] InnoDB: Completed initialization of buffer pool
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.186614Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.198564Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.205216Z 0 [Note] InnoDB: Removed temporary tablespace data file: "ibtmp1"
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.205233Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.205256Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.216115Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.216473Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.216488Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.216854Z 0 [Note] InnoDB: Waiting for purge to start
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.267089Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 14410429
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.267320Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.267323Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.268083Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:29:51
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272371Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272390Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272393Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272394Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272692Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.272728Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.273012Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.273031Z 0 [Note] IPv6 is available.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.273036Z 0 [Note]   - '::' resolves to '::';
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.273045Z 0 [Note] Server socket created on IP: '::'.
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.274241Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.277552Z 0 [Note] InnoDB: Removed temporary tablespace data file: "ibtmp1"
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.277572Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.277594Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.282075Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao-dao_db-1                   | 2022-04-24T10:29:51.282382Z 0 [Note] mysqld: ready for connections.
servicesdao-dao_db-1                   | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.287843Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.288225Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.288244Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.288486Z 0 [Note] InnoDB: Waiting for purge to start
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.338970Z 0 [Note] InnoDB: 5.7.37 started; log sequence number 12690981
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.339272Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.339281Z 0 [Note] Plugin 'FEDERATED' is disabled.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343211Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343236Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343240Z 0 [Warning] A deprecated TLS version TLSv1 is enabled. Please use TLSv1.2 or higher.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343241Z 0 [Warning] A deprecated TLS version TLSv1.1 is enabled. Please use TLSv1.2 or higher.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343684Z 0 [Warning] CA certificate ca.pem is self signed.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.343816Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.344385Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.344420Z 0 [Note] IPv6 is available.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.344426Z 0 [Note]   - '::' resolves to '::';
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.344435Z 0 [Note] Server socket created on IP: '::'.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.345964Z 0 [Note] InnoDB: Buffer pool(s) load completed at 220424 10:29:51
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.345972Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.352005Z 0 [Note] Event Scheduler: Loaded 0 events
servicesdao-dao_logsdb-1               | 2022-04-24T10:29:51.352268Z 0 [Note] mysqld: ready for connections.
servicesdao-dao_logsdb-1               | Version: '5.7.37'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
dao_rabbitmq                           | 2022-04-24 10:29:53.427764+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:53.441506+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:53.441543+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:53.441559+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:53.441567+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:53.441628+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:53.441637+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:53.441645+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:53.786925+00:00 [noti] <0.44.0> Application syslog exited with reason: stopped
dao_rabbitmq                           | 2022-04-24 10:29:53.787002+00:00 [noti] <0.228.0> Logging: switching to configured handler(s); following messages may not be visible in this log output
dao_rabbitmq                           | 2022-04-24 10:29:53.802558+00:00 [notice] <0.228.0> Logging: configured log handlers are now ACTIVE
dao_rabbitmq                           | 2022-04-24 10:29:53.991183+00:00 [info] <0.228.0> ra: starting system quorum_queues
dao_rabbitmq                           | 2022-04-24 10:29:53.991252+00:00 [info] <0.228.0> starting Ra system: quorum_queues in directory: /var/lib/rabbitmq/mnesia/rabbit@1d52ae8b94cd/quorum/rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:54.044758+00:00 [info] <0.264.0> ra system 'quorum_queues' running pre init for 0 registered servers
dao_rabbitmq                           | 2022-04-24 10:29:54.054329+00:00 [info] <0.265.0> ra: meta data store initialised for system quorum_queues. 0 record(s) recovered
dao_rabbitmq                           | 2022-04-24 10:29:54.066047+00:00 [notice] <0.270.0> WAL: ra_log_wal init, open tbls: ra_log_open_mem_tables, closed tbls: ra_log_closed_mem_tables
dao_rabbitmq                           | 2022-04-24 10:29:54.071605+00:00 [info] <0.228.0> ra: starting system coordination
dao_rabbitmq                           | 2022-04-24 10:29:54.071626+00:00 [info] <0.228.0> starting Ra system: coordination in directory: /var/lib/rabbitmq/mnesia/rabbit@1d52ae8b94cd/coordination/rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:54.072891+00:00 [info] <0.277.0> ra system 'coordination' running pre init for 0 registered servers
dao_rabbitmq                           | 2022-04-24 10:29:54.073672+00:00 [info] <0.278.0> ra: meta data store initialised for system coordination. 0 record(s) recovered
dao_rabbitmq                           | 2022-04-24 10:29:54.073816+00:00 [notice] <0.283.0> WAL: ra_coordination_log_wal init, open tbls: ra_coordination_log_open_mem_tables, closed tbls: ra_coordination_log_closed_mem_tables
dao_rabbitmq                           | 2022-04-24 10:29:54.075647+00:00 [info] <0.228.0> 
dao_rabbitmq                           | 2022-04-24 10:29:54.075647+00:00 [info] <0.228.0>  Starting RabbitMQ 3.9.15 on Erlang 24.3.3 [jit]
dao_rabbitmq                           | 2022-04-24 10:29:54.075647+00:00 [info] <0.228.0>  Copyright (c) 2007-2022 VMware, Inc. or its affiliates.
dao_rabbitmq                           | 2022-04-24 10:29:54.075647+00:00 [info] <0.228.0>  Licensed under the MPL 2.0. Website: https://rabbitmq.com
dao_rabbitmq                           | 
dao_rabbitmq                           |   ##  ##      RabbitMQ 3.9.15
dao_rabbitmq                           |   ##  ##
dao_rabbitmq                           |   ##########  Copyright (c) 2007-2022 VMware, Inc. or its affiliates.
dao_rabbitmq                           |   ######  ##
dao_rabbitmq                           |   ##########  Licensed under the MPL 2.0. Website: https://rabbitmq.com
dao_rabbitmq                           | 
dao_rabbitmq                           |   Erlang:      24.3.3 [jit]
dao_rabbitmq                           |   TLS Library: OpenSSL - OpenSSL 1.1.1n  15 Mar 2022
dao_rabbitmq                           | 
dao_rabbitmq                           |   Doc guides:  https://rabbitmq.com/documentation.html
dao_rabbitmq                           |   Support:     https://rabbitmq.com/contact.html
dao_rabbitmq                           |   Tutorials:   https://rabbitmq.com/getstarted.html
dao_rabbitmq                           |   Monitoring:  https://rabbitmq.com/monitoring.html
dao_rabbitmq                           | 
dao_rabbitmq                           |   Logs: /var/log/rabbitmq/rabbit@1d52ae8b94cd_upgrade.log
dao_rabbitmq                           |         <stdout>
dao_rabbitmq                           | 
dao_rabbitmq                           |   Config file(s): /etc/rabbitmq/conf.d/10-defaults.conf
dao_rabbitmq                           | 
dao_rabbitmq                           |   Starting broker...2022-04-24 10:29:54.076897+00:00 [info] <0.228.0> 
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  node           : rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  home dir       : /var/lib/rabbitmq
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  config file(s) : /etc/rabbitmq/conf.d/10-defaults.conf
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  cookie hash    : ednl3pYMjiYt8lq7p/QRCA==
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  log(s)         : /var/log/rabbitmq/rabbit@1d52ae8b94cd_upgrade.log
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>                 : <stdout>
dao_rabbitmq                           | 2022-04-24 10:29:54.076897+00:00 [info] <0.228.0>  database dir   : /var/lib/rabbitmq/mnesia/rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:54.255237+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:54.255274+00:00 [info] <0.228.0> Feature flags:   [ ] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:54.255292+00:00 [info] <0.228.0> Feature flags:   [ ] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:54.255315+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:54.255325+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:54.255332+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:54.255339+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:54.255380+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:54.255392+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:54.255410+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.591964+00:00 [info] <0.228.0> Running boot step pre_boot defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.592022+00:00 [info] <0.228.0> Running boot step rabbit_global_counters defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.592155+00:00 [info] <0.228.0> Running boot step rabbit_osiris_metrics defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.592248+00:00 [info] <0.228.0> Running boot step rabbit_core_metrics defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.592671+00:00 [info] <0.228.0> Running boot step rabbit_alarm defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.596141+00:00 [info] <0.295.0> Memory high watermark set to 3166 MiB (3319921049 bytes) of 7915 MiB (8299802624 bytes) total
dao_rabbitmq                           | 2022-04-24 10:29:56.599471+00:00 [info] <0.297.0> Enabling free disk space monitoring
dao_rabbitmq                           | 2022-04-24 10:29:56.599495+00:00 [info] <0.297.0> Disk free limit set to 50MB
dao_rabbitmq                           | 2022-04-24 10:29:56.601996+00:00 [info] <0.228.0> Running boot step code_server_cache defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.602050+00:00 [info] <0.228.0> Running boot step file_handle_cache defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.602348+00:00 [info] <0.302.0> Limiting to approx 1048479 file handles (943629 sockets)
dao_rabbitmq                           | 2022-04-24 10:29:56.602471+00:00 [info] <0.303.0> FHC read buffering: OFF
dao_rabbitmq                           | 2022-04-24 10:29:56.602493+00:00 [info] <0.303.0> FHC write buffering: ON
dao_rabbitmq                           | 2022-04-24 10:29:56.603024+00:00 [info] <0.228.0> Running boot step worker_pool defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.603067+00:00 [info] <0.285.0> Will use 8 processes for default worker pool
dao_rabbitmq                           | 2022-04-24 10:29:56.603085+00:00 [info] <0.285.0> Starting worker pool 'worker_pool' with 8 processes in it
dao_rabbitmq                           | 2022-04-24 10:29:56.603572+00:00 [info] <0.228.0> Running boot step database defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.603834+00:00 [info] <0.228.0> Node database directory at /var/lib/rabbitmq/mnesia/rabbit@1d52ae8b94cd is empty. Assuming we need to join an existing cluster or initialise from scratch...
dao_rabbitmq                           | 2022-04-24 10:29:56.603871+00:00 [info] <0.228.0> Configured peer discovery backend: rabbit_peer_discovery_classic_config
dao_rabbitmq                           | 2022-04-24 10:29:56.603889+00:00 [info] <0.228.0> Will try to lock with peer discovery backend rabbit_peer_discovery_classic_config
dao_rabbitmq                           | 2022-04-24 10:29:56.603940+00:00 [info] <0.228.0> All discovered existing cluster peers:
dao_rabbitmq                           | 2022-04-24 10:29:56.603955+00:00 [info] <0.228.0> Discovered no peer nodes to cluster with. Some discovery backends can filter nodes out based on a readiness criteria. Enabling debug logging might help troubleshoot.
dao_rabbitmq                           | 2022-04-24 10:29:56.605119+00:00 [notice] <0.44.0> Application mnesia exited with reason: stopped
dao_rabbitmq                           | 2022-04-24 10:29:56.666187+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.666311+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.672177+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.672228+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.672252+00:00 [info] <0.228.0> Feature flag `drop_unroutable_metric`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.672285+00:00 [info] <0.228.0> Feature flag `drop_unroutable_metric`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.672851+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.672886+00:00 [info] <0.228.0> Feature flags:   [~] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.672900+00:00 [info] <0.228.0> Feature flags:   [ ] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.672910+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.672918+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.672925+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.672932+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.672951+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.672969+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.672976+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.677561+00:00 [info] <0.228.0> Feature flag `drop_unroutable_metric`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.678571+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.678598+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.678625+00:00 [info] <0.228.0> Feature flags:   [ ] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.678637+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.678685+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.678701+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.678711+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.678758+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.678783+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.678809+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.683090+00:00 [info] <0.228.0> Feature flag `empty_basic_get_metric`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.683127+00:00 [info] <0.228.0> Feature flag `empty_basic_get_metric`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.683800+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.683835+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.683855+00:00 [info] <0.228.0> Feature flags:   [~] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.683865+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.683873+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.683881+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.683887+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.683984+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.683999+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.684040+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.688871+00:00 [info] <0.228.0> Feature flag `empty_basic_get_metric`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.691488+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.691530+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.691551+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.691561+00:00 [info] <0.228.0> Feature flags:   [ ] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.691572+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.691594+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.691647+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.691661+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.691679+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.691701+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.696024+00:00 [info] <0.228.0> Feature flag `implicit_default_bindings`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.696080+00:00 [info] <0.228.0> Feature flag `implicit_default_bindings`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.696592+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.696625+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.696645+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.696678+00:00 [info] <0.228.0> Feature flags:   [~] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.696697+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.696708+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.696715+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.696736+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.696743+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.696837+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.700982+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 0 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.701057+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.701090+00:00 [info] <0.228.0> Feature flag `implicit_default_bindings`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.703045+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.703085+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.703106+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.703114+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.703123+00:00 [info] <0.228.0> Feature flags:   [ ] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.703131+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.703138+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.703145+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.703153+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.703171+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.707113+00:00 [info] <0.228.0> Feature flag `maintenance_mode_status`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.707156+00:00 [info] <0.228.0> Feature flag `maintenance_mode_status`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.707704+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.707729+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.707755+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.707794+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.707822+00:00 [info] <0.228.0> Feature flags:   [~] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.707840+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.707851+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.707922+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.707935+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.707967+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.712989+00:00 [info] <0.228.0> Creating table rabbit_node_maintenance_states for feature flag `maintenance_mode_status`
dao_rabbitmq                           | 2022-04-24 10:29:56.716340+00:00 [info] <0.228.0> Feature flag `maintenance_mode_status`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.718714+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.718756+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.718778+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.718787+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.718797+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.718804+00:00 [info] <0.228.0> Feature flags:   [ ] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.718811+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.718818+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.718826+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.718845+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.723419+00:00 [info] <0.228.0> Feature flag `quorum_queue`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.723466+00:00 [info] <0.228.0> Feature flag `quorum_queue`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.724092+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.724127+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.724148+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.724160+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.724168+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.724176+00:00 [info] <0.228.0> Feature flags:   [~] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.724256+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.724283+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.724294+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.724325+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.729258+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.729333+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.729348+00:00 [info] <0.228.0> Feature flag `quorum_queue`:   migrating Mnesia table rabbit_queue...
dao_rabbitmq                           | 2022-04-24 10:29:56.739162+00:00 [info] <0.228.0> Feature flag `quorum_queue`:   migrating Mnesia table rabbit_durable_queue...
dao_rabbitmq                           | 2022-04-24 10:29:56.748721+00:00 [info] <0.228.0> Feature flag `quorum_queue`:   Mnesia tables migration done
dao_rabbitmq                           | 2022-04-24 10:29:56.748761+00:00 [info] <0.228.0> Feature flag `quorum_queue`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.750342+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.750394+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.750410+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.750420+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.750429+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.750458+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.750468+00:00 [info] <0.228.0> Feature flags:   [ ] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.750475+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.750484+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.750491+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.755139+00:00 [info] <0.228.0> Feature flag `stream_queue`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.755187+00:00 [info] <0.228.0> Feature flag `stream_queue`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.755706+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.755744+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.755755+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.755765+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.755772+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.755779+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.755895+00:00 [info] <0.228.0> Feature flags:   [~] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.755928+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.755955+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.755966+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.761032+00:00 [info] <0.228.0> Feature flag `stream_queue`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.762759+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.762782+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.762808+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.762818+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.762871+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.762882+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.762890+00:00 [info] <0.228.0> Feature flags:   [x] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.762929+00:00 [info] <0.228.0> Feature flags:   [ ] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.762941+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.762959+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.766951+00:00 [info] <0.228.0> Feature flag `user_limits`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.767020+00:00 [info] <0.228.0> Feature flag `user_limits`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.767562+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.767595+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.767624+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.767661+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.767690+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.767707+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.767732+00:00 [info] <0.228.0> Feature flags:   [x] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.767803+00:00 [info] <0.228.0> Feature flags:   [~] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.767825+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.767847+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.772831+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.772889+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.783082+00:00 [info] <0.228.0> Feature flag `user_limits`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.784530+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.784554+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.784573+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.784581+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.784603+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.784612+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.784619+00:00 [info] <0.228.0> Feature flags:   [x] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.784626+00:00 [info] <0.228.0> Feature flags:   [x] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.784646+00:00 [info] <0.228.0> Feature flags:   [ ] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.784665+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.790528+00:00 [info] <0.228.0> Feature flag `virtual_host_metadata`: supported, attempt to enable...
dao_rabbitmq                           | 2022-04-24 10:29:56.790606+00:00 [info] <0.228.0> Feature flag `virtual_host_metadata`: mark as enabled=state_changing
dao_rabbitmq                           | 2022-04-24 10:29:56.791322+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.791345+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.791363+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.791438+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.791450+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.791458+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.791467+00:00 [info] <0.228.0> Feature flags:   [x] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.791474+00:00 [info] <0.228.0> Feature flags:   [x] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.791481+00:00 [info] <0.228.0> Feature flags:   [~] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.791520+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.795745+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.795824+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.806004+00:00 [info] <0.228.0> Feature flag `virtual_host_metadata`: mark as enabled=true
dao_rabbitmq                           | 2022-04-24 10:29:56.807826+00:00 [info] <0.228.0> Feature flags: list of feature flags found:
dao_rabbitmq                           | 2022-04-24 10:29:56.807857+00:00 [info] <0.228.0> Feature flags:   [x] drop_unroutable_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.807870+00:00 [info] <0.228.0> Feature flags:   [x] empty_basic_get_metric
dao_rabbitmq                           | 2022-04-24 10:29:56.807879+00:00 [info] <0.228.0> Feature flags:   [x] implicit_default_bindings
dao_rabbitmq                           | 2022-04-24 10:29:56.807933+00:00 [info] <0.228.0> Feature flags:   [x] maintenance_mode_status
dao_rabbitmq                           | 2022-04-24 10:29:56.807946+00:00 [info] <0.228.0> Feature flags:   [x] quorum_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.807954+00:00 [info] <0.228.0> Feature flags:   [x] stream_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.807962+00:00 [info] <0.228.0> Feature flags:   [x] user_limits
dao_rabbitmq                           | 2022-04-24 10:29:56.807996+00:00 [info] <0.228.0> Feature flags:   [x] virtual_host_metadata
dao_rabbitmq                           | 2022-04-24 10:29:56.808009+00:00 [info] <0.228.0> Feature flags: feature flag states written to disk: yes
dao_rabbitmq                           | 2022-04-24 10:29:56.812255+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.812329+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.818795+00:00 [info] <0.228.0> Waiting for Mnesia tables for 30000 ms, 9 retries left
dao_rabbitmq                           | 2022-04-24 10:29:56.818863+00:00 [info] <0.228.0> Successfully synced tables from a peer
dao_rabbitmq                           | 2022-04-24 10:29:56.818879+00:00 [info] <0.228.0> Peer discovery backend rabbit_peer_discovery_classic_config does not support registration, skipping registration.
dao_rabbitmq                           | 2022-04-24 10:29:56.818898+00:00 [info] <0.228.0> Will try to unlock with peer discovery backend rabbit_peer_discovery_classic_config
dao_rabbitmq                           | 2022-04-24 10:29:56.818926+00:00 [info] <0.228.0> Running boot step database_sync defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819056+00:00 [info] <0.228.0> Running boot step feature_flags defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819334+00:00 [info] <0.228.0> Running boot step codec_correctness_check defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819361+00:00 [info] <0.228.0> Running boot step external_infrastructure defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819373+00:00 [info] <0.228.0> Running boot step rabbit_registry defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819472+00:00 [info] <0.228.0> Running boot step rabbit_auth_mechanism_cr_demo defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819521+00:00 [info] <0.228.0> Running boot step rabbit_queue_location_random defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819814+00:00 [info] <0.228.0> Running boot step rabbit_event defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.819956+00:00 [info] <0.228.0> Running boot step rabbit_auth_mechanism_amqplain defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820086+00:00 [info] <0.228.0> Running boot step rabbit_auth_mechanism_plain defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820187+00:00 [info] <0.228.0> Running boot step rabbit_exchange_type_direct defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820249+00:00 [info] <0.228.0> Running boot step rabbit_exchange_type_fanout defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820299+00:00 [info] <0.228.0> Running boot step rabbit_exchange_type_headers defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820326+00:00 [info] <0.228.0> Running boot step rabbit_exchange_type_topic defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820447+00:00 [info] <0.228.0> Running boot step rabbit_mirror_queue_mode_all defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820567+00:00 [info] <0.228.0> Running boot step rabbit_mirror_queue_mode_exactly defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820619+00:00 [info] <0.228.0> Running boot step rabbit_mirror_queue_mode_nodes defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820737+00:00 [info] <0.228.0> Running boot step rabbit_priority_queue defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.820763+00:00 [info] <0.228.0> Priority queues enabled, real BQ is rabbit_variable_queue
dao_rabbitmq                           | 2022-04-24 10:29:56.820970+00:00 [info] <0.228.0> Running boot step rabbit_queue_location_client_local defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.821080+00:00 [info] <0.228.0> Running boot step rabbit_queue_location_min_masters defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.821166+00:00 [info] <0.228.0> Running boot step kernel_ready defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.821225+00:00 [info] <0.228.0> Running boot step rabbit_sysmon_minder defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.821321+00:00 [info] <0.228.0> Running boot step rabbit_epmd_monitor defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.821972+00:00 [info] <0.568.0> epmd monitor knows us, inter-node communication (distribution) port: 25672
dao_rabbitmq                           | 2022-04-24 10:29:56.822070+00:00 [info] <0.228.0> Running boot step guid_generator defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.823449+00:00 [info] <0.228.0> Running boot step rabbit_node_monitor defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.823557+00:00 [info] <0.572.0> Starting rabbit_node_monitor
dao_rabbitmq                           | 2022-04-24 10:29:56.823787+00:00 [info] <0.228.0> Running boot step delegate_sup defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.824270+00:00 [info] <0.228.0> Running boot step rabbit_memory_monitor defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.824532+00:00 [info] <0.228.0> Running boot step core_initialized defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.824552+00:00 [info] <0.228.0> Running boot step upgrade_queues defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.828814+00:00 [info] <0.228.0> message_store upgrades: 1 to apply
dao_rabbitmq                           | 2022-04-24 10:29:56.828899+00:00 [info] <0.228.0> message_store upgrades: Applying rabbit_variable_queue:move_messages_to_vhost_store
dao_rabbitmq                           | 2022-04-24 10:29:56.828978+00:00 [info] <0.228.0> message_store upgrades: No durable queues found. Skipping message store migration
dao_rabbitmq                           | 2022-04-24 10:29:56.829150+00:00 [info] <0.228.0> message_store upgrades: Removing the old message store data
dao_rabbitmq                           | 2022-04-24 10:29:56.830044+00:00 [info] <0.228.0> message_store upgrades: All upgrades applied successfully
dao_rabbitmq                           | 2022-04-24 10:29:56.834568+00:00 [info] <0.228.0> Running boot step channel_tracking defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.836876+00:00 [info] <0.228.0> Setting up a table for channel tracking on this node: tracked_channel_on_node_rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:56.839475+00:00 [info] <0.228.0> Setting up a table for channel tracking on this node: tracked_channel_table_per_user_on_node_rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:56.839692+00:00 [info] <0.228.0> Running boot step rabbit_channel_tracking_handler defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.839771+00:00 [info] <0.228.0> Running boot step connection_tracking defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.842512+00:00 [info] <0.228.0> Setting up a table for connection tracking on this node: tracked_connection_on_node_rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:56.845020+00:00 [info] <0.228.0> Setting up a table for per-vhost connection counting on this node: tracked_connection_per_vhost_on_node_rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:56.847381+00:00 [info] <0.228.0> Setting up a table for per-user connection counting on this node: tracked_connection_table_per_user_on_node_rabbit@1d52ae8b94cd
dao_rabbitmq                           | 2022-04-24 10:29:56.847550+00:00 [info] <0.228.0> Running boot step rabbit_connection_tracking_handler defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.847629+00:00 [info] <0.228.0> Running boot step rabbit_exchange_parameters defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.847671+00:00 [info] <0.228.0> Running boot step rabbit_mirror_queue_misc defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.847812+00:00 [info] <0.228.0> Running boot step rabbit_policies defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848062+00:00 [info] <0.228.0> Running boot step rabbit_policy defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848154+00:00 [info] <0.228.0> Running boot step rabbit_queue_location_validator defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848219+00:00 [info] <0.228.0> Running boot step rabbit_quorum_memory_manager defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848253+00:00 [info] <0.228.0> Running boot step rabbit_stream_coordinator defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848458+00:00 [info] <0.228.0> Running boot step rabbit_vhost_limit defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.848508+00:00 [info] <0.228.0> Running boot step rabbit_mgmt_reset_handler defined by app rabbitmq_management
dao_rabbitmq                           | 2022-04-24 10:29:56.848530+00:00 [info] <0.228.0> Running boot step rabbit_mgmt_db_handler defined by app rabbitmq_management_agent
dao_rabbitmq                           | 2022-04-24 10:29:56.848544+00:00 [info] <0.228.0> Management plugin: using rates mode 'basic'
dao_rabbitmq                           | 2022-04-24 10:29:56.848730+00:00 [info] <0.228.0> Running boot step recovery defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.849550+00:00 [info] <0.228.0> Running boot step empty_db_check defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.849577+00:00 [info] <0.228.0> Will seed default virtual host and user...
dao_rabbitmq                           | 2022-04-24 10:29:56.849617+00:00 [info] <0.228.0> Adding vhost '/' (description: 'Default virtual host', tags: [])
dao_rabbitmq                           | 2022-04-24 10:29:56.855703+00:00 [info] <0.633.0> Making sure data directory '/var/lib/rabbitmq/mnesia/rabbit@1d52ae8b94cd/msg_stores/vhosts/628WB79CIFDYO9LJI6DKMI09L' for vhost '/' exists
dao_rabbitmq                           | 2022-04-24 10:29:56.856893+00:00 [info] <0.633.0> Setting segment_entry_count for vhost '/' with 0 queues to '2048'
dao_rabbitmq                           | 2022-04-24 10:29:56.858504+00:00 [info] <0.633.0> Starting message stores for vhost '/'
dao_rabbitmq                           | 2022-04-24 10:29:56.858601+00:00 [info] <0.637.0> Message store "628WB79CIFDYO9LJI6DKMI09L/msg_store_transient": using rabbit_msg_store_ets_index to provide index
dao_rabbitmq                           | 2022-04-24 10:29:56.859805+00:00 [info] <0.633.0> Started message store of type transient for vhost '/'
dao_rabbitmq                           | 2022-04-24 10:29:56.859897+00:00 [info] <0.641.0> Message store "628WB79CIFDYO9LJI6DKMI09L/msg_store_persistent": using rabbit_msg_store_ets_index to provide index
dao_rabbitmq                           | 2022-04-24 10:29:56.860542+00:00 [warning] <0.641.0> Message store "628WB79CIFDYO9LJI6DKMI09L/msg_store_persistent": rebuilding indices from scratch
dao_rabbitmq                           | 2022-04-24 10:29:56.861271+00:00 [info] <0.633.0> Started message store of type persistent for vhost '/'
dao_rabbitmq                           | 2022-04-24 10:29:56.861370+00:00 [info] <0.633.0> Recovering 0 queues of type rabbit_classic_queue took 4ms
dao_rabbitmq                           | 2022-04-24 10:29:56.861402+00:00 [info] <0.633.0> Recovering 0 queues of type rabbit_quorum_queue took 0ms
dao_rabbitmq                           | 2022-04-24 10:29:56.861418+00:00 [info] <0.633.0> Recovering 0 queues of type rabbit_stream_queue took 0ms
dao_rabbitmq                           | 2022-04-24 10:29:56.862978+00:00 [info] <0.228.0> Created user 'daorabbit'
dao_rabbitmq                           | 2022-04-24 10:29:56.863737+00:00 [info] <0.228.0> Successfully set user tags for user 'daorabbit' to [administrator]
dao_rabbitmq                           | 2022-04-24 10:29:56.864513+00:00 [info] <0.228.0> Successfully set permissions for 'daorabbit' in virtual host '/' to '.*', '.*', '.*'
dao_rabbitmq                           | 2022-04-24 10:29:56.864553+00:00 [info] <0.228.0> Running boot step rabbit_looking_glass defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864570+00:00 [info] <0.228.0> Running boot step rabbit_core_metrics_gc defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864627+00:00 [info] <0.228.0> Running boot step background_gc defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864735+00:00 [info] <0.228.0> Running boot step routing_ready defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864776+00:00 [info] <0.228.0> Running boot step pre_flight defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864789+00:00 [info] <0.228.0> Running boot step notify_cluster defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864806+00:00 [info] <0.228.0> Running boot step networking defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864835+00:00 [info] <0.228.0> Running boot step definition_import_worker_pool defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.864866+00:00 [info] <0.285.0> Starting worker pool 'definition_import_pool' with 8 processes in it
dao_rabbitmq                           | 2022-04-24 10:29:56.865358+00:00 [info] <0.228.0> Running boot step cluster_name defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.865405+00:00 [info] <0.228.0> Initialising internal cluster ID to 'rabbitmq-cluster-id-cwCPeBXxIWk2DteBwY634A'
dao_rabbitmq                           | 2022-04-24 10:29:56.866229+00:00 [info] <0.228.0> Running boot step direct_client defined by app rabbit
dao_rabbitmq                           | 2022-04-24 10:29:56.866341+00:00 [info] <0.228.0> Running boot step rabbit_management_load_definitions defined by app rabbitmq_management
dao_rabbitmq                           | 2022-04-24 10:29:56.866440+00:00 [info] <0.678.0> Resetting node maintenance status
dao_rabbitmq                           | 2022-04-24 10:29:56.874688+00:00 [info] <0.737.0> Management plugin: HTTP (non-TLS) listener started on port 15672
dao_rabbitmq                           | 2022-04-24 10:29:56.874821+00:00 [info] <0.765.0> Statistics database started.
dao_rabbitmq                           | 2022-04-24 10:29:56.874889+00:00 [info] <0.764.0> Starting worker pool 'management_worker_pool' with 3 processes in it
dao_rabbitmq                           | 2022-04-24 10:29:56.879787+00:00 [info] <0.779.0> Prometheus metrics: HTTP (non-TLS) listener started on port 15692
dao_rabbitmq                           | 2022-04-24 10:29:56.879869+00:00 [info] <0.678.0> Ready to start client connection listeners
dao_rabbitmq                           | 2022-04-24 10:29:56.881087+00:00 [info] <0.823.0> started TCP listener on [::]:5672
dao_rabbitmq                           |  completed with 4 plugins.
dao_rabbitmq                           | 2022-04-24 10:29:56.941107+00:00 [info] <0.678.0> Server startup complete; 4 plugins started.
dao_rabbitmq                           | 2022-04-24 10:29:56.941107+00:00 [info] <0.678.0>  * rabbitmq_prometheus
dao_rabbitmq                           | 2022-04-24 10:29:56.941107+00:00 [info] <0.678.0>  * rabbitmq_management
dao_rabbitmq                           | 2022-04-24 10:29:56.941107+00:00 [info] <0.678.0>  * rabbitmq_web_dispatch
dao_rabbitmq                           | 2022-04-24 10:29:56.941107+00:00 [info] <0.678.0>  * rabbitmq_management_agent
dao_rabbitmq                           | 2022-04-24 10:30:02.173608+00:00 [info] <0.835.0> accepting AMQP connection <0.835.0> (172.18.0.10:40298 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.181834+00:00 [info] <0.838.0> accepting AMQP connection <0.838.0> (172.18.0.11:59358 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.193762+00:00 [info] <0.835.0> connection <0.835.0> (172.18.0.10:40298 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.206943+00:00 [info] <0.838.0> connection <0.838.0> (172.18.0.11:59358 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.211738+00:00 [info] <0.865.0> accepting AMQP connection <0.865.0> (172.18.0.10:40300 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.215082+00:00 [info] <0.865.0> connection <0.865.0> (172.18.0.10:40300 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.226251+00:00 [info] <0.878.0> accepting AMQP connection <0.878.0> (172.18.0.11:59362 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.228021+00:00 [info] <0.878.0> connection <0.878.0> (172.18.0.11:59362 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.243036+00:00 [info] <0.891.0> accepting AMQP connection <0.891.0> (172.18.0.12:42876 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.263091+00:00 [info] <0.891.0> connection <0.891.0> (172.18.0.12:42876 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.272306+00:00 [info] <0.904.0> accepting AMQP connection <0.904.0> (172.18.0.12:42878 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.280966+00:00 [info] <0.904.0> connection <0.904.0> (172.18.0.12:42878 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
servicesdao-dao_identityservice-1      | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_identityservice-1      |       Now listening on: http://[::]:80
servicesdao-dao_identityservice-1      | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_identityservice-1      |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_identityservice-1      | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_identityservice-1      |       Hosting environment: Development
servicesdao-dao_identityservice-1      | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_identityservice-1      |       Content root path: /app
dao_rabbitmq                           | 2022-04-24 10:30:02.362080+00:00 [info] <0.918.0> accepting AMQP connection <0.918.0> (172.18.0.14:41554 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.362579+00:00 [info] <0.921.0> accepting AMQP connection <0.921.0> (172.18.0.9:58962 -> 172.18.0.8:5672)
servicesdao-dao_apigateway-1           | warn: Microsoft.AspNetCore.DataProtection.Repositories.FileSystemXmlRepository[60]
servicesdao-dao_apigateway-1           |       Storing keys in a directory '/root/.aspnet/DataProtection-Keys' that may not be persisted outside of the container. Protected data will be unavailable when container is destroyed.
dao_rabbitmq                           | 2022-04-24 10:30:02.384679+00:00 [info] <0.918.0> connection <0.918.0> (172.18.0.14:41554 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.385220+00:00 [info] <0.921.0> connection <0.921.0> (172.18.0.9:58962 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:02.392969+00:00 [info] <0.944.0> accepting AMQP connection <0.944.0> (172.18.0.14:41556 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.395015+00:00 [info] <0.947.0> accepting AMQP connection <0.947.0> (172.18.0.9:58964 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:02.395084+00:00 [info] <0.944.0> connection <0.944.0> (172.18.0.14:41556 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
servicesdao-dao_apigateway-1           | warn: Microsoft.AspNetCore.DataProtection.KeyManagement.XmlKeyManager[35]
servicesdao-dao_apigateway-1           |       No XML encryptor configured. Key {d3d9dc70-e6f5-4845-95c6-67c81e5de3bd} may be persisted to storage in unencrypted form.
dao_rabbitmq                           | 2022-04-24 10:30:02.397535+00:00 [info] <0.947.0> connection <0.947.0> (172.18.0.9:58964 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
servicesdao-dao_notificationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_notificationservice-1  |       Now listening on: http://[::]:80
servicesdao-dao_notificationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_notificationservice-1  |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_notificationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_notificationservice-1  |       Hosting environment: Development
servicesdao-dao_notificationservice-1  | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_notificationservice-1  |       Content root path: /app
servicesdao-dao_apigateway-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_apigateway-1           |       Now listening on: http://[::]:80
servicesdao-dao_apigateway-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_apigateway-1           |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_apigateway-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_apigateway-1           |       Hosting environment: Development
servicesdao-dao_apigateway-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_apigateway-1           |       Content root path: /app
servicesdao-dao_logservice-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_logservice-1           |       Now listening on: http://[::]:80
servicesdao-dao_logservice-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_logservice-1           |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_logservice-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_logservice-1           |       Hosting environment: Development
servicesdao-dao_logservice-1           | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_logservice-1           |       Content root path: /app
servicesdao-dao_dbservice-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_dbservice-1            |       Now listening on: http://[::]:80
servicesdao-dao_dbservice-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_dbservice-1            |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_dbservice-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_dbservice-1            |       Hosting environment: Development
servicesdao-dao_dbservice-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_dbservice-1            |       Content root path: /app
servicesdao-dao_apigateway-1           | info: Ocelot.RateLimit.Middleware.ClientRateLimitMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TP:00000001, previousRequestId: no previous request id, message: EndpointRateLimiting is not enabled for /PlatformSetting/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authentication.Middleware.AuthenticationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TP:00000001, previousRequestId: no previous request id, message: No authentication needed for /PublicActions/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authorisation.Middleware.AuthorisationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TP:00000001, previousRequestId: no previous request id, message: /PlatformSetting/GetLatestSetting route does not require user to be authorised
servicesdao-dao_apigateway-1           | info: Ocelot.Requester.Middleware.HttpRequesterMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TP:00000001, previousRequestId: no previous request id, message: 204 (No Content) status code, request uri: http://dao_dbservice/PlatformSetting/GetLatestSetting
dao_rabbitmq                           | 2022-04-24 10:30:12.504332+00:00 [info] <0.1006.0> accepting AMQP connection <0.1006.0> (172.18.0.13:60320 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:12.520167+00:00 [info] <0.1006.0> connection <0.1006.0> (172.18.0.13:60320 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
dao_rabbitmq                           | 2022-04-24 10:30:12.526823+00:00 [info] <0.1019.0> accepting AMQP connection <0.1019.0> (172.18.0.13:60322 -> 172.18.0.8:5672)
dao_rabbitmq                           | 2022-04-24 10:30:12.528679+00:00 [info] <0.1019.0> connection <0.1019.0> (172.18.0.13:60322 -> 172.18.0.8:5672): user 'daorabbit' authenticated and granted access to vhost '/'
servicesdao-dao_webportal-1            | warn: Microsoft.AspNetCore.DataProtection.Repositories.FileSystemXmlRepository[60]
servicesdao-dao_webportal-1            |       Storing keys in a directory '/root/.aspnet/DataProtection-Keys' that may not be persisted outside of the container. Protected data will be unavailable when container is destroyed.
servicesdao-dao_webportal-1            | warn: Microsoft.AspNetCore.DataProtection.KeyManagement.XmlKeyManager[35]
servicesdao-dao_webportal-1            |       No XML encryptor configured. Key {124ef9fb-f259-42d5-a861-0dbbaae8c71b} may be persisted to storage in unencrypted form.
servicesdao-dao_webportal-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_webportal-1            |       Now listening on: http://[::]:80
servicesdao-dao_webportal-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_webportal-1            |       Application started. Press Ctrl+C to shut down.
servicesdao-dao_webportal-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_webportal-1            |       Hosting environment: Development
servicesdao-dao_webportal-1            | info: Microsoft.Hosting.Lifetime[0]
servicesdao-dao_webportal-1            |       Content root path: /app
servicesdao-dao_apigateway-1           | warn: Ocelot.DownstreamRouteFinder.Middleware.DownstreamRouteFinderMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TQ:00000003, previousRequestId: no previous request id, message: DownstreamRouteFinderMiddleware setting pipeline errors. IDownstreamRouteFinder returned Error Code: UnableToFindDownstreamRouteError Message: Failed to match ReRoute configuration for upstream path: /favicon.ico, verb: GET.
servicesdao-dao_apigateway-1           | warn: Ocelot.Responder.Middleware.ResponderMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TQ:00000003, previousRequestId: no previous request id, message: Error Code: UnableToFindDownstreamRouteError Message: Failed to match ReRoute configuration for upstream path: /favicon.ico, verb: GET. errors found in ResponderMiddleware. Setting error response for request path:/favicon.ico, request method: GET
servicesdao-dao_apigateway-1           | info: Ocelot.RateLimit.Middleware.ClientRateLimitMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TS:00000001, previousRequestId: no previous request id, message: EndpointRateLimiting is not enabled for /PlatformSetting/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authentication.Middleware.AuthenticationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TS:00000001, previousRequestId: no previous request id, message: No authentication needed for /PublicActions/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authorisation.Middleware.AuthorisationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TS:00000001, previousRequestId: no previous request id, message: /PlatformSetting/GetLatestSetting route does not require user to be authorised
servicesdao-dao_apigateway-1           | info: Ocelot.Requester.Middleware.HttpRequesterMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TS:00000001, previousRequestId: no previous request id, message: 204 (No Content) status code, request uri: http://dao_dbservice/PlatformSetting/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.RateLimit.Middleware.ClientRateLimitMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TT:00000001, previousRequestId: no previous request id, message: EndpointRateLimiting is not enabled for /PlatformSetting/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authentication.Middleware.AuthenticationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TT:00000001, previousRequestId: no previous request id, message: No authentication needed for /PublicActions/GetLatestSetting
servicesdao-dao_apigateway-1           | info: Ocelot.Authorisation.Middleware.AuthorisationMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TT:00000001, previousRequestId: no previous request id, message: /PlatformSetting/GetLatestSetting route does not require user to be authorised
servicesdao-dao_apigateway-1           | info: Ocelot.Requester.Middleware.HttpRequesterMiddleware[0]
servicesdao-dao_apigateway-1           |       requestId: 0HMH5RLL020TT:00000001, previousRequestId: no previous request id, message: 204 (No Content) status code, request uri: http://dao_dbservice/PlatformSetting/GetLatestSetting

```

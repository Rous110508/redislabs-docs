---
Title: Proxy object
linkTitle: proxy
description: An object that represents a proxy in the cluster
weight: $weight
alwaysopen: false
categories: ["RS"]
---

An API object that represents a [proxy](https://en.wikipedia.org/wiki/Proxy_server) in the cluster.

| Name | Type/Value | Description |
|------|------------|-------------|
| uid                                  | integer     | Unique ID of proxy (read-only) |
| threads                              | integer, <nobr>(range: 1-256)</nobr> | Number of threads |
| max_threads                          | integer, <nobr>(range: 1-256)</nobr> | Max number of threads |
| dynamic_threads_scaling              | boolean     | Automatically adjust the number of threads|
| threads_usage_threshold              | integer, <nobr>(range: 50-99)</nobr> | Max number of threads |
| duration_usage_threshold             | integer, <nobr>(range: 10-300)</nobr> | Max number of threads |
| backlog                              | integer     | tcp listen queue backlog |
| conns                                | integer     | Number of connections |
| client_keepcnt                       | integer     | Client tcp keepalive count |
| client_keepidle                      | integer     | Client tcp keepalive idle |
| client_keepintvl                     | integer     | Client tcp keepalive interval |
| max_servers                          | integer     | Max number of Redis servers |
| max_listeners                        | integer     | Max number of listeners |
| max_worker_client_conns              | integer     | Max client connections per thread |
| max_worker_server_conns              | integer     | Max server connections per thread |
| max_worker_txns                      | integer     | Max in-flight transactions per thread |
| ignore_bdb_cconn_limit               | boolean     | Ignore client connection limits |
| ignore_bdb_cconn_output_buff_limits  | boolean     | Ignore buffer limit |
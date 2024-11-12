# DuckDB C API Headers
This directory contains the C API headers of DuckDB. These headers should be of the same 
DuckDB version as is specified in `Makefile`. Note that these headers can be updated automatically 
to match the `MINIMUM_DUCKDB_VERSION` makefile variable by running (assuming the default makefile setup):

```shell
make update_duckdb_headers
```

Of course manually updating the headers is also fine, just make sure that the headers are always from the same 
DuckDB version and that they are not from a later release of DuckDB than is specified in the `MINIMUM_DUCKDB_VERSION`
build variable. Using headers from an older version than `MINIMUM_DUCKDB_VERSION` is allowed, but you probably don't want
that.
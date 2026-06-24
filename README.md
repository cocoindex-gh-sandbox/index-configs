# index-configs

Tenant configuration for the **cccx** indexer (CocoIndex Code Plus) test sandbox.

`configs/*.json` map a `tenant_key` to a repo + include/exclude globs. The
indexer (`CCCX_CONFIG_REPO_OWNER=cocoindex-gh-sandbox`,
`CCCX_CONFIG_REPO_NAME=index-configs`, `CCCX_CONFIG_DIR=configs`) polls this repo
and indexes each tenant. Set `to_delete: true` on an entry to drop a tenant.

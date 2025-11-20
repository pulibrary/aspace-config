# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**We are on v4.1.1 (prod) and v4.1.1 (staging)**

## Plugins

Please refer to [this spreadsheet](https://docs.google.com/spreadsheets/d/1uRQCC2rJ4qw-rwTP4B_n7PhDdcTJjo2_gL-eywoTe-k/edit?gid=0#gid=0) in the ArchivesSpace Operations Group's Google Drive for up-to-date information on installed plugins.
          
## Other configuration choices

| setting | staging | prod |
| ------ | ------- | ---- |
| SOLR | `AppConfig[:indexer_records_per_thread] = 15 AppConfig[:indexer_thread_count] = 2 AppConfig[:pui_indexer_enabled] = false` | `AppConfig[:indexer_records_per_thread] = 15 AppConfig[:indexer_thread_count] = 2 AppConfig[:pui_indexer_enabled] = false` (updated 12/10/23) |
| metadata permissions| n/a | AppConfig[:spreadsheet_bulk_updater_apply_deletes] = true |
| infrastructure | ASpace (in Docker container) and SOLR running on one ECS server; MySQL on separate shared RDS MySQL server | ASpace and SOLR running on one ECS server; MySQL on separate shared RDS MySQL server | 

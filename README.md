# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**We are on v3.5.1 (prod) and v3.5.1 (staging)**

## Plugins

| plugin | staging | prod |
| ------ | ------- | ---- |
| aspace-oauth | branch: v3.2.0 <br/> url: https://github.com/lyrasis/aspace-oauth.git | branch: v3.2.0 <br/> url: https://github.com/lyrasis/aspace-oauth.git |
| as_marcao | branch: v1.0 <br/> url: https://github.com/hudmol/as_marcao.git <br/> updated: 6/17/2024| branch: v1.0 <br/> url: https://github.com/hudmol/as_marcao.git <br/> updated: 5/30/2023 |
| as_princeton_shim | [removed 4/26/2024] | branch: v1.0 <br/> url: https://github.com/hudmol/as_princeton_shim.git |
| as_spreadsheet_bulk_updater | branch: main <br/> url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git </br> create_missing_top_containers: true| branch: main <br/> url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git </br> max_top_container_results: true |
| digitization_workorder | branch: master <br/> url: https://github.com/duke-libraries/digitization_work_order.git | branch: master <br/> url: https://github.com/duke-libraries/digitization_work_order.git |
| editable_external_ids | branch: master <br/> url: https://github.com/hudmol/editable_external_ids.git | n/a |
| newrelic | n/a | url: https://github.com/archivesspace-plugins/newrelic.git <br/> branch: master <br/> restricted: true |
| next_accession | branch: master <br/> url: https://github.com/duspeccoll/next_accession.git| branch: master </br> url: https://github.com/duspeccoll/next_accession.git |
| princeton_ead_exporter | branch: main <br/> url: https://github.com/pulibrary/princeton_ead_exporter.git | branch: main <br/> url: https://github.com/pulibrary/princeton_ead_exporter.git |
| refid_rules | branch: master <br/> url: https://github.com/archivesspace-plugins/refid_rules.git | branch: master <br/> url: https://github.com/archivesspace-plugins/refid_rules.git
| timewalk | n/a | branch: master <br/> url: https://github.com/alexduryee/timewalk.git
| user_defined_in_basic | branch: release 1.0<br/> url: https://github.com/hudmol/user_defined_in_basic.git <br/> updated: 4/20/2023 | branch: '1.0' <br/> url: https://github.com/hudmol/user_defined_in_basic.git <br/> updated: 5/30/2023

## Other configuration choices

| setting | staging | prod |
| ------ | ------- | ---- |
| SOLR | `AppConfig[:indexer_records_per_thread] = 15 AppConfig[:indexer_thread_count] = 2 AppConfig[:pui_indexer_enabled] = false` | `AppConfig[:indexer_records_per_thread] = 15 AppConfig[:indexer_thread_count] = 2 AppConfig[:pui_indexer_enabled] = false` (updated 12/10/23) |
| infrastructure | ASpace (in Docker container) and SOLR running on one ECS server; MySQL on separate shared RDS MySQL server | ASpace and SOLR running on one ECS server; MySQL on separate shared RDS MySQL server | 

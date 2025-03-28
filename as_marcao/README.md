To install:

1. clone [user_defined_in_basic](https://github.com/hudmol/user_defined_in_basic) to the `plugins` directory
2. clone [as_marcao](https://github.com/hudmol/as_marcao) to the `plugins` directory
3. add `user_defined_in_basic` to `AppConfig[:plugins]` in `common/config/config-defaults.rb`
4. add `as_marcao` to `AppConfig[:plugins]` in `common/config/config-defaults.rb`
5. add configurations for `user_defined_in_basic`:
```
  AppConfig[:user_defined_in_basic] = {
  "accessions" => ["date_1", "text_1", "text_2", "text_3", "boolean_1", "boolean_2", "boolean_3", "date_2", "string_1", "string_2", "string_3", "string_4", "real_1", "real_2", "enum_2"],
  "digital_objects" => [],
  "resources" => ["boolean_1"],
  "hide_user_defined_section" => true
  }
```
6. add configurations for `as_marcao`:
```
  AppConfig[:marcao_schedule] = '22 2 * * *'
  AppConfig[:marcao_flag_field] = 'boolean_1'
  AppConfig[:marcao_sftp_host] = '127.0.0.1'
  AppConfig[:marcao_sftp_user] = 'a_user'
  AppConfig[:marcao_sftp_password] = 'secret password'
  AppConfig[:marcao_sftp_path] = '/remote/path'
  AppConfig[:marcao_sftp_timeout] = 30
```
7. add `en.yml`
   This is a top-level file in `locales`, which sits right inside `archivesspace`. Contrary to what the documentation says, it is not exposed in the docker image version. Do
   ```
   docker cp ~path/to/en.yml archivesspace:/archivesspace/locales
   ```
8. run `./setup-database.sh`

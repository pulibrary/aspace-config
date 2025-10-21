### To install:

1. clone [user_defined_in_basic](https://github.com/hudmol/user_defined_in_basic) to the `plugins` directory
2. clone [as_marcao](https://github.com/hudmol/as_marcao) to the `plugins` directory
3. add `user_defined_in_basic` to `AppConfig[:plugins]` in `common/config/config-defaults.rb`
4. add `as_marcao` to `AppConfig[:plugins]` in `common/config/config-defaults.rb` (3.5.1) or `config/config.rb` (4.x)
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
   This is a top-level file in `locales`, which sits right inside `archivesspace`. Contrary to what the 4.0 documentation says, it is not exposed in the docker image version. Do
   ```
   docker cp ~path/to/en.yml archivesspace:/archivesspace/locales
   ```

### To troubleshoot:

1. To run manually, change the schedule in config.rb, then restart
2. The output file `marcao_export.xml` gets saved to `/build/dev/shared/marcao`
3. The report of the last successful run is called `report.json` and gets saved to the same directory
   (It only gets saved after the first _successful_ run, including sftp upload. In other words, if something goes after the initial install or right after an update, no report gets saved.)

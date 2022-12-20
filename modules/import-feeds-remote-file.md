# Import Feeds: Remote File

This module enables manually or automatically import data from remote files located on a (s)FTP Server.

> Module `Import Feeds` is required for this module to work.

## Creating a Feed

To create import feed using Remote File select `(s)FTP` or `Path` as a `Type`. `Import Data Settings` will be adjusted automatically. 

![Selecting Remote File](_assets/import-feeds-remote-file/import-feeds-remote-file-create.png)

## Import Data Settings

### (s)FTP

Although you import by (s)FTP you will still need a sample file for configurator and mapping rules. Use it as your guiding hand and select any of the standard file type.

![IMPORT DATA SETTINGS tab with path option](_assets/import-feeds-remote-file/import-feeds-remote-file-sftp.png)

- `Connection` – select existing or create one (creating a new one will be mentioned in a separate menu)
- `Dir Path` – path (link) to the file/files
- `File Name / File Name Mask *` – if you know exact name of the file write it down. If you know the logic of naming or have multiple files with similar names you can use mask (part of name/names) to find all corresponding files
<!-- тут треба обовязково вказити приклад як писати маску -->
<!-- що буде якщо по масці буде знайдено більше чим один файл? -->

- `Delete Original File After Import` checkbox – set this option to delete all sucsessfully imported files from original place (to not use them again in future imports) after they are imported.

### Path

You can upload file to be used for configurator rules by stating `Dir Path` and `File Name / File Name Mask *`. Alternatively you can attach a file as usual.
<!-- для чого іконка стрілочки? --> 

![IMPORT DATA SETTINGS tab with path option](_assets/import-feeds-remote-file/import-feeds-remote-file-path.png)

- `Dir Path` – path (link) to the file/files
<!-- має починатись з чого? абсолютний чи відосний шлях? -->
- `File Name / File Name Mask *` – if you know exact name of the file write it down. If you know the logic of naming or have multiple files with similar names you can use mask (part of name/names) to find all corresponding files
- `Delete Original File After Import` checkbox - an option to clear all successfully imported files from original place (to not use them again in future imports).

<!-- цих 3 пункти уже було описано вище, навіщо ще раз? -->

### Connection menu

Here you can select established connections or create a new one. Use name, `Host` and `Port` to locate it and  `User` and `Password` (of your database) for the system to get access to it.

![create](_assets/import-feeds-database/import-feeds-database-connection.png)
<!-- цей урл побитий, треба його перевірити -->

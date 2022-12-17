# Export Feeds: Remote File

When you don't want to export files every time and upload them to the web you may use the `Export Feeds: Remote File` module. It will export data from your ATRO system to you using HTTP protocol in appropriate form.

> Note that you will still need `Export Feeds` module to export anything.

## Creating Remote File feed

To create remote file export feed select `(s)FTP` as a `Type`. You may need to adjust `Maximum Number of Records per Iteration *` option or leave it default. Then proceed as normal up to `EXPORT DATA SETTINGS` tab.

![Selecting HTTP request](_assets/export-feeds-remote-file/export-feeds-remote-file-create.png)

## EXPORT DATA SETTINGS tab

Select a format you want data to be exported in. You can use CSV, XLS, JSON or XML. For JSON or XML there is a `Template` to be set. After that fill the required fields.

- `Connection ` – select established connections or create a new one
- `File path *` – select url where request will go. It is mesured from the `Connection `.

![Selecting HTTP request](_assets/export-feeds-remote-file/export-feeds-remote-file-settings.png)

### Connection menu

Here you can select established connections or create a new one. Use name, `Host` and `Port` to locate it and  `User` and `Password` (of your database) for the system to get access to it.

![create](_assets/import-feeds-database/import-feeds-database-connection.png)
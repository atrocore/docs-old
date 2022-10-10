# Connector

The "Connector" module allows you to orchestrate multiple import and export feeds, of any type. Ypu can set the sort order for the execution of your feeds, run the sequence automatically as a scheduled or event-based job, or manually, in just one click. Also it adds additional functions to export and import feeds.

## Main functions

The "Connector" module was created primarily to be used together with Export and Import feeds, so further description of the module is given in the context of them.

To go to connector menu visit Dashboard/Connectors. There you can see all existing connectors, edit them, delete or create new.

![Main menu](_assets/connector/main-menu.png)

### Creating Connector

To create a connector click `Create Connector` button. You will see next menu

![Creating Connector](_assets/connector/creating.png)

Set the name, description and press the checkbox if you want it to be active. Then press `Save`. The menu next is the same as editing menu.

### Editing Connector

![Connector menu](_assets/connector/connector-menu.png)

In the `Feeds` section you can add or unlink export or import feeds. To add one press arrow and select `Select: Import Feed` or `Select: Export Feed` for import and export feeds apparently. To unlink one press tree dots and select `Unlink`.

You can also change the order of feeds to benefit your task. To do so, just grab and pull the feed.

### Running connector jobs

To run connector press `Execute`. This will launch all the feeds you set in `Feeds` section. The order of the feeds launched will be from the top feed down to the last. So, when and only when a previous feed is done as a success, a new one will start and so on to the last. If a result of a job is an error a new feed is not started and cancelled.

![Job list](_assets/connector/job-list.png)

![Running jobs](_assets/connector/running-jobs.png)

This will make sure your intent is achieved.

## Additional functions

"Connector" module also has some additional functions to help ypu export and import more flexible. It includes additional filtering and value modifiers.

### Additional filtering



### Value Modifiers
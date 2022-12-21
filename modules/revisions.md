# Revisions

The "Revisions" module provides users with the ability to easily work with the change history: view the field and attribute value changes history in the pop-up and restore previous values from the change history.

## Administrator Functions

After the "Revisions" module is installed, users will be able to see the change history of audited fields and restore these changes.

### Field Configuration

To enable storage of the change history for a particular field, perform the following actions:

1. Open the fields list of the desired entity in the Entity Manager and select the field in the "Name" column: 

![Edit Entity Fields](./_assets/revisions/edit-entity-fields.jpg)

2. On the field detail view page that opens, activate the `Audited` checkbox and save the field changes to enable its updates logging:

![Edit Entity Fields Audited](./_assets/revisions/edit-entity-fields-audited.jpg)

### Stream Configuration

For reviewing the changes in the Stream on the entity record page, `Stream` must be activated for the desired entity settings. To open the entity settings page, click `Edit` for the desired entity record in the Entity Manager:

![Enable stream](./_assets/revisions/enable_stream.jpg)

### Removing a Record from the Stream

> Administrator only has access to the single record actions for change history records displayed in the Stream.

To remove a change log entry, select this record in the Stream and select the `Remove` option from its single record actions list:

![Remove From Stream](./_assets/revisions/remove-from-stream.jpg)

> Beware that this action is irreversible.

After removing the entry from the Stream, it also disappears from the change history pop-up.

### Restoring Values from the Stream

Select the desired change in the stream and select the `Restore` option from its single record actions list:

![Restore in the stream](./_assets/revisions/stream-restore.jpg)

Confirm your decision by pressing the `Restore` button in the  pop-up warning that appears:

![Restore warning](./_assets/revisions/restore-warning.jpg)

The revert itself is logged similarly to manual changing of this field, i.e. a new change entry is added to the stream (with the information about the date and time, old and new field values and the user who made the revert).

### History of record changes in the Stream 

"Revisions" module allows you to track changes in post and comments in the stream. Select the arrow to summon a menu tracking changes to posts in a stream.

![Changes in the Stream](./_assets/revisions/stream-changes.png)

## User Functions

By design, user has access to the revision functionality for the field and [attribute](https://atropim.com/help/attributes) values only, but not the Stream.

### Changing the History Pop-Up Display

In order to see the change history of a certain field, click the clock icon located in the top right corner of this field on the entity detail view page:

![Revision Icon](./_assets/revisions/revision-icon.jpg) 

Then the pop-up opens with the list of changes in this field, if any:

![Revision List](./_assets/revisions/revision-list.jpg)

The following data is displayed in the "List" pop-up:

- the date and time of the change;
- the user name who made the change;
- the values of the field before (`Old Value`) and after (`New Value`) the change;
- the locale name, if a multilingual field was changed. 

To learn more about multilingual fields and locales please read [here](https://atropim.com/help/multilingualism-admin) and [here](https://atropim.com/help/multilingualism).

The be able to see the field history you need the editing right for this field.

### Restoring of an Old Field / Attribute Value 

To revert any change made to the audited **field**, click the `Restore` button for the desired change in the change history pop-up:

![Restore in the pop-up](./_assets/revisions/revision-list-restore.jpg)

Additionally, change history tracking and value restoration are available for product **attribute** values. For this use the `Show changes` option from the single record actions drop-down menu of the desired attribute on the "Product attributes" panel:

![Attributes tracking](./_assets/revisions/attributes-tracking.jpg)

# Advanced Navigation

The "Advanced Navigation" module allows to create navigation groups in order to improve the usability of your AtroСore, AtroPIM or AtroDAM system. Thanks to the module, you can combine the related navigation items into **groups**, e.g. Export Feeds and Export Jobs can be grouped into "Export". 

## Administrator Functions 

To configure the navigation menu, go to `Administration > User Interface`.

Please, note that after the "Advanced Navigation" module installation, the `...` tab, which is used to hide other navigation points, is no longer available in the "Add Item" pop-up window. In the "Advanced Navigation" module we assume that all navigation items are to be grouped. The `...` tab will be available again when the module is uninstalled from the AtroCore system.

### Navigation Groups

To create a new navigation group, click the `Add Group` button:

![Add group](./_assets/advanced-navigation/ui-add-group.jpg)

In the pop-up window that opens, enter the group name, and assign its icon and color, if needed:

![Add group](./_assets/advanced-navigation/add-group-popup.jpg)

Click `Save` to complete the group creation and return to the "User Interface" page; the created group will be added to the tab list:

![Added group](./_assets/advanced-navigation/added-group.jpg)

To edit the created group, use the pencil button located on the right of the corresponding group in the tab list and make the desired changes in the editing pop-up.

### Navigation Items

Navigation items are also managed on the "User Interface" page. To add a new item (or items) to the navigation group, click the `+` button on the right of the corresponding group in the tab list and select the desired items via the `Add` button in the pop-up that opens:

![Added group](./_assets/advanced-navigation/add-navigation-item.jpg)

Close the pop-up window to complete the operation; the added items will be displayed within the corresponding navigation group:

![Added items](./_assets/advanced-navigation/added-items.jpg)

The order of the grouped or ungrouped navigation items can be easily configured via drag-and-drop:

![Items ordering](./_assets/advanced-navigation/items-ordering.jpg)

Please, note that a menu item can be used only once in the navigation. So, to add an item, which is already used in the navigation menu, to the group, you will have to delete it first from the menu using the `x` button on its right and then add it to the desired group via the `+` button. Ungrouped items cannot be added to the group via drag-and-drop.

To apply the changes, click `Save` on the "User Interface" page. Refresh the page to see the updated advanced navigation menu:

![Advanced menu](./_assets/advanced-navigation/advanced-menu.jpg)

Please, note that an empty navigation group (i.e. with no navigation items inside) will not be displayed in the navigation menu.

## User Functions

With the "Advanced Navigation" module installed and configured by the administrator in the AtroCore system, users will see advanced navigation. Click the group name to unfold navigation points belonging to this group or to fold them back. 

Each user can configure his own navigation menu. To do this, select the `Custom tab list` checkbox on the "User interface" panel within the "Preferences" page. Create the desired navigation group and add items to it in the same way as it is described for the [administrator](#navigation-groups):

![Custom navigation menu](./_assets/advanced-navigation/custom-navigation-menu-cfg.jpg)

After the updates and upgrades of AtroCore, all settings made should remain. If they disappear, the "Advanced Navigation" module should be reinstalled – the disappeared settings will be restored, because the module stores them in a separate file. 

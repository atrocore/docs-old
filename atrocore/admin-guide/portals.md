# Portals

## What is Portal?

Portals are intended to give external users limited access to your system. These externals could be your suppliers, partners, customers, photographers, copywriters, translators, etc. A Portal may have own users, called Portal Users. Different Portal Roles may be assigned to Portal Users.

Here we describe an "Assets Portal", which sould be used for external photographers to work with product images (which are Assets for us).

## Creating a Portal

To create a portal go to `Administration / Portals` and press `Create Portal` button. 

On `General` panel you need to assign the Portal's name, role, set it active/inactive and assign an URL for the portal users to access it.
On the `Settings` panel you can set the `Default currency` and the default `Locale` for the portal users.

![discussion-button](../_assets/admin-guide/Assets_Portal/Assets_Portal.png)

In `user interface` tab you san set what entities new user can see. First, you can select logo and theme.

`Navigation menu` is all submenus user will be able to see (they will be available on his screen on the right). `Quick create list` is list of things user can create.

![discussion-button](../_assets/admin-guide/Assets_Portal/Assets_Portal2.png)

In the pictures above you can see an example of such portal. Using this particular one a photographer, for example, can upload product photos as assets personally. No other functions are available so no harm to you product information will be done. 

Portals can be also edited, duplicated or deleted.

## Portal Roles

Portal roles set rules and restrictions for portal users. To set them go to `Dashboard/Portal Roles` and create a new role by pressing `Create Portal Role` or edit existing one by clicking it and then pressing `Edit` button (see picture below). In this example we will continue editing a photographer's portal.

![discussion-button](../_assets/admin-guide/Assets_Portal/Assets_Portal3.png)

Here you can see entities and access rights of this role to them. Rights are entity-based (so you select them for each entity separately). They are:

- `Access` - rights to do anything in this entity. Without `Access` set to `enabled` there will be no rights you can see below (you can not do anything with the entity withot having access to it). You can set  `enabled`, `disabled` or `non-set`. `Non-set` sets default permissions according to `ACL Strict Mode` checkbox in `Administration/Settings` menu.
- `Create` - rights to create data in this entity. Simply select yes or no.
- `Read` - rights to read data in this entity. You can set all data in the entity to be readable, no data, only own data or account data (see square on the picture below). Account is all the data owned by n account that gave the rights.
- `Edit` - rights to edit data in this entity. You can set all data in the entity to be editable, no data, only own data or account data. 
- `Delete` - rights to delete data in this entity. You can set all data in the entity to be deletable, no data, only own data or account data. 
- `Stream` - access to the panel that shows changes in the data and who changed.

The example for our case is on the picture below:

![discussion-button](../_assets/admin-guide/Assets_Portal/Assets_Portal4.png)

Now when role is set we can select it for our portal.

![discussion-button](../_assets/admin-guide/Assets_Portal/Assets_Portal5.png)

> Please note, that one role can be selected for many portals (if they have same rights). If you have a role already set you can select it right away.

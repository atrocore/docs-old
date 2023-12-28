# Advanced data types

"Advanced data types" module allows to add new data types for fields and attributes and adds a new entity type "Relationship".

Included additional data types:

## Alias

Alias – allows to link the attribute value to another attribute value. If the aliased attribute have a value in different scope, the global value will be selected per default. If no global value is available the system will take the value of the first avaiable channel-specific value.

This attribute type should be used if you need to trasfer to some external system, eg some marketplace, your existing attribute values with a different attribute name/code etc. You have an attribute with a code "hat_size" and it needs to be transfered to the amazon marketplace with a code "headdress_size" and maybe a different name.

## Relation entity type

When you create a many-to-many relationship between two entities, an entity of type Relation is automatically created in the entity manager. The entity name is formed by combining the names of the two entities that form it. By default, the entity has two fields of the link type, which refer to the related base (or hieararchy) entities, as well as the fields id, created/modify at and created/modify by. The Advanced Data Types module provides the ability to edit, configure entities of type Relation and display it as a menu item. If you have this module installed, you can perform the same actions on a Relation entity as you would on a base or hierarchy entity. You can assign additional properties to Relation entity: add new fields, change labels, select Text Filter Fields, Default Order and create new links with other entities.

A good example could be the entity "Product Channels", which is included in the PIM module. This entity links the entities "Products" and "Channels", so that multiple products can be linked with multiple channels. Additionally for the entity "Product Channels" you have the possibility to activate/deactivate some product for a channel. This checkbox is an additional property for a relation "Product Channels". The Admin can also add any additional properties, if needed.

To find, create and edit entity you can go to `Administration / Entities` page. To create entity press `Create entity` button. To edit existing one select the entity and press `Edit` button.

![Create an entity](_assets/advanced-data-types/creating-assets.png)

### Adding new relations

To add a new relation for your entity of type "Relationship"  go to `Administration / Entity` and press `Relationships`. You will see all relations of this entity. Some relationships are generated automatically, you cannot edit or delete them. They are needed for this entity type. To add a new Relationship press `Create link`.

![a new relation](_assets/advanced-data-types/a-new-relation.png)

For entity of type Relation it is possible to create only many-to-one link with another entity.

### Adding new fields

To add additional fields for the entity of type "Relation" go to `Administration / Entity` and press `Fields` for your entity. You see all the fields that this entity has. Some fields are generated automatically, you cannot edit or delete them. To add a new field click on `Add field` and choose the type for your new field.

![additional fields](_assets/advanced-data-types/additional-fields.png)

### Setting permissions for an entity of type Relation

An entity of type relation inherits the permissions from the two entities it consists of. That is, if the user has permission to create, read and edit the ProductChannel entity, but editing is prohibited for one or both entities (Channel and Product), then the user will not be able to edit the ProductChannel entity either. Thus, in order to have permission to perform some action with an entity of the Relation type, the user must be allowed this action for both the entities that form it, as well as for the Relation entity itself.

To configure permissions for a specific user, you need to add a role to the user and configure the permissions for that role in `Administration / Roles`

![permissions settings](_assets/advanced-data-types/permissions.png)

# Ownership Inheritance

This module allows you to configure the inheritance of the ownership information for selected entities. This functionality is particularly useful for larger companies that want more flexible user access for certain entities.

The ownership information such as assigned user, owner, assigned teams is important for determining the authorization and access levels in the system. These can be activated or deactivated for each entity.

Thanks to this module, it is possible to configure inheritance of data records’ ownership information from the ownership information of higher-level entities in the system. This saves time when entering ownership information and still ensures that users have the necessary permissions.

## Administrator functions
Currently, the administrator can set up inheritance rules for the entities Products and Product Attribute Values.

![ownership-inheritance-configuration](./_assets/ownership-inheritance/ownership-inheritance-configuration.png)

### Inheritance of ownership information for a product
The assigned owner of a product can be inherited:
- from the product catalog
- from the product family.

The owner of a product can be inherited:
- from the product catalog
- from the product family.

The assigned teams of a product can be inherited:
- from the product catalog
- from the product family.

### Inheritance of owner information for a product attribute value

The assigned owner of a product attribute value can be inherited:
- from the product
- from the attribute.

The owner of a product attribute value can be inherited:
- from the product
- from the attribute.

The assigned teams of a product attribute value can be inherited:
- from the product
- from the attribute.

You can also overwrite the existing ownership information by applying the configured inheritance to all existing records. Click the respective checkbox “Overwrite existing data” to do this.

![overwrite](./_assets/ownership-inheritance/ownership-inheritance-configuration-with-overwrite.png)

## User functions
No additional actions are required from users.

Once a product or a product attribute value has been created, you need no longer enter the owner, the assigned user or the assigned teams yourself, because these values ​​are automatically assigned in accordance with the preconfigured inheritance rules.

### Example 1:
The system is configured so that the owner of a product is inherited from the product family. If this owner is changed for the product family, the owner of the affected product is also automatically changed.

### Example2:
If the inheritance of the owner of the product is set up for the product attribute values, each product attribute value assigned to the product will automatically receive the same owner as the product itself. This means that if a user has access to a product data set, he also automatically has access to all values of its attributes.

Inheritance can be switched off. To do this, click on the chain icon. If the inheritance is switched off, you can specify the owner information manually. So that the changes in the superordinate data records lead to automatic changes to the owner information for the products or product attribute values. The inheritance of the owner information should be switched on again.


# Advanced Classification

The "Advanced Classification" module allows the user to create product family hierarchies. A product family describes products of same kind with common attributes (features). This module facilitates the product family creation and management as well as product filtering. The module enables you to manage product families that are similar but slightly differ from each other. 

## Product family creation and configuration

To create a new product family go to the `Products / Product family` and click `Create product family` button.

![Export feed cfg file](_assets/advanced-classification/create_product_family_with_parent.png)

- **Active** – select this checkbox to activate the product family.
- **Name** – specify the product family name. You may also add its translation in the corresponding fields. 
- **Code** - this field should be unique for each product family.
- **Parent** - define the parent element from which this product family will be inherited.

To add fields for additional languages you need to add these additional languages here: "Administration / Languages".

## Product family editing

In order to view the product family details, click on its name in the list. Click the `Edit` button if you need to make any changes.

- **Name** – specify the product family name. You may also add its translation in the corresponding fields. To add more fields for different languages go to `Administration / Languages`.
- **Code** - this field should be unique for each product family.
- **Parent** - define the parent element from which this product family will be inherited.

![Export feed cfg file](_assets/advanced-classification/edit_product_family.png)

Below the overview panel you can see children product families, attributes and products which belong to this particular product family. 

All child product families automatically inherit their attribute configuration from the parent product family. These configurations, e.g., whether the attribute is mandatory or not and its scope can still be changed. The inherited attributes are marked with italic font.

![Export feed cfg file](_assets/advanced-classification/inherited_attributes.png)

The `Children` panel is another way to add hierarchical structure to your product family. You may either create a new product family which will be a child to the current one by clicking the `+` icon.

On the `Children` panel you may either create a new product family which will be a child to the current one by clicking the `+` icon
![Export feed cfg file](_assets/advanced-classification/create_new_child.png)

or choose from the existing by clicking the `Select` button in the dropdown menu and choose the corresponding product families from the list. In this case the selected product families will be added to the current product family as its children.
![Export feed cfg file](_assets/advanced-classification/select_product_family_children.png)

## Product family tree

Important! The "Advanced Classification" module enables you to filter your products on the product list page by the product family. On the left panel in the `Product` tab click the dropdown menu and select `Product family`. The tree structure reflecting the product family hierarchy will then be shown. Choose the necessary item, and you're good to go!

![Export feed cfg file](_assets/advanced-classification/sort_by_product_family.png)

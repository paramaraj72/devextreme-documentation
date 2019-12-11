---
type: function(item)
---
---
##### shortDescription
Specifies a function that customizes a form item after it has been created.

##### param(item): dxFormSimpleItem|dxFormGroupItem|dxFormTabbedItem|dxFormEmptyItem
Provides access to the item instance.

---
If you did not define form items using the [items](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/items.md '{basewidgetpath}/Configuration/#items') option, the **Form** widget creates them automatically according to the structure of an object passed to the [formData](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/formData.md '{basewidgetpath}/Configuration/#formData') option. The **customizeItem** option enables you to modify options of each generated item before this item is rendered. Each generated item passed to this function as an argument has a [Simple Item](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/SimpleItem '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/SimpleItem/') structure.

If the **items** option contains definition for form items, you usually do not need to pass a function to the **customizeItem** option because you can customize items before passing them to the **items** option. However, if you assign a function to this option, it will be called for each item. In this case, an item can have structure corresponding to any of the following item types.

- [Simple](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/SimpleItem '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/SimpleItem/')  
 A standard item consisting of a label and an editor widget used to specify a value of the associated data field.

- [Group](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/GroupItem '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/GroupItem/')  
 An item representing a container of other form items.

- [Tabbed](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/TabbedItem '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/TabbedItem/')  
 An item representing a tabbed container of other form items.

- [Empty](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/EmptyItem '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/EmptyItem/')  
 An empty item used to add a space between neighboring form items.
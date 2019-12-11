---
type: template
---
---
##### shortDescription
Specifies an item template that should be used to render this item only.

---
Whether you use a default or a custom template for widget items, you can specify a specific template for a particular item. To do so, set the **template** field for the data source object of this item. The following types of the specified value are available.

- Assign a jQuery object of the template's container.
- Assign a DOM Node of the template's container.
- Assign a function that returns the jQuery object or a DOM Node of the template's container.

[note]The [dxTemplate](/api-reference/10%20UI%20Widgets/Markup%20Components/dxTemplate '/Documentation/ApiReference/UI_Widgets/Markup_Components/dxTemplate/') component can not be used as a **toolbarItems** template .

#####See Also#####
- [template](/api-reference/50%20Common/Object%20Structures/template '/Documentation/ApiReference/Common/Object_Structures/template/')
- [Customize Widget Element Appearance](/concepts/05%20Widgets/zz%20Common/05%20UI%20Widgets/30%20Customize%20Widget%20Element%20Appearance '/Documentation/Guide/Widgets/Common/UI_Widgets/Customize_Widget_Element_Appearance/')
- [Customize Widget Element Appearance - MVVM Approach](/concepts/05%20Widgets/zz%20Common/05%20UI%20Widgets/35%20Customize%20Widget%20Element%20Appearance%20-%20MVVM%20Approach '/Documentation/Guide/Widgets/Common/UI_Widgets/Customize_Widget_Element_Appearance_-_MVVM_Approach/')
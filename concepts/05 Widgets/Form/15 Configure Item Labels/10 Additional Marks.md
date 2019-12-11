[Simple items](/concepts/05%20Widgets/Form/05%20Configure%20Simple%20Items '/Documentation/Guide/Widgets/Form/Configure_Simple_Items/') may require a value or may allow a user to skip it. Both types of items can be marked with a symbol or text. Required items are those whose [isRequired](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/SimpleItem/isRequired.md '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/SimpleItem/#isRequired') option is *true*, others are considered optional.

To specify the mark or text for required and optional items, use the [requiredMark](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/requiredMark.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#requiredMark') and [optionalMark](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/optionalMark.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#optionalMark') options. Note that the "optional" mark will not be displayed until you set the [showOptionalMark](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/showOptionalMark.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#showOptionalMark') option to *true*. You can also hide the "required" mark using the [showRequiredMark](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/showRequiredMark.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#showRequiredMark') option.

    <!--JavaScript-->
    $(function() {
        $("#formContainer").dxForm({
            formData: {
                firstName: "John",
                lastName: "Heart",
                position: "CEO"
            },
            items: [
                { dataField: "firstName", isRequired: true },
                { dataField: "lastName", isRequired: true },
                "position"
            ],
            requiredMark: "!",
            optionalMark: "opt",
            showOptionalMark: true
        });
    });

Each label ends with a colon. To hide it, assign *false* to the [showColonAfterLabel](/api-reference/10%20UI%20Widgets/dxForm/1%20Configuration/showColonAfterLabel.md '/Documentation/ApiReference/UI_Widgets/dxForm/Configuration/#showColonAfterLabel') option. Note that you can show/hide a colon for an individual item using the **label** | [showColon](/api-reference/10%20UI%20Widgets/dxForm/5%20Item%20Types/SimpleItem/label/showColon.md '/Documentation/ApiReference/UI_Widgets/dxForm/Item_Types/SimpleItem/label/#showColon') option.

    $(function() {
        $("#formContainer").dxForm({
            formData: {
                firstName: "John",
                lastName: "Heart",
                position: "CEO"
            },
            showColonAfterLabel: false,
            items: ["firstName", "lastName", {
                dataField: "position",
                label: { showColon: true }
            }]
        });
    });

#####See Also#####
- [Form - Configure Item Labels | Location and Alignment](/concepts/05%20Widgets/Form/15%20Configure%20Item%20Labels/05%20Location%20and%20Alignment '/Documentation/Guide/Widgets/Form/Configure_Item_Labels/Location_and_Alignment/')
- [Form - Change Item Options at Runtime](/concepts/05%20Widgets/Form/20%20Change%20Options%20at%20Runtime/10%20Item%20Options.md '/Documentation/Guide/Widgets/Form/Change_Options_at_Runtime/Item_Options/')
- [Form - Change Editor Options at Runtime](/concepts/05%20Widgets/Form/20%20Change%20Options%20at%20Runtime/15%20Editor%20Options.md '/Documentation/Guide/Widgets/Form/Change_Options_at_Runtime/Editor_Options/')
- [Form - Configure Simple Items](/concepts/05%20Widgets/Form/05%20Configure%20Simple%20Items '/Documentation/Guide/Widgets/Form/Configure_Simple_Items/')
- [Form Demos](https://js.devexpress.com/Demos/WidgetsGallery/#demo/forms_and_multi-purpose-form-grouped_fields)
- [Form API Reference](/api-reference/10%20UI%20Widgets/dxForm '/Documentation/ApiReference/UI_Widgets/dxForm/')

[tags]form, required, optional, mark, colon
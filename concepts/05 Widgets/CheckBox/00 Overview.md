The **CheckBox** is a small box, which when selected by the end user, shows that a particular feature has been enabled or a specific option has been chosen.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/editors-check_box-overview" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>

The following code adds the **CheckBox** to your page.

    <!--HTML-->
    <div id="checkBoxContainer"></div>
     
<!---->
 
    <!--JavaScript-->
    $(function() {
        $("#checkBoxContainer").dxCheckBox({
            text: "Check me",
            value: undefined
        });
    });

The **CheckBox** widget can have the following states: checked (the **value** option is _true_), unchecked (**value** is _false_), undetermined (**value** is _undefined_).

#####See Also#####
- [Widget Basics - jQuery](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/')
- [Widget Basics - AngularJS](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/')
- [Widget Basics - Knockout](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/')
- [CheckBox - Handle the Value Change Event](/concepts/05%20Widgets/CheckBox/10%20Handle%20the%20Value%20Change%20Event.md '/Documentation/Guide/Widgets/CheckBox/Handle_the_Value_Change_Event')
- [CheckBox - Keyboard Support](/concepts/05%20Widgets/CheckBox/20%20Keyboard%20Support.md '/Documentation/Guide/Widgets/CheckBox/Keyboard_Support')
- [CheckBox API Reference](/api-reference/10%20UI%20Widgets/dxCheckBox '/Documentation/ApiReference/UI_Widgets/dxCheckBox/')

[tags]check box, checkBox, editor, overview
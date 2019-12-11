---
hidden: 
module: ui/drop_down_menu
export: default
inherits: ..\Widget\Widget.md
---
---
##### lib
dx.mobile.js, dx.web.js, dx.viz-web.js, dx.all.js

##### shortDescription
A drop-down menu widget.

---
The **DropDownMenu** widget is a UI element (a button or a toolbar item) that displays a drop-down menu when clicked.

You can create the widget using one of the following approaches.

- [**jQuery**](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div id="dropDownMenu"></div>

        <!--JavaScript-->
        $("#dropDownMenu").dxDropDownMenu({
            dataSource: dropDownMenuData,
            buttonText: 'Show menu',
            buttonIcon: 'menu'
        });

- [**Angular**](/concepts/00%20Getting%20Started/15%20Widget%20Basics%20-%20Angular/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Angular/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <dx-drop-down-menu
            [dataSource]="dropDownMenuData"
            buttonText="Show menu"
            buttonIcon="menu">
        </dx-drop-down-menu>

- [**AngularJS**](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div dx-drop-down-menu="{
            dataSource: dropDownMenuData,
            buttonText: 'Show menu',
            buttonIcon: 'menu'
        }"></div>

- [**Knockout**](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div data-bind="dxDropDownMenu: {
            dataSource: dropDownMenuData,
            buttonText: 'Show menu',
            buttonIcon: 'menu'
        }"></div>

Note that DevExtreme widgets require you to link the jQuery library to your application. If you use the Knockout or AngularJS approach, the Knockout or AngularJS library is also required. For detailed information on linking these libraries to your project, refer to the topics in the [Installation](/concepts/00%20Getting%20Started/01%20Installation/01%20Local%20Scripts.md '/Documentation/Guide/Getting_Started/Installation/Local_Scripts/') section.
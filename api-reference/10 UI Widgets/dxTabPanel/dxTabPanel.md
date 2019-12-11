---
module: ui/tab_panel
export: default
inherits: ..\dxMultiView\dxMultiView.md
---
---
##### widgettree
dataSource: [
        {
            title: "Info",
            text: "John Smith, 1986"
        },
        {
            title: "Contacts",
            text: "phone: (555)555-5555, email: John.Smith@example.com"
        },
        {
            title: "Address",
            text: "CA San Francisco Stanford Ave st."
        }
],
height: 200

##### lib
dx.mobile.js, dx.web.js, dx.viz-web.js, dx.all.js

##### shortDescription
The **TabPanel** is a widget consisting of the [Tabs](/concepts/05%20Widgets/Tabs/00%20Overview.md '/Documentation/Guide/Widgets/Tabs/Overview/') and [MultiView](/concepts/05%20Widgets/MultiView/00%20Overview.md '/Documentation/Guide/Widgets/MultiView/Overview/') widgets. It automatically synchronizes the selected tab with the currently displayed view and vice versa.

---
You can create the widget using one of the following approaches.

- [**jQuery**](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div id="tabPanel"></div>

        <!--JavaScript-->var tabs = [{
            title: 'Info',
            text: 'This is Info Tab'
        }, {
            title: 'Contacts',
            text: 'This is Contacts Tab'
        }, {
            title: 'Address',
            text: 'This is Address Tab'
        }];
        $(function () {
            $("#tabPanel").dxTabPanel({
                items: tabs
            });
        });

- [**Angular**](/concepts/00%20Getting%20Started/15%20Widget%20Basics%20-%20Angular/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Angular/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <dx-tab-panel [items]="tabs"></dx-tab-panel>

        <!--JavaScript-->
        export class AppComponent {
            tabs = [
                // ...
            ];
        }

- [**AngularJS**](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/Create_and_Configure_a_Widget/')  

        <!--HTML--><div ng-controller="DemoController">
            <div dx-tab-panel="{
                items: tabs
            }"></div>
        </div>

        <!--JavaScript-->angular.module('DemoApp', ['dx'])
            .controller("DemoController", function ($scope) {
                $scope.tabs = [
                    // ...   
                ];
            });

- [**Knockout**](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div data-bind="dxTabPanel: {
            items: tabs
        }"></div>

        <!--JavaScript-->var viewModel = {
            tabs: [
                // ...
            ]
        };
        ko.applyBindings(viewModel);

- [**ASP.NET MVC Wrappers**](/concepts/35%20ASP.NET%20MVC%20Wrappers/20%20Fundamentals/05%20Creating%20a%20Widget.md '/Documentation/Guide/ASP.NET_MVC_Wrappers/Fundamentals/#Creating_a_Widget')

        <!--Razor C#-->@(Html.DevExtreme().TabPanel()
            .ID("tabPanel")
            .Items(items => {
                items.Add().Title("Info").Text("This is Info Tab");
                items.Add().Title("Contacts").Text("This is Contacts Tab");
                items.Add().Title("Address").Text("This is Address Tab");
            })
        )

        <!--Razor VB-->@(Html.DevExtreme().TabPanel() _
            .ID("tabPanel") _
            .Items(Sub(items)
                items.Add().Title("Info").Text("This is Info Tab")
                items.Add().Title("Contacts").Text("This is Contacts Tab")
                items.Add().Title("Address").Text("This is Address Tab")
            End Sub)
        )

Note that DevExtreme widgets require you to link the jQuery library to your application. If you use the Knockout or AngularJS approach, the Knockout or AngularJS library is also required. For detailed information on linking these libraries to your project, refer to the topics in the [Installation](/concepts/00%20Getting%20Started/01%20Installation/01%20Local%20Scripts.md '/Documentation/Guide/Getting_Started/Installation/Local_Scripts/') section.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/navigationtabpaneltabpaneltabpanel/" class="button orange small fix-width-155" style="margin-right:5px;" target="_blank">View Demo</a>
<a href="http://www.youtube.com/watch?v=SyGIlFZY_S0&list=PL8h4jt35t1wjGvgflbHEH_e3b23AA30-z&index=42" class="button orange small fix-width-155" target="_blank">Watch Video</a>

#####See Also#####
- [TabPanel - Overview](/concepts/05%20Widgets/TabPanel/00%20Overview.md '/Documentation/Guide/Widgets/TabPanel/Overview/')
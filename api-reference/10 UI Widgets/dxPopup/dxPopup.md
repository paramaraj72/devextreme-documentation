---
module: ui/popup
export: default
inherits: ..\dxOverlay\dxOverlay.md
---
---
##### widgettree
visible: true

##### lib
dx.mobile.js, dx.web.js, dx.viz-web.js, dx.all.js

##### shortDescription
The **Popup** widget is a pop-up window overlaying the current view.

---
You can create the widget using one of the following approaches.

- [**jQuery**](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div id="popup">
            <p>Popup content</p>
        </div>

        <!--JavaScript-->$(function () {
            $("#popup").dxPopup({
                title: 'Popup Title',
                visible: true
            });
        });

- [**Angular**](/concepts/00%20Getting%20Started/15%20Widget%20Basics%20-%20Angular/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Angular/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <dx-popup
            title="Popup Title"
            [(visible)]="isPopupVisible">
                <p>Popup content</p>
        </dx-popup>

        <!--JavaScript-->
        export class AppComponent {
            isPopupVisible = true;
        }

- [**AngularJS**](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/Create_and_Configure_a_Widget/')  

        <!--HTML--><div ng-controller="DemoController">
            <div dx-popup="{
                title: 'Popup Title',
                bindingOptions: {
                    visible: 'isPopupVisible'
                }
            }">
                <p>Popup content</p>
            </div>
        </div>

        <!--JavaScript-->angular.module('DemoApp', ['dx'])
            .controller('DemoController', function DemoController($scope) {
                $scope.isPopupVisible = true;
            });

- [**Knockout**](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout/01%20Create%20and%20Configure%20a%20Widget.md '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/Create_and_Configure_a_Widget/')  

        <!--HTML-->
        <div data-bind="dxPopup: {
            title: 'Popup Title',
            visible: isPopupVisible
        }"></div>

        <!--JavaScript-->var viewModel = {
            isPopupVisible: ko.observable(true)
        };
        ko.applyBindings(viewModel);

- [**ASP.NET MVC Wrappers**](/concepts/35%20ASP.NET%20MVC%20Wrappers/20%20Fundamentals/05%20Creating%20a%20Widget.md '/Documentation/Guide/ASP.NET_MVC_Wrappers/Fundamentals/#Creating_a_Widget')

        <!--Razor C#-->@(Html.DevExtreme().Popup()
            .ID("popover")
            .Title("Popup Title")
            .Visible(true)
            .ContentTemplate(@<text>
                <p>Popup content</p>
            </text>)
        )

        <!--Razor VB-->@Code
            Html.DevExtreme().Popup() _
                .ID("popover") _
                .Title("Popup Title") _
                .Visible(True) _
                .ContentTemplate(Sub()
                    @<text>
                        <p>Popup content</p>
                    </text>
                End Sub).Render()
        End Code

Note that DevExtreme widgets require you to link the jQuery library to your application. If you use the Knockout or AngularJS approach, the Knockout or AngularJS library is also required. For detailed information on linking these libraries to your project, refer to the topics in the [Installation](/concepts/00%20Getting%20Started/01%20Installation/01%20Local%20Scripts.md '/Documentation/Guide/Getting_Started/Installation/Local_Scripts/') section.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/dialogsandnotificationspopuppopuppopup/" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>

#####See Also#####
- [Popup - Overview](/concepts/05%20Widgets/Popup/00%20Overview.md '/Documentation/Guide/Widgets/Popup/Overview/')
- [Popup - Show and Hide the Popup](/concepts/05%20Widgets/Popup/10%20Show%20and%20Hide%20the%20Popup '/Documentation/Guide/Widgets/Popup/Show_and_Hide_the_Popup/')
---
default: 'month'
acceptValues: 'month' | 'year' | 'decade' | 'century'
type: String
---
---
##### shortDescription
Specifies the [maximum zoom level](/api-reference/10%20UI%20Widgets/dxCalendar/1%20Configuration/maxZoomLevel.md '/Documentation/ApiReference/UI_Widgets/dxCalendar/Configuration/#maxZoomLevel') of a [calendar](/api-reference/10%20UI%20Widgets/dxCalendar '/Documentation/ApiReference/UI_Widgets/dxCalendar/'), which is used to pick the date.

---
The zoom level ascends from 'month' to 'century' ('month'->'year'->'decade'->'century').

The option makes sense only if the [pickerType](/api-reference/10%20UI%20Widgets/dxDateBox/1%20Configuration/pickerType.md '/Documentation/ApiReference/UI_Widgets/dxDateBox/Configuration/#pickerType') option is set to 'calendar'.

When configuring the widget using [ASP.NET MVC Wrappers](/concepts/35%20ASP.NET%20MVC%20Wrappers/20%20Fundamentals '/Documentation/Guide/ASP.NET_MVC_Wrappers/Fundamentals/'), specify this option using the `CalendarZoomLevel` enum. This enum accepts the following values: `Month`, `Year`, `Decade` and `Century`.
---
default: 'row'
acceptValues: 'row' | 'col'
type: String
---
---
##### shortDescription
Specifies the direction of item positioning in the widget.

---
If the option value is *"row"*, items are located side by side. If the value is *"col"*, items are located one under another.

When configuring the widget using [ASP.NET MVC Wrappers](/concepts/35%20ASP.NET%20MVC%20Wrappers/20%20Fundamentals '/Documentation/Guide/ASP.NET_MVC_Wrappers/Fundamentals/'), specify this option using the `BoxDirection` enum. This enum accepts the following values: `Row` and `Col`.
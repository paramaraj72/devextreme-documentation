---
module: events/click
type: eventType
---
---
##### shortDescription
Raised when the element is clicked.

##### param(event): jQuery.event
The standard jQuery event argument. For the information on event handler arguments, refer to the <a href="/Documentation/ApiReference/UI_Widgets/UI_Events/">UI Events introduction</a>.

---
The native **click** event waits 300 ms after the element was clicked. This time interval is required to wait for the second click. If a user clicks the element one more time during this time span, the **dblclick** event is raised instead of the **click**. The **dxclick** event is raised immediately after the element is clicked.
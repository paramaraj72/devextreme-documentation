---
EventForAction: ..\4 Events\cellPrepared.md
default: null
type: function(e)
---
---
##### shortDescription
A handler for the [cellPrepared](/api-reference/10%20UI%20Widgets/dxPivotGrid/4%20Events/cellPrepared.md '/Documentation/ApiReference/UI_Widgets/dxPivotGrid/Events/#cellPrepared') event.

##### param(e): Object
Information about the event.

##### field(e.component): Object
The widget <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxPivotGrid/Methods/#instance">instance</a>.

##### field(e.element): jQuery
The widget's container.

##### field(e.model): Object
Data that is available for binding against the element. Available only in the Knockout approach.

##### field(e.area): String
The <a href="/Documentation/16_2/ApiReference/Data_Layer/PivotGridDataSource/Configuration/fields/#area">area</a> to which the prepared cell belongs.

##### field(e.cellElement): jQuery
The container of the prepared cell.

##### field(e.cell): PivotGridCell
The cell object.

##### field(e.rowIndex): Number
The position of a cell's row.

##### field(e.columnIndex): Number
The position of a cell's column.

---
The **cellPrepared** event fires after a cell has been rendered. When implementing a handling function for this event, use the object passed to this function as its parameter. Among the fields of this object, you can find data relating to the prepared cell.
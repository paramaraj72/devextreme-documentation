---
EventForAction: ..\4 Events\cellHoverChanged.md
default: null
type: function(e)
---
---
##### shortDescription
A handler for the [cellHoverChanged](/api-reference/10%20UI%20Widgets/dxDataGrid/4%20Events/cellHoverChanged.md '/Documentation/ApiReference/UI_Widgets/dxDataGrid/Events/#cellHoverChanged') event.

##### param(e): Object
Information about the event.

##### field(e.component): Object
The widget <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxDataGrid/Methods/#instance">instance</a>.

##### field(e.element): jQuery
The widget's container.

##### field(e.model): Object
Data that is available for binding against the element. Available only in the Knockout approach.

##### field(e.eventType): String
Identifies whether the cell has been hovered over or hovered out. This field equals either <i>"mouseover"</i> or <i>"mouseout"</i>.

##### field(e.data): Object
The object of the data source presented by the row to which the current cell belongs.

##### field(e.key): any
The key of the row. If a field providing keys is not specified in a <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxDataGrid/Configuration/#dataSource">data source</a>, the whole data object is considered the key.

##### field(e.value): any
The value of the current cell as it is specified in the data source.

##### field(e.text): String
The value of the current cell in a string format. Use this field to get the value with an applied <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxDataGrid/Configuration/columns/#format">format</a>.

##### field(e.displayValue): String
The value displayed by the current cell. Differs from the <b>value</b> field only when the column to which the current cell belongs uses <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxDataGrid/Configuration/columns/lookup/">lookup</a>.

##### field(e.columnIndex): Number
The index of the column to which the current cell belongs. For more information on how this index is calculated, refer to the <a href="/Documentation/16_2/Guide/Widgets/DataGrid/Visual_Elements/#Grid_Columns/Calculating_the_Column_Index">Calculating the Column Index</a> topic.

##### field(e.rowIndex): Number
The <i>visible</i> index of the row to which the current cell belongs. When you have several pages in a grid, grid rows are indexed beginning with 0 on each page. Note that <a href="/Documentation/16_2/Guide/Widgets/DataGrid/Visual_Elements/#Group_Rows">group cells</a> are also counted as rows and, thus, have row indexes. For further information about row indexes, see the <a href="/Documentation/16_2/Guide/Widgets/DataGrid/Visual_Elements/#Grid_Rows">Grid Rows</a> topic.

##### field(e.column): Object
The <a href="/Documentation/16_2/ApiReference/UI_Widgets/dxDataGrid/Configuration/columns/">settings of the column</a> to which the current cell belongs.

##### field(e.rowType): String
The type of the row to which the current cell belongs. This field equals <i>'data'</i> for <a href="/Documentation/16_2/Guide/Widgets/DataGrid/Visual_Elements/#Grid_Rows">ordinary rows</a> or <i>'group'</i> for <a href="/Documentation/16_2/Guide/Widgets/DataGrid/Visual_Elements/#Group_Rows">group rows</a>. Use this field to distinguish rows by type.

##### field(e.cellElement): jQuery
The element of the hovered cell.

##### field(e.row): dxDataGridRowObject
The settings of the row to which the cell belongs.

---
The **cellHoverChanged** event fires when the hover state of a grid cell is changed. When implementing a handling function for this event, use the object passed to this function as its parameter. Among the fields of this object, you can find data relating to the cell whose hover state has been changed. For example, to identify whether a cell has been hovered over or hovered out, check the value of the **eventType** field.
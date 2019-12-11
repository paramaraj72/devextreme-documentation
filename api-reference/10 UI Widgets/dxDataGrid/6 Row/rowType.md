---
type: String
---
---
##### shortDescription
The type of the row.

---
This field can have one of the following values.

- *"data"* - for [rows representing data objects](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/020%20Grid%20Rows.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Grid_Rows')
- *"detail"* - for the row containing the detail section in the [master-detail interface](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/150%20Master-Detail%20Interface.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Master-Detail_Interface')
- *"detailAdaptive" - for the row containing in the detail section of the [adaptive column](/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Gid_Columns/Command_Columns)
- *"group"* - for [group rows](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/100%20Group%20Rows '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Group_Rows')
- *"groupFooter"* - for the row displayed in the [group footer](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/100%20Group%20Rows/20%20Group%20Summary.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Group_Rows/Group_Summary')
- *"header"* - for the [header row](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/010%20Grid%20Columns/050%20Configuring%20Column%20Headers.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Grid_Columns/Configuring_Column_Headers')
- *"filter"* - for the [filter row](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/070%20Filter%20Row.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Filter_Row')
- *"totalFooter"* - for the row containing the [total summary](/concepts/05%20Widgets/DataGrid/001%20Visual%20Elements/140%20Total%20Summary.md '/Documentation/Guide/Widgets/DataGrid/Visual_Elements/#Total_Summary')

[note]Available row properties depend on the row type. For example, the [data](/api-reference/10%20UI%20Widgets/dxDataGrid/6%20Row/data.md '/Documentation/ApiReference/UI_Widgets/dxDataGrid/Row/#data') and [key](/api-reference/10%20UI%20Widgets/dxDataGrid/6%20Row/key.md '/Documentation/ApiReference/UI_Widgets/dxDataGrid/Row/#key') properties are undefined for *header*, *filter* and *totalFooter* rows, but have values for the other row types. To get exhaustive information on the particular property, refer to its description.
---
id: dxTreeListRowObject.key
type: any
---
---
##### shortDescription
The row's key. Available if [rowType](/api-reference/10%20UI%20Components/dxTreeList/6%20Row/rowType.md '/Documentation/ApiReference/UI_Components/dxTreeList/Row/#rowType') is *"data"*, *"detail"* or *"detailAdaptive"*.

---
Keys are provided by the [key](/api-reference/30%20Data%20Layer/Store/1%20Configuration/key.md '/Documentation/ApiReference/Data_Layer/CustomStore/Configuration/#key') field of the store that underlies the [dataSource](/api-reference/10%20UI%20Components/dxTreeList/1%20Configuration/dataSource.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/#dataSource'). Alternatively, you can set the UI component's [keyExpr](/api-reference/10%20UI%20Components/dxTreeList/1%20Configuration/keyExpr.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/#keyExpr') property. With hierarchical data, keys can be generated automatically if **key** and **keyExpr** are not set.
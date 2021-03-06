---
id: dxSankey.Options.onNodeClick
type: function(e) | String
default: null
EventForAction: dxSankey.nodeClick
notUsedInTheme: 
---
---
##### shortDescription
A function that is executed when a sankey node is clicked or tapped.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): dxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.model): Object
The model data. Available only if you use Knockout.

##### field(e.target): dxSankeyNode
The [Node](/api-reference/10%20UI%20Components/dxSankey/6%20Node '/Documentation/ApiReference/UI_Components/dxSankey/Node/') object.

---
#####See Also#####
- [node](/api-reference/10%20UI%20Components/dxSankey/1%20Configuration/node '/Documentation/ApiReference/UI_Components/dxSankey/Configuration/node/')
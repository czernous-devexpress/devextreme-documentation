---
id: BaseGauge.subvalues(subvalues)
---
---
##### shortDescription
Updates subvalues.

##### param(subvalues): Array<Number>
New subvalues.

---
Use this method to change gauge subvalues at runtime.

[note]It is necessary to set the [subvalues](/api-reference/10%20UI%20Components/BaseGauge/1%20Configuration/subvalues.md '{basewidgetpath}/Configuration#subvalues') property in order to use the **subvalues(subvalues)** method. Set this property to an empty array, in case you don't need to show subvalues initially.

#include common-demobutton-named with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Gauges/ValueIndicatorsAPI/",
    name: "Value Indicators API"
}
#include common-demobutton-named with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Gauges/VariableNumberOfSubvalueIndicators/",
    name: "Subvalue Indicators"
}

#####See Also#####
#include common-link-callmethods
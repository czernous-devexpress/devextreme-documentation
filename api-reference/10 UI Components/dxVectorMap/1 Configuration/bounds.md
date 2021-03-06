---
id: dxVectorMap.Options.bounds
type: Array<Number>
default: undefined
notUsedInTheme: 
---
---
##### shortDescription
Specifies the positioning of a map in geographical coordinates.

---
When you need to display only a specific region on a map, specify the geographical coordinates of this region using the **bounds** property. Assign an array of four values to this property. These values represent geographical coordinates in the following format: *[minLongitude, maxLatitude, maxLongitude, minLatitude]* with the default range of **longitude** [-180, 180] and **latitude** [-90, 90]. See the image below to review how these values are applied to a map.

![ChartMargin ChartJS](/images/ChartJS/VectorMapBounds.png)

If your [dataSource](/api-reference/10%20UI%20Components/dxVectorMap/1%20Configuration/layers/dataSource.md '/Documentation/ApiReference/UI_Components/dxVectorMap/Configuration/layers/#dataSource') contains coordinates in a different range, implement a [custom projection](https://js.devexpress.com/Demos/WidgetsGallery/Demo/VectorMap/CustomProjection).

[note] Specifying the **bounds** property with the { minLon: *minLongitude*, maxLat: *maxLatitude*, maxLon: *maxLongitude*, minLat: *minLatitude* } object is now <font color="red">deprecated</font>.
---
id: dxPolarChartSeriesTypes.CommonPolarChartSeries.hoverStyle
type: Object
---
---
##### shortDescription
An object defining configuration properties for a hovered series.

##### propertyOf
dxPolarChartSeriesTypes.areapolarseries,dxPolarChartSeriesTypes.barpolarseries,dxPolarChartSeriesTypes.stackedbarpolarseries,dxPolarChartSeriesTypes.linepolarseries

---
To set a custom 'hover' style for all series at once, use the **hoverStyle** object within the **commonSeriesSettings** configuration object.

If you have several series of one type, you can set hover style properties to the values specific to this type using the corresponding object (**area**, **line** or another) within the **commonSeriesSettings** configuration object. The values that are set within series-type-specific configuration objects override the corresponding common values.

In case you have to set a hover style property for an individual series, use the **hoverStyle** object within the series object of the [series](/api-reference/10%20UI%20Components/dxPolarChart/1%20Configuration/series '/Documentation/ApiReference/UI_Components/dxPolarChart/Configuration/series/') array. The values that are set individually override corresponding common values.
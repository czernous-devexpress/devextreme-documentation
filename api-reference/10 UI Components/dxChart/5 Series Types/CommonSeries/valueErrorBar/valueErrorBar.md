---
id: dxChartSeriesTypes.CommonSeries.valueErrorBar
type: Object
---
---
##### shortDescription
Configures error bars.

##### propertyOf
dxChartSeriesTypes.AreaSeries,dxChartSeriesTypes.BarSeries,dxChartSeriesTypes.LineSeries,dxChartSeriesTypes.ScatterSeries,dxChartSeriesTypes.SplineAreaSeries,dxChartSeriesTypes.StepAreaSeries,dxChartSeriesTypes.StepLineSeries

---
Error bars are used on charts to indicate an error or an uncertainty in a reported measurement. They give a general idea of how precise the measurement is.

![DevExtreme HTML5 Charts ErrorBars](/images/ChartJS/visual_elements/error_bars.png)

Error bars can be generated either from concrete or calculated values. To generate one error bar, two values, high and low, are needed. If the [data source](/api-reference/10%20UI%20Components/BaseChart/1%20Configuration/dataSource.md '/Documentation/ApiReference/UI_Components/dxChart/Configuration/#dataSource') of your chart provides concrete high and low values, assign the required data source fields to the **highValueField** and **lowValueField** properties.

Alternatively, error bar values can be calculated according to an algorithm. In this case, choose the required algorithm using the **type** property, and specify the value to be used in calculation using the **value** property.

[note]Error bars are available for axes of the numeric [type](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/argumentAxis/type.md '/Documentation/ApiReference/UI_Components/dxChart/Configuration/argumentAxis/#type') only.

#include common-demobutton with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Charts/ErrorBars/"
}
---
id: dxChartSeriesTypes.CommonSeries.sizeField
type: String
default: 'size'
---
---
##### shortDescription
Specifies which data source field provides size values for bubbles. Required by and applies only to *bubble* series.

##### propertyOf
dxChartSeriesTypes.BubbleSeries

---
Each point in a bubble series has an argument, a regular value and a size value. Arguments are provided by the **argumentField**; regular values are provided by the **valueField**; size values are provided by the **sizeField**.

Size values do not specify the real sizes of bubbles directly, they only define the sizes of bubbles in relation to each other. Apart from a size value, the real, pixel-measured size of a bubble depends on the [minBubbleSize](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/minBubbleSize.md '/Documentation/ApiReference/UI_Components/dxChart/Configuration/#minBubbleSize') and [maxBubbleSize](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/maxBubbleSize.md '/Documentation/ApiReference/UI_Components/dxChart/Configuration/#maxBubbleSize') values and the size of the [pane](/concepts/05%20UI%20Components/Chart/40%20Panes/00%20Overview.md '/Documentation/Guide/UI_Components/Chart/Panes/Overview/').

Commonly, a chart contains several series, and many of them have the same size field. In this case, assign the name of this field to the **sizeField** property of the [commonSeriesSettings](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/commonSeriesSettings '/Documentation/ApiReference/UI_Components/dxChart/Configuration/commonSeriesSettings/') object. If a series must have a unique size field, specify the same property, but do so in the series object within the [series](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/series '/Documentation/ApiReference/UI_Components/dxChart/Configuration/series/') array.
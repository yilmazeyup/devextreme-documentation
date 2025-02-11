---
id: dxBarGauge.Options.tooltip.customizeTooltip
type: function(scaleValue)
default: undefined
---
---
##### shortDescription
Allows you to change tooltip appearance.

##### param(scaleValue): Object
Information on the bar value.

##### field(scaleValue.index): Number
A zero-based index of the hovered bar. The closer this bar is to the gauge's center, the greater its index.

##### field(scaleValue.value): Number
The raw value.

##### field(scaleValue.valueText): String
The [formatted](/api-reference/10%20UI%20Components/BaseWidget/1%20Configuration/tooltip/format.md '/Documentation/ApiReference/UI_Components/dxBarGauge/Configuration/tooltip/#format') value converted to a string.

##### return: Object
The tooltip's text or markup and color.

---
#include dataviz-customize-tooltip-return

#include dataviz-ref-functioncontext

#include common-demobutton with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Gauges/Tooltip/"
}
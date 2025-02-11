---
id: dxPolarChart.Options.onArgumentAxisClick
type: function(e)
default: null
notUsedInTheme: 
---
---
##### shortDescription
A function that is executed when a [label](/concepts/05%20UI%20Components/PolarChart/10%20Visual%20Elements/070%20Axis%20Labels.md '/Documentation/Guide/UI_Components/PolarChart/Visual_Elements/#Axis_Labels') on the [argument axis](/concepts/05%20UI%20Components/PolarChart/10%20Visual%20Elements/050%20Axes/10%20Argument%20Axis.md '/Documentation/Guide/UI_Components/PolarChart/Visual_Elements/#Axes/Argument_Axis') is clicked or tapped.

##### param(e): Object
Information about the event.

##### field(e.argument): Date | Number | String
The clicked label's value.

##### field(e.component): dxPolarChart
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.model): any
The model data. Available only if you use Knockout.

---

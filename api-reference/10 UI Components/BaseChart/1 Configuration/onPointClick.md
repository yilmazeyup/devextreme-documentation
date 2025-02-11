---
id: BaseChart.Options.onPointClick
type: function(e)
default: null
notUsedInTheme: 
---
---
##### shortDescription
A function that is executed when a series point is clicked or tapped.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.model): any
The model data. Available only if you use Knockout.

##### field(e.target): basePointObject
The clicked series point; described in the [Point](/api-reference/10%20UI%20Components/BaseChart/7%20Chart%20Elements/Point '{basewidgetpath}/Chart_Elements/Point/') section.

---
[note]

The [onSeriesClick](/api-reference/10%20UI%20Components/dxChart/1%20Configuration/onSeriesClick.md '{basewidgetpath}/Configuration/#onSeriesClick') function is executed after this function. The following code shows how to prevent this: 

---
##### jQuery

    <!--JavaScript-->
    $(function () {
        $("#{widgetName}Container").dx{WidgetName}({
            // ...
            onPointClick: function (e) {
                e.event.cancel = true;
            }
        });
    });

##### Angular

    <!--TypeScript-->
    import { Dx{WidgetName}Module } from "devextreme-angular";
    // ...
    export class AppComponent {
        cancelSeriesClick (e) {
            e.event.cancel = true;
        }
    }
    @NgModule({
        imports: [
            // ...
            Dx{WidgetName}Module
        ],
        // ...
    })

    <!--HTML--><dx-{widget-name} ...
        (onPointClick)="cancelSeriesClick($event)">
    </dx-{widget-name}>

##### Vue

    <!-- tab: App.vue -->
    <template>
        <Dx{WidgetName} ...
            @point-click="cancelSeriesClick">
        </Dx{WidgetName}>
    </template>

    <script>
    import Dx{WidgetName} from 'devextreme-vue/{widget-name}';

    export default {
        components: {
            Dx{WidgetName}
        },
        methods: {
            cancelSeriesClick (e) {
                e.event.cancel = true;
            }
        }
    }
    </script>

##### React

    <!-- tab: App.js -->
    import React from 'react';

    import {WidgetName} from 'devextreme-react/{widget-name}';

    class App extends React.Component {
        render() {
            return (
                <{WidgetName} ...
                    onPointClick={this.cancelSeriesClick}>
                </{WidgetName}>
            );
        }

        cancelSeriesClick (e) {
            e.event.cancel = true;
        }
    }

    export default App;

---

[/note]

#include common-demobutton-named with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Charts/Selection/",
    name: "Bar Chart"
}
---
id: GridBase.Options.scrolling.rowRenderingMode
acceptValues: 'standard' | 'virtual'
type: String
default: 'standard'
---
---
##### shortDescription
Specifies the rendering mode for loaded rows.

---
Unlike the [mode](/api-reference/10%20UI%20Components/dxDataGrid/1%20Configuration/scrolling/mode.md '{basewidgetpath}/Configuration/scrolling/#mode') property, which defines when to load data for rows, this property defines when to render them. The following rendering modes are available: 

- *"standard"*        
Renders all the loaded rows at once.

- *"virtual"*     
Renders only those rows that get into the viewport. Use this mode if the [pageSize](/api-reference/10%20UI%20Components/GridBase/1%20Configuration/paging/pageSize.md '{basewidgetpath}/Configuration/paging/#pageSize') is large. Rows that are being currently rendered can be shown as gray boxes. If you do not want them to appear, disable the **scrolling**.[renderAsync](/api-reference/10%20UI%20Components/GridBase/1%20Configuration/scrolling/renderAsync.md '{basewidgetpath}/Configuration/scrolling/#renderAsync') property, but this can impact performance.

#include common-demobutton with {
    url: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/DataGrid/RemoteVirtualScrolling/"
}
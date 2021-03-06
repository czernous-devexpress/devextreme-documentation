---
id: dxTreeMap.Options.tile
type: Object
---
---
##### shortDescription
Configures tiles.

---
A tile is a rectangle representing a node that has no children in the current context. Several tiles can be collected into a [group](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/group '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/group/') if the [data source](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/dataSource.md '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/#dataSource') implies a hierarchical structure.

The following list provides an overview of tiles' features that you can configure using the **tile** object.

* **Labels**      
Each tile is identified by a label. Its appearance can be changed using the fields of the [label](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/tile/label '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/tile/label/') object. If the tile's area is too small, the label will be hidden.
* **Color**     
There are several approaches to colorizing the tiles. Refer to the [color](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/tile/color.md '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/tile/#color') property description to find information about all of them.
* **Hover and Selection Styles**        
A tile can be in the [hover](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/hoverEnabled.md '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/#hoverEnabled') or [selected](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/selectionMode.md '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/#selectionMode') state. In these states, its style changes to the one specified by the [hoverStyle](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/tile/hoverStyle '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/tile/hoverStyle/') or [selectionStyle](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/tile/selectionStyle '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/tile/selectionStyle/') object respectively. Along with the tile, its parent group can enter the hover or selected state. To enable this feature, assign **true** to the [interactWithGroup](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/interactWithGroup.md '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/#interactWithGroup') property of the root configuration object.
* **Border's Appearance**     
Specify the fields of the [border](/api-reference/10%20UI%20Components/dxTreeMap/1%20Configuration/tile/border '/Documentation/ApiReference/UI_Components/dxTreeMap/Configuration/tile/border/') object to configure the tile borders.

An object assigned to the **tile** field configures all tiles in the UI component. To customize a specific tile, pass a similar object to the [customize(options)](/api-reference/10%20UI%20Components/dxTreeMap/6%20Node/3%20Methods/customize(options).md '/Documentation/ApiReference/UI_Components/dxTreeMap/Node/Methods/#customizeoptions') method of the node represented by the tile.
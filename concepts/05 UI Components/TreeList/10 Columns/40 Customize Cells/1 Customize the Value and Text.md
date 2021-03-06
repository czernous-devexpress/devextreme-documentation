Use the [customizeText](/api-reference/_hidden/GridBaseColumn/customizeText.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/columns/#customizeText') function to customize the text displayed in cells. Note that this text is not used is not used to sort, filter, and group data or calculate summaries. 

---
##### jQuery

    <!--JavaScript-->
    $(function() {
        $("#treeListContainer").dxTreeList({
            // ...
            columns: [{
                dataField: "Price",
                customizeText: function(cellInfo) {
                    return cellInfo.value + "$";
                }
            }]
        });
    });

##### Angular

    <!--TypeScript-->
    import { DxTreeListModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        priceColumn_customizeText (cellInfo) {
            return cellInfo.value + "$";
        }
    }
    @NgModule({
        imports: [
            // ...
            DxTreeListModule
        ],
        // ...
    })

    <!--HTML-->
    <dx-tree-list ... >
        <dxi-column dataField="Price" [customizeText]="priceColumn_customizeText"></dxi-column>
    </dx-tree-list>

##### Vue

    <!-- tab: App.vue -->
    <template>
        <DxTreeList ... >
            <DxColumn
                data-field="Price"
                :customize-text="priceColumn_customizeText"
            />
        </DxTreeList>
    </template>

    <script>
    import 'devextreme/dist/css/dx.light.css';
    import DxTreeList, {
        DxColumn
    } from 'devextreme-vue/tree-list';

    export default {
        components: {
            DxTreeList,
            DxColumn
        },
        methods: {
            priceColumn_customizeText(cellInfo) {
                return cellInfo.value + '$';
            }
        }
    }
    </script>

##### React

    <!-- tab: App.js -->
    import React from 'react';
    import 'devextreme/dist/css/dx.light.css';
    import TreeList, {
        Column
    } from 'devextreme-react/tree-list';

    const priceColumn_customizeText = (cellInfo) => {
        return cellInfo.value + '$';
    };

    export default function App() {
	    return (
            <TreeList ... >
                <Column
                    dataField="Price"
                    customizeText={priceColumn_customizeText}
                />
            </TreeList>
        );
    }
    
---

To use the text displayed in cells in those data processing operations, specify the [calculateCellValue](/api-reference/_hidden/GridBaseColumn/calculateCellValue.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/columns/#calculateCellValue') function instead. It populates a column with custom values and allows you to create unbound columns - columns that are not bound to any individual data field. In the following example, this function combines full names using data from the **firstName** and **lastName** fields: 

---
##### jQuery

    <!--JavaScript-->
    $(function() {
        $("#treeListContainer").dxTreeList({
            // ...
            columns: [{
                caption: "Full Name",
                calculateCellValue: function (rowData) {
                    return rowData.firstName + " " + rowData.lastName;
                }
            }]
        });
    });

##### Angular

    <!--TypeScript-->
    import { DxTreeListModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        fullNameColumn_calculateCellValue (rowData) {
            return rowData.firstName + " " + rowData.lastName;
        }
    }
    @NgModule({
        imports: [
            // ...
            DxTreeListModule
        ],
        // ...
    })

    <!--HTML-->
    <dx-tree-list ... >
        <dxi-column caption="Full Name" [calculateCellValue]="fullNameColumn_calculateCellValue"></dxi-column>
    </dx-tree-list>

##### Vue

    <!-- tab: App.vue -->
    <template>
        <DxTreeList ... >
            <DxColumn
                caption="Full Name"
                :calculate-cell-value="fullNameColumn_calculateCellValue"
            />
        </DxTreeList>
    </template>

    <script>
    import 'devextreme/dist/css/dx.light.css';

    import DxTreeList, {
        DxColumn
    } from 'devextreme-vue/tree-list';

    export default {
        components: {
            DxTreeList,
            DxColumn
        },
        methods: {
            fullNameColumn_calculateCellValue(rowData) {
                return rowData.firstName + ' ' + rowData.lastName;
            }
        }
    }
    </script>

##### React

    <!-- tab: App.js -->
    import React from 'react';

    import 'devextreme/dist/css/dx.light.css';

    import TreeList, {
        Column
    } from 'devextreme-react/tree-list';

    const fullNameColumn_calculateCellValue = (rowData) => {
        return rowData.firstName + ' ' + rowData.lastName;
    };

    export default function App() {
	    return (
            <TreeList ... >
                <Column
                    caption="Full Name"
                    calculateCellValue={fullNameColumn_calculateCellValue}
                />
            </TreeList>
        );
    }
    
---

Some features are disabled in columns with calculated values. Refer to the [calculateCellValue](/api-reference/_hidden/GridBaseColumn/calculateCellValue.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/columns/#calculateCellValue') description for a list of disabled features and the properties that enable them.
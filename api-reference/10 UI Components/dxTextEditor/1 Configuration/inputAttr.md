---
id: dxTextEditor.Options.inputAttr
type: Object
default: {}
---
---
##### shortDescription
Specifies the attributes to be passed on to the underlying HTML element.

---
---
##### jQuery

    $(function(){
        $("#{widgetName}Container").dx{WidgetName}({
            // ...
            inputAttr: {
                id: "inputId"
            }
        });
    });

##### Angular

    <!--HTML-->
    <dx-{widget-name} ...
        [inputAttr]="{ id: 'inputId' }">
    </dx-{widget-name}>

    <!--TypeScript-->
    import { Dx{WidgetName}Module } from "devextreme-angular";
    // ...
    export class AppComponent {
        // ...
    }
    @NgModule({
        imports: [
            // ...
            Dx{WidgetName}Module
        ],
        // ...
    })

##### Vue

    <!-- tab: App.vue -->
    <template>
        <Dx{WidgetName}
            :input-attr="inputAttr"
        />
    </template>

    <script>
    import 'devextreme/dist/css/dx.light.css';

    import Dx{WidgetName} from 'devextreme-vue/{widget-name}';

    export default {
        components: {
            Dx{WidgetName}
        },
        data() {
            return {
                inputAttr: { id: 'inputId' }
            }
        }
    }
    </script>

##### React

    <!-- tab: App.js -->
    import 'devextreme/dist/css/dx.light.css';

    import {WidgetName} from 'devextreme-react/{widget-name}';

    const inputAttr = { id: 'inputId' };

    export default function App() {
        return (
            <{WidgetName}
                inputAttr={inputAttr}
            />
        );
    }

##### ASP.NET MVC Controls

    <!--Razor C#-->@(Html.DevExtreme().{WidgetName}()
        .InputAttr("id", "inputId")
        // ===== or =====
        .InputAttr(new {
            @id = "inputId"
        })
        // ===== or =====
        .InputAttr(new Dictionary<string, object>() {
            { "id", "inputId" }
        })
    )

    <!--Razor VB-->@(Html.DevExtreme().{WidgetName}() _
        .InputAttr("id", "inputId")
        ' ===== or =====
        .InputAttr(New With {
            .id = "inputId"
        })
        ' ===== or =====
        .InputAttr(New Dictionary(Of String, Object) From {
            { "id", "inputId" }
        })
    )

---
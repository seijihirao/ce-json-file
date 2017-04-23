# \<json-file\>

[![Bower version](https://badge.fury.io/bo/ce-json-file.svg)](https://badge.fury.io/bo/ce-json-file)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/seijihirao/ce-json-file)

Json file reader element

## INSTALL

```
$ bower install --save ce-json-file
```

## IMPORT

```HTML
    <link rel="import" href="../bower_components/ce-json-file/json-file.html">
```

## USING

```HTML
    <ce-json-file
        path="pathto/myfile.json"
        json="{{my_json}}"></ce-json-file>
```

# CustomElements.AppJsonBehavior

Json file reader behavior for polymer

## INSTALL

```
$ bower install --save ce-json-file
```

## IMPORT

```HTML
    <link rel="import" href="../bower_components/ce-json-file/json-file-behavior.html">
```

## USING

```HTML
<dom-module id="x-app">
    <template>
        <div>[[json.name]]</div>
    </template>
    <script>
        Polymer({
            is: "x-app",

            behaviors: [
                CustomElements.AppJsonBehavior
            ],

            properties: {
                file: {
                    value: 'resources.json'
                }
            }
        });
    </script>
</dom-module>
```
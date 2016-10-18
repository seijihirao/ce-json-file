# \<json-file\>

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
    <json-file
        file="pathto/myfile.json"
        json="{{my_json}}"></json-file>
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
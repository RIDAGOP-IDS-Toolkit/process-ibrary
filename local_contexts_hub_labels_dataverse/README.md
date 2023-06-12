# Local Contexts Hub Labels - Dataverse

The __Local Contexts Hub Labels - Dataverse__ Process is available as a generated user interface version and with a html
page, which
includes UI elements for that process.

The process uses 2 services, Local Contexts Hub and Dataverse, which are both connected with OpenAPI bridge.
The Bridge-definition of Dataverse is in a specific json file, while the one for Local Contexts Hub is in the
process-page file. This is because we already use the Dataverse bridge in other processes, while the Local Contexts Hub
is only used in the process so far, so we can simply integrate it into the process page file.

This repo contains all files. 
Beware that you need to update the links in respect to your final file structure
```
- index.html
    _init_toolkit_(<process-page-url>)
    assets

- lc_hub_labels_no_ui.json / lc_hub_labels.json
    schemaUri: url of the toolkit schema
    process.instance.scriptUri: lc_hub_labels.js
    services.data_repo.bridge.source.uri: dataverse_bridge_openapi.json
    process.instance.services.lc_hub.bridge.source.instance.execute.openapiSchemaUri: localcontextshub_openapi.json

- dataverse_bridge_openapi.json
    execute.openapiSchemaUri: dataverse_openapi.json
```


Beware that you still need the toolkit
module (https://www.npmjs.com/package/ridagop-toolkit) and include the toolkit schema (__TODO__).
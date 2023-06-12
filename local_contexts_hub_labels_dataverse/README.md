# Local Contexts Hub Labels - Dataverse

The __Local Contexts Hub Labels - Dataverse__ Process is available as a generated user interface version and with a html
page, which
includes UI elements for that process.

The process uses 2 services, Local Contexts Hub and Dataverse, which are both connected with OpenAPI bridge.
The Bridge-definition of Dataverse is in a specific json file, while the one for Local Contexts Hub is in the
process-page file. This is because we already use the Dataverse bridge in other processes, while the Local Contexts Hub
is only used in the process so far, so we can simply integrate it into the process page file.

This repo contains all files. Beware that you still need the toolkit
module (https://www.npmjs.com/package/ridagop-toolkit) and include the toolkit schema (__TODO__).
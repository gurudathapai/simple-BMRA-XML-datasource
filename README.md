## Simple BMRA XML Datasource - 

More documentation about datasource plugins can be found in the [Docs](https://github.com/grafana/grafana/blob/master/docs/sources/plugins/developing/datasources.md).

This also serves as a living example implementation of a datasource.

Your backend needs to implement 4 urls:

 * `/` should return 200 ok. Used for "Test connection" on the datasource config page.
 *'/' should return an xml file with same schema as here below
 * `/xsd` used by the find metric options on the query tab in panels.
  
## Installation
-not  available yet-

To install this plugin using the `grafana-cli` tool:
```
sudo grafana-cli plugins install grafana-bmra-xml-datasource
sudo service grafana-server restart
```
See [here](https://grafana.com/plugins/grafana-bmra-xml-datasource/installation) for more
information.



Copy the data source you want to `/public/app/plugins/datasource/`. Then restart grafana-server. The new data source should now be available in the data source type dropdown in the Add Data Source View.

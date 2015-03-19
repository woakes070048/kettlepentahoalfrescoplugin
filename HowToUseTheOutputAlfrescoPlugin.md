# Introduction #

The Output Alfresco Plugin is very simple to use. The only thing you have to pay attention are the names of the input fields to the plugin. These fields must have the same name (case sensitive) of the metadata you have defined into the Alfresco Custom Content-Model.


# Details #

Our target is to extract data from a data source (e.g. a database) and to load them into Alfresco repository as Documents with specific metadata deriving from the Data Source Input Fields.

Let's suppose to define a Kettle Transformation with two simple steps:
  * An Input Table
  * The Alfresco Plugin

Let's assume you defined an Alfresco Custom Content-Model named **car** and with these metadata:
  * carmodel
  * carengine
  * carcolour

Now, you have only to connect the two steps.

Attention!!!
You must be sure that the field names in output from the Table Input step have the same name (case sensitive) of the Alfresco Custom Content-Model metadata. If not, you can make any mapping with other Kettle Steps (e.g. Filter Rows Steps) in order to provide the right field names in input to the Alfresco Output Plugin.
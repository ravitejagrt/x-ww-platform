# x-ww-platform Experience API
Wework platform experience API

# Use Case <a name="usecase"/>

As a Customer I want to add products to my cart to checkout and purchase them in the WeWork website.

### POST/item
This endpoint adds the item to the cart for checkout 

### POST/item/{itemId}
This endpoint updates the item that is already in the cart

### Running on Studio <a name="runonstudio"/>
Once you have imported Anypoint project into Anypoint Studio you need to follow these steps to run it:

+ Locate the properties file `config-<env>.yaml`, in src/main/app/resources/properties
+ Complete all the properties required as per the examples in the section [Properties to be configured](#propertiestobeconfigured)
+ Once that is done, right click on you Anypoint Template project folder 
+ Hover you mouse over `"Run as"`
+ Click on  `"Mule Application"`
+ Comment API Auto discovery global config to run the application locally in Anypoint Studio

## Properties to be configured (With examples) <a name="propertiestobeconfigured"/>
In order to use this Mule Anypoint Project you need to configure properties (Credentials, configurations, etc.) either in properties file or runtime configuration or in CloudHub as Environment Variables.
Detailed list with examples:
### Application properties
+ http.port `8081`
+ mule.env `local`
+ secret.key ``

Secure properties can be found in the files secure-<env_name>.yaml files

### Munits
We may be able to get the coverage in Anypoint Studio with out configuring enterprise maven repositories and it's credentials in settings.xml. In order to get the Munit coverage outside Anypoint Studio, you need to add enterprise maven repositories in settings.xml with correct credentials.

# Instructions for the JustIn delivery module

Module files are installed in any standard way to install modules in OpenCart.

After installation, you need to update the modifiers.

OpenCart version (OcStore) - 2.3.x


##### Module settings

To go to the module settings, you need:
1. Go to the administrative panel of the store
2. Select the menu "Modules / Extensions"
3. Select the submenu "Modules / Extensions"
4. Select the type of extension "Shipping"
5. Install the "JustIn" module and go to edit

##### Configuration items
1. In the "Basic Settings" tab, enter the Login and Password to the JustIn API.
2. Select the language for obtaining information on the API.
3. Test mode is required to test the module and get acquainted with the functionality.
4. Be sure to change the status of the module to "On" ("Enabled")
5. In the "Cost" tab, you need to set the settings according to the needs of the store to calculate the cost of delivery and display to customers
- Fixed cost - if the "Fixed cost for all orders" setting is enabled, then the amount from the "Fixed cost" field will be used as the cost for delivery in the order. In this case, the tariff of delivery does not matter.
- Free delivery - if the amount of goods in the order is greater than the amount specified in the field "Free delivery from", then delivery will be considered free
IMPORTANTLY! Free shipping is valid even when the fixed cost is enabled. To remove free shipping just leave the field blank, or specify zero "0"
- Delivery tariff depending on the weight of goods in the order - used when calculating the cost of delivery depending on the weight of goods in the order
WARNING! At the time of development of the module, the company JustIn works with delivery to 30 kg. If the total weight of the goods in the order will exceed the maximum allowable weight - the delivery module will not be available.
6. In the "Advanced" tab you can select additional settings for the module:
- "The user can select a branch in any city" - if the setting is disabled, then at the time of ordering the user is given the choice of only branches that are located in the specified city. If the settings are enabled - the user has the option to choose from all branches of JustIn.
IMPORTANTLY! If the user has entered an incorrect city name, or there are no branches in the city for delivery - the branch will also be selected from all JustIn branches.
- "Unit of weight calculation mode" - is necessary if the store uses a unit of weight not a kilogram. (Example: The store uses grams - turn on the mode of calculation of the unit of weight, select grams and specify 1000 in relation)
7. Click the save settings button
8. After saving the settings, you need to reopen the module settings and update the information about branches and cities

## Working with the order

After placing an order with the customer, the store administrator has the opportunity to change the delivery department.
##### This requires:
1. Go to the administrative panel of the store
2. Select the "Sales" menu
3. Select the "Order" submenu
4. Click the "Browse" button on the required order
5. In the "JustIn Delivery" section, click the "Edit" button
6. Select the desired branch
7. Click the save button


The store administrator has the ability to send a delivery request from the administration panel.

To do this, click the "Show delivery request form" button, enter all the necessary form data and click "Send delivery request".

After a successful request, a button for receiving a sticker will appear above the "Show delivery request form" button.

Note. The "Save form" button saves the information entered in the form without sending a delivery request. 


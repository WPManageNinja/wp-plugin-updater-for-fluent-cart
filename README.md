# wp-plugin-updater-for-fluent-cart

Please copy and paste PluginManager directory into your WordPress plugin.
require and replace the namespace with your plugin namespace.

In LicenseManager.php file, replace your settings in __construct.
here item_id is the variation id of your product in the store. And the license_server is the store url.


            'item_id'        => 1,  // variation id
            'license_server' => 'https://cart.test', // use store url

```php


### License API endpoints:
Fluent Software Licensing: 
Frontend API added, we are still working on some validation and security. 

Some example API requests (item_id is the product variation id):
activate_license:
https://yourSiteUrl/?fluent_cart_action=activate_license&item_id=14&license=442df6117d981000ea689fa9c5077770&url=https://www.cart.test

deactivate_license:
https://yourSiteUrl/?fluent_cart_action=deactivate_license&item_id=14&license=442df6117d981000ea689fa9c5077770&url=https://www.cart.test

check_license:
https://yourSiteUrl/?fluent_cart_action=check_license&license=442df6117d981000ea689fa9c5077770&url=https://www.cart.test

get_version:
https://yourSiteUrl/?fluent_cart_action=get_version&item_id=120&license=442df6117d981000ea689fa9c5077770

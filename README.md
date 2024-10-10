# wp-plugin-updater-for-fluent-cart

Please copy and paste PluginManager directory into your WordPress plugin.
require and replace the namespace with your plugin namespace.

In LicenseManager.php file, replace your settings in __construct.
here item_id is the variation id of your product in the store. And the license_server is the store url.


            'item_id'        => 1,  // variation id
            'license_server' => 'https://cart.test', // use store url

```php

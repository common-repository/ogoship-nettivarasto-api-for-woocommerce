=== Ogoship API for WooCommerce ===
Contributors: ogoship
Tags: ogoship,nettivarasto,3PL,logistics
Requires at least: 4.5
Tested up to: 6.6.2
Requires PHP: 5.6
Stable tag: 3.8.0
License: GNU General Public License v3.0
License URI: http://www.gnu.org/licenses/gpl-3.0.html

OGOship plugin for WooCommerce 3.x

== Description ==
OGOship plugin for WooCommerce 3.x

This plugin integrates WooCommerce stores with OGOship services

Allows WooCommerce orders to be sent directly to OGOship manually by admins or upon payment completion.
Optional updating of stock levels from OGOship to WooCommerce

Note: OGOship uses product SKU to match products, so make sure your WooCommerce products have an unique SKU set.

== Installation ==
1. Copy Merchant ID and API Secret Token from myOGO Merchant page and add them to WooCommerce general settings
2. Create/edit WooCommerce products and match their SKU to OGOship product codes.
3. Edit your shipping methods and check if they should be sent from OGOship and match the codes with ones on your Merchant page
Optionally use \'export all products\' and \'get latest changes\' links in WooCommerce general settings to immediately export and import data.

== Changelog ==
Version 3.8.0
 * Fix PHP 8 warnings
 * Improve null value handling

Version 3.7.1
 * Support High-Performance Order Storage

Version 3.7.0
 * Basic support for VAT on products

Version 3.6.6
 * Fixed a bug with order actions

Version 3.6.5
 * Fix partial release
 * Match to github version
 
Version 3.6.3
 * Fix send order checks
 * Add support for Budbee Box pickup point codes

Version 3.6.2
 * Remove Certificate pinning
 * Improve some setting texts

Version 3.6.1
 * Don't treat duplicate order as error
 * Improve field descriptions

Version 3.6.0
 * Make shipping methods compatible with server side integration
 * Tracking url handling

Version 3.5.0
 * Automatic sending of orders when they are moved to 'processing' state.
 * Add more OGOship fields to product details. Move OGOship specific fields to their own panel.

Version 3.4.1
 * Ensure scheduled updates stay on (Wordpress 5.1 cron changes removed it in some cases)

Version 3.4.0
 * Also search shipping metadata for pick up point code.

Version 3.3.9
 * Add receiver company if set
 
Version 3.3.8
 * Search several meta fields for a pickup point code
 * Bug fixes

Version 3.3.7
 * Fixed issue with some order statuses not updating from OGOship to WooCommerce.

Version 3.3.6
 * Fixed an issue which caused error for some uncommon Wordpress installations

Version 3.3.5
 * Extra checks when matching orders to update
 * Add fallback if https fails. To be removed later if everything works.

Version 3.3.4
 * Certificate pinning for SSL API
 
Version 3.3.3
 * Update REST-client library
 * Replace references to Nettivarasto with OGOship
 
Version 3.3.2
 * Woocommerce 3.4 compatibility fix for delivery type transfer

Version 3.3.1
 * Added support for Pick up Point Codes by https://markup.fi/products/woocommerce-noutopistehaku plugin

Version 3.3.0
 * Send currency along with order

Version 3.2.9
 * List products with empty SKU in addition to duplicates
 * Updated some translations

Version 3.2.8
 * Don't call WPML when there are no products translations.

Version 3.2.6
 * Added ability to search for products with duplicate SKUs.
 * Added option to turn off hourly updates

Version 3.2.5
 * Change localizations to match Wordpress plugin directory expectations

Version 3.2.4
 * Fixed issue where WooCommerce could overwrite product name in some cases (introduced by changes in WooCommerce 3.1)
 * Send prices with order lines ( for possible customs declarations)

Version 3.2.3
 * Fixed issue where order missing from WooCommerce could cause Get Latest Changes to fail

Version 3.2.1
 * Fixed issue with getting latest changes timestamp

Version 3.2.0
 * Use longer identifier (0103-2A4D567874d) when sending orders to avoid id collisions, backwards compatible
 * Fetch changes from Nettivarasto 7 days at max.
 * Updated Woocommerce objects to use WC 3.0 style
 * Updated translations
 * Other minor fixes

See full details at https://github.com/ogoship/woocommerce
=== Tag Filters ===
Contributors: jtzl
Tags: plugins, tags, filter, admin
Requires at least: 6.8
Tested up to: 6.8
Stable tag: 1.0.0
Requires PHP: 7.4
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Customize the Plugins interface enabling tag-based filtering.

== Description ==

Tag Filters enhances the plugin management screens in the WordPress admin area by adding the ability to filter plugins by their tags.

On the 'Add New' plugins screen, it adds a list of tags that are present in the currently displayed plugins. Clicking on a tag will filter the list to show only the plugins with that tag.

On the 'Installed Plugins' screen, it adds a 'Tags' column, displaying the tags for each plugin (if they have a `readme.txt` or `package.json` with tags/keywords). Clicking on a tag will filter the list to show only the plugins with that tag.

== Installation ==

1. Upload the `plugin-tag-filters` folder to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Navigate to the 'Plugins > Add New' or 'Plugins > Installed Plugins' screen to see the tag filtering functionality.

== Frequently Asked Questions ==

= Where does the plugin get the tags from? =

For the 'Add New' screen, this plugin processes tag data that WordPress itself retrieves from the WordPress.org plugin API - the plugin does not make direct API calls but filters the results after WordPress fetches them. For the 'Installed Plugins' screen, the tags are retrieved from the `readme.txt` file (from the 'Tags' header) or the `package.json` file (from the 'keywords' field) of each plugin.

= Does this plugin contact any external services? =

No, this plugin does not make any direct external network requests. For the 'Add New' screen, it processes data that WordPress itself retrieves from WordPress.org. For the 'Installed Plugins' screen, it only reads local files (readme.txt and package.json) from your installed plugins.

== Screenshots ==

1. Tag filters on the 'Add New' plugin screen.
2. 'Tags' column on the 'Installed Plugins' screen.
3. Filtering installed plugins by tag.

== Changelog ==

= 1.0.0 =
* Initial release.

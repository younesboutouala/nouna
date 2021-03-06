=== WPML to MultilingualPress ===
Contributors: inpsyde, Bueltge, nullbyte, derpixler, dnaber-de
Tags: WPML, convert, export, import, migration, l10n, i18n, bilingual, international, internationalization, lang, language, localization,  multilanguage, multi language, multilingual, multi lingual, multisite, switcher, translation, website translation, wordpress translation,  network, categories, taxonomy, xliff
Requires at least: 3.8
Tested up to: 4.4
Stable tag: trunk

Convert posts from an existing WPML multilingual site via XLIFF Export/Import for MultilingualPress

== Description ==

= Attention =
This plugin is considered a **tool for developers and advanced users**. It is not a feature plugin for daily use. You can use the plugin, but **make a full backup** of your entire system and make sure you can role back easily! Please give us feedback if you see problems. The best way for feedback is an issue on the repository on [github.com/inpsyde/wpml2mlp](https://github.com/inpsyde/wpml2mlp/issues).

At the moment there's a **known issue** with the scalability which is addressed in the ongoing refactoring. If you're in doubt whether to use the plugin or not, please ask before.

**Please note**: This is **not WPML**! We are not the developer of WPML itself and thus we can't provide any kind of support for WPML.

= What and why? =
If a WordPress site is translated with the WPML Plugin, each translated entry is stored as a separate posts and some custom tables are used to connect the translations. Now if you de-activate the WPML Plugin or have issues with functionality related to version updates, you get a WordPress site with multilingual confusion. This plugin migrates all data from WPML and creates a new WordPress network site out of each single language with use of [MultilingualPress](https://wordpress.org/plugins/multilingual-press/) plugin and also the [Premium](http://multilingualpress.pro/) Version.

This migration plugin:

* Converts the WPML translation records to default core posts or post types
* It creates the relationship about the languages inside the network of the Multisite with the [MultilingualPress](https://wordpress.org/plugins/multilingual-press/) plugin
* Helps to export/import your data to your new WPMS site.
* Use XLIFF (XML Localisation Interchange File Format) format as Export file
* Restores the meta data back to posts and their meta data so that [MultilingualPress](https://wordpress.org/plugins/multilingual-press/) will recognize all your translations.

[MultilingualPress](https://wordpress.org/plugins/multilingual-press/) connects multiple sites as language alternatives in a multisite. Use a customizable widget or Nav Menu to link to all sites.

We cannot guarantee free ad hoc support. Please be patient, we are a small team.
You can follow our progress and development notices on our [developer blog](http://make.marketpress.com/multilingualpress/).


== Installation ==

= Requirements =
* WordPress Multisite 3.4+
* PHP 5.2.4, newer PHP versions will work faster.
* [MultilingualPress](https://wordpress.org/plugins/multilingual-press/) plugin, also the [Premium](http://multilingualpress.pro/) Version

Use the installer via back-end of your install or ...

1. Unpack the download-package.
2. Upload the files to the `/wp-content/plugins/` directory.
3. Single Site: Activate the plugin through the **Plugins** menu in WordPress and click **Activate**
4. Multisite: Activate the plugin through the **Network/Plugins** menu in WordPress and click **Network Activate**.
5. Go to **Settings** on Multisite or **Tools** on single site, **WPML2MLP**, then start the export of the current WPML stuff.

== Changelog ==

= 1.0.0 (09/24/2015) =
* Lot of tester - stable release
* Add move of categories
* Bugfixes and maintenance

= 0.1 Beta (10/25/2014) =
 * First public release, but Beta version

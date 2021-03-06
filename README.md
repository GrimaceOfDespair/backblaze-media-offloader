[![Author](https://img.shields.io/badge/author-Daniel%20M.%20Hendricks-blue.svg?colorB=9900cc )](https://www.danhendricks.com)
[![Latest Version](https://img.shields.io/github/release/dmhendricks/backblaze-media-offloader.svg)](https://github.com/dmhendricks/backblaze-media-offloader/releases)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/danielhendricks)
[![WP Engine](https://img.shields.io/badge/WP%20Engine-Compatible-orange.svg)](http://bit.ly/WPEnginePlans)
[![GitHub License](https://img.shields.io/badge/license-GPLv2-yellow.svg)](https://raw.githubusercontent.com/dmhendricks/backblaze-media-offloader/master/LICENSE)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/dmhendricks/backblaze-media-offloader.svg?style=social)](https://twitter.com/danielhendricks)

# Backblaze B2 Media Offloader Plugin for WordPress

This is currently **under development and only supports basic functions**. Test in a development environment first and use at your own risk.

**This plugin has not been tested on a WordPress multisite setup.**

## Description

This is a WordPress plugin that allows you to serve your WordPress Media Library files via the [Backblaze B2](https://www.backblaze.com/b2/cloud-storage.html#af9kre) cloud storage service.

From their web site:

> *The lowest cost cloud storage on the planet: $0.005/GB a month. Try it and get the first 10 GB free on us.*

### Contributing

I am open to pull requests as well as other feedback. One of the best ways that you can contribute is to help me make it better, either with code or with constructive feedback. Other ways:

* Translations (**after** I get a clean translation file created)
* Sponsor a personal account on WP Engine (for testing plugins) or provide me with SFTP access to a transferrable install.
* I recently got laid off from my job, so if you have any leads/ideas...

## Requirements

* WordPress 4.0 or higher
* PHP 5.6 or higher

### Installation

Until sufficient testing and a proper translation file has been completed, you may [download an installable ZIP](https://f001.backblazeb2.com/file/hendricks/projects/github/dmhendricks/backblaze-media-offloader/releases/backblaze-media-offloader.zip) of this plugin.

### Updates

Once I produce a release version, automatic updates will be available via WordPress. For now, you will have to update manually.

## Known Compatibilities & Conflicts

### Compatible Plugins

* [Safe SVG](https://wordpress.org/plugins/safe-svg/)
* [SVG Support](https://wordpress.org/plugins/svg-support/)

### Conflicts

* [Carbon Fields](https://wordpress.org/plugins/carbon-fields/) - This plugin is **_not_** compatible with legacy versions of Carbon Fields. If it detects that a version <=1.6.0 is loaded, it will deactivate.

There are probably other incompatibilities due to the current method being used rewrite URLs.

If you are aware of any others, please [share](https://github.com/dmhendricks/backblaze-media-offloader/issues).

## TODO

#### Immediate Goals

* **Ability to Delete Locally-Uploaded Files** - Currently, the plugin only uploads media to and deleted from B2, which limits the usefulness of "offloading" content.
* Fix bug with checkboxes on Settings page not being checked by default
* Extensive testing, documentation/wiki and code cleanup
* Implement a better, more persistent means of URL rewriting
* Clean up and create a proper translation (`.pot`) file
* Clean up settings page

#### Future Goals

* Add ability to password-protect content
* Add ability to store files in private buckets

#### Long-Term Goals

* Add one-click feature to migrate existing local media to B2
* Add time-expiring URLs

## Change Log

Release changes will be noted on the [Releases](https://github.com/dmhendricks/backblaze-media-offloader/releases) page.

#### Branch: `master`

* Completely refactored code
* Switched from direct API calls to a fork of [Backblaze B2 SDK for PHP](https://github.com/cwhite92/b2-sdk-php/)

## Credits

Please support [humans.txt](http://humanstxt.org/). It's an initiative for knowing the people behind the web. It's an unobtrusive text file that contains information about the different people who have contributed to building the web site/project.

**Carbon Fields**

	URL: http://carbonfields.net/
	Author: htmlBurger.com
	Twitter: @htmlburger
	Author URI: https://htmlburger.com/
	Location: London, England

**Backblaze B2 PHP SDK**

	URL: https://github.com/cwhite92/b2-sdk-php/
	Author: Chris White
	Twitter: @cwhite_92
	Author URI: https://cwhite.me/
	Location: Edinburgh, United Kingdom

## Screenshot

![Settings Page](https://raw.githubusercontent.com/dmhendricks/backblaze-media-offloader/master/assets/screenshot-1.png "Settings Page")

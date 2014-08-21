# EDD Extension Boilerplate

The EDD Extension Boilerplate serves as a foundation and aims to provide a standardized guide for building extensions. Just download, tweak a few things, and you'll be able to get to the real code in no time!

## Features

* The Plugin Boilerplate is fully-based on the WordPress [Plugin API](http://codex.wordpress.org/Plugin_API).
* Uses [PHPDoc](http://en.wikipedia.org/wiki/PHPDoc) conventions to document the code.
* Example values are given, so you can see what needs to be changed.
* Uses a strict file organization scheme to make sure the assets are easily maintainable.

## Contents

The EDD Extension Boilerplate includes the following files:

* This README, a CHANGELOG, and a `gitignore` file.
* A subdirectory called `plugin-name` that represents the core plugin file.

## Installation

1. Copy the `plugin-name` directory into your `wp-content/plugins` directory
2. Navigate to the *Plugins* dashboard page
3. Locate the menu item that reads *TODO*
4. Click on *Activate*

This will activate the EDD Extension Boilerplate. Because the Boilerplate has no real functionality, nothing will be added to WordPress; however, this demonstrates exactly how your plugin should behave while you're working with the Boilerplate.

## Configuration

 * Replace all instances of plugin-name with the name of your plugin. By WordPress coding standards, the folder name, plugin file name, and text domain should all match. For the purposes of standardization, the folder name, plugin file name, and text domain are all the lowercase form of the actual plugin name, replacing spaces with hyphens.
 * Replace all instances of Plugin_Name with the name of your plugin. For the purposes of standardization, the camel case form of the plugin name, replacing spaces with underscores, is used to define classes in your extension.
 * Replace all instances of PLUGINNAME with the name of your plugin. For the purposes of standardization, the uppercase form of the plugin name, removing spaces, is used to define plugin constants.
 * Replace all instances of Plugin Name with the actual name of your plugin. This really doesn't need to be anywhere other than in the EDD Licensing call in the hooks method.
 * Find all instances of @todo in the plugin and update the relevant areas as necessary.
 * All functions that are not class methods MUST be prefixed with the plugin name, replacing spaces with underscores. NOT PREFIXING YOUR FUNCTIONS CAN CAUSE PLUGIN CONFLICTS!

## File Structure

 * The `plugin-name.php` file should only be used for core functionality necessary to bootstrap the plugin itself.
 * All other code should be in `includes` or a folder therein.
 * The `libraries` folder is provided for reference. If your plugin requires and external libraries, put them here. Otherwise, remove the folder.
 * The `admin` folder is provided for reference. Any code that is explicit to the dashboard belongs here.
 * The `assets` folder contains subfolders for `css`, `img`, and `js` files. Common sense applies.

## License

The EDD Extension Boilerplate is licensed under the GPL v2 or later.

> This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License, version 2, as
published by the Free Software Foundation.

> This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

> You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA

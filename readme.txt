=== Windows Azure Storage for WordPress (with cache control extension) ===
Contributors: Microsoft Open Technologies, aQovia UK Ltd
Tags: Microsoft, Microsoft Open Technologies, Windows Azure, Windows Azure Storage, WordPress, Media Files, Upload
Requires at least: 2.8.0
Tested up to: 3.8.1

Stable tag: 2.0.3

This WordPress plugin allows you to use Windows Azure Storage Service to host your media for your WordPress powered blog.

== Description ==

This WordPress plugin allows you to use Windows Azure Storage Service to host 
your media for your WordPress powered blog. Windows Azure Storage is an effective way 
to scale storage of your site without having to go through the expense of setting up the 
infrastructure for a content delivery.

Please refer UserGuide.pdf for learning more about the plugin.

For more details on Windows Azure Storage Services, please visit the 
<a href="http://www.microsoft.com/azure/windowsazure.mspx">Windows Azure Platform web-site</a>.

Related Links:
*<a href="http://wordpress.org/extend/plugins/windows-azure-storage/" title="Windows Azure Storage for WordPress">Plugin Homepage</a>*

== Installation ==
1. Extract the Windows Azure Storage Plugin windows-azure-storage.zip to the plugins directory of the WordPress installation. 
e.g. if WordPress is installed in "/var/www/html/wordpress" directory, extract the windows-azure-storage.zip file into directory "/var/www/html/wordpress/wp-content/plugins".

1. To activate the plugin, log in into the WordPress as administrator and navigate to list of plugins. Then check the associated checkbox for the plugin and click on "Activate" link.

== Changelog ==
= 2.0.3 =
* Fixed issues if file uploads initially weren't handled by this plugin but were so later on

= 2.0.2 =
* Updated to use Windows Azure SDK for PHP 0.4.0 from https://github.com/WindowsAzure/azure-sdk-for-php (tested on WP 3.8.1)
* Fixed bad header issues when calling SetBlobProperties, also retains previous properties info on content type etc.

= 2.0.1 =
* Enables setting of default cache-control header for uploaded files and changing it later either individually or via bulk update
* For faster access keeps cache-control data stored in local metadata db (but always in sync with Azure container if changed in WP)
* Note: extension enabled only if "Use Windows Azure Storage for default upload" is ticked in Settings > Windows Azure

= 2.0 =
* Updated to use Windows Azure SDK for PHP from https://github.com/WindowsAzure/azure-sdk-for-php and fixed to work with Wordpress 3.4.1

= 1.9 =
* Fixed case sensitivity error in file names on Linux

= 1.8 =
* Bug fixed in generating blob storage URL when using Windows Azure Storage emulator

= 1.7 =
* Added support to upload video files to blob storage

= 1.5 =
* Included Windows Azure SDK for PHP v4.1.0 with the plugin. Now setting mime-type for uploaded file to blob storage.

= 1.4 =
* Included Windows Azure SDK for PHP v4.0.2 with the plugin.

= 1.3 =
* Included Windows Azure SDK for PHP v4.0.1 with the plugin, so no need to install the SDK separetely. Also fixed thumbnail handling issue while uploading files when some specific theme is enabled.

= 1.2 =
* This release is compatible with Windows Azure SDK for PHP v3.0.0. It also fixes issue with deleting media files when thumbnails are associated.

= 1.1 =
* This release is compatible with Windows Azure SDK for PHP v2.1.0 and WordPress 3.1

= 1.0 =
* First release of Windows Azure Storage plugin for WordPress

== License ==
This code released under the terms of the New BSD License (BSD).

# OC_webp_image
opencart webp image support
This extension integrates WebP into OpenCart, and adds WebP images to the page if the browser supports it. Browser support for WebP is detected based on a user-agent check. If WebP support is detected, the extension will output webp format images, otherwise the original cached images(png, jpg, gif) will be displayed.

WebP images are generated with php GD library.
You need to have WebP Support enabled in GD library in order to use this module.
You can check if the webp support is enabled on your server php by: asking the hosting support or using the php functions phpinfo() or gd_info(), or just install the module and if it is not working, uninstall it.

Installation:
This is a plug and play modification without any settings.
Install it with Extension Installer and don't forget to refresh the modification cache.
The new webp images are stored in the image/cachewebp folder next to the default image/cache folder.
The webp quality is set to 90, best in most cases. If you want to change it, you have to do it in the ocmod file. In this case you have to manually clean the cachewebp folder in order to replace the cached images.

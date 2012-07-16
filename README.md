Tribal Fusion Async
===================

This package will work to make your Tribal Fusion tags async. The dependencies for this are:

1. jQuery
2. writecapture.js

[writecapture](https://github.com/iamnoah/writeCapture) is necessary since Tribal Fusion's tags use the evil (blocking..) document.write everywhere. Hence, writecapture is used to over ride the document.write references in the tribal fusion tags.

This implementation has been tested on Internet Explorer 8+, Firefox 3.6+, Chrome 14+ and Safari 5+.

Async ads have dropped my Google page load times on a large web property (20M+ page views per month) from an average of 8s to about 4.8s.

Please make sure you replace the async ad tag in adloader.js with your own script tag. This is the relevant block:

	var tf_300 = '<scr'+'ipt type="text/javascript"><!--e9 = new Object();e9.size = "300x250";//--></scr'+'ipt><scr'+'ipt src="http://tags.expo9.exponential.com/tags/YOUR-ACCOUNT/ATF/tags.js"></scr'+'ipt>';

That's it, enjoy super fast page loading!

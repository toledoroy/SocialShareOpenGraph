SocialShareOpenGraph
====================

Magento SocialShare - Open Graph Tags

The Open Graph protocol enables any web page to become a rich object in a social graph. 
Facebook Graph allows any web page to have the same functionality as any other object on Facebook. 
Use this extension to Make your Magento store Graph compatible and enable any web page on your site to become a rich object in a social graph. 
This will enables the use of Open Graph analytics and more advanced social Add-ons.

See on Magento Commerce http://www.magentocommerce.com/magento-connect/socialshare-open-graph.html


Installation 
====================

    1. Install the Extention
    2. Clear Cache, log out and back in
    3. Navigate to System -> Configuration -> Social Share
    4. Enable Open Graph Tags, and You're Done

	For Facebook Support and analytics create a facebook application on http://www.facebook.com/developers/createapp.php and insert in your Application ID
	
Change Log	
====================
	V3.0.2
			* Open Graph Protocol Updates
			* Changed is_empty value check
			* added default price 0.00 for type 'product' as to facebook requirements
			* Striping HTML Before using htmlspecialchars
	V3.0.1		
			* Tested on Magento 1.9.2
	V3.0.0
		1.       Moved layout XML into a socialshare folder
		2.       Moved design phtml into base/default to support fallback of non-default based themes
		3.       Added logic to prevent Facebook Share JS from loading if no FB app-id is specified (body.html) -> prevents load & js errors for users who only need the OG metadata.
		4.       Added image upload functionality in adminhtml configuration for a default OG image (website logo, for instance). This is only loaded if no other image is found, and is not required.
		5.       Added OG Tags support for the homepage and Category pages
		6.       Added support for category images
		7.       Added support for MAP (if enabled in magento core config), final price vs special price/price and related logic.
		8.       Added support for product ratings
		9.       Built logic around an array to allow for defaults to be inserted for missing data.
		10.      Naming, capitalization and spelling in system.xml -> nothing that changes configuration values that already existed.

	
	
Code Suggestions Reference  
====================

	Type tags and CMS determination logic and type article
	http://naileditdesign.com/facebook-open-graph-meta-tags-in-magento/
	
	htmlspecialchars suggestion
	http://magento.stackexchange.com/questions/16272/how-to-dynamic-generate-open-graph-protocol-meta-tags
	
	Code for pulling current category image
	http://denialdesign.blogspot.com/2012/10/quickly-add-open-graph-tags-to-magento.html
	
	Video Content Tags (NOT IMPLEMENTED)
	http://www.gofishclientcatchers.com/internet-marketing-blog/development-blog/facebook-meta-tags-for-magento/

	Product Object
	https://developers.facebook.com/docs/payments/product
	
	Product Rating
	https://developers.pinterest.com/rich_pins_product/
	
	Image Tag
	og:image : Provided og:image is not big enough. Please use an image that's at least 200x200 and preferably 1500x1500. (Maximum image size is 5MB.) 
	
	
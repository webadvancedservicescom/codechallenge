# codechallenge
==== 1.7.0.2 ====

=== Fixes ===
Fixed: Security vulnerability in Zend_XmlRpc - http://framework.zend.com/security/advisory/ZF2012-01 
Fixed: PayPal Standard does not display on frontend during checkout with some merchant countries



==== 1.7.0.1 ====

=== Major Highlights ===
Improved the backend configuration UI for PayPal payment solutions

=== Improvements ===
Added the functionality for creating nested field sets in the System configuration
Implemented the support for the extended and shared configuration fields
Added the ability to define dependencies between fields from different field sets

=== Changes ===
Moved PayPal configuration to the Payment Methods menu
Set the default value of the cUrl VERIFYPEER option to TRUE for PayPal and added the ability to change this value
Changed the design and position of the configuration field tooltips

=== Fixes ===
Fixed: Inability of SOAP v2 API use in non WS-I compatible mode in the applications written in languages with strong typing
Fixed: In some cases comments history tab on order does not contain information about customer notifications
Fixed: Several potential security vulnerabilities



==== 1.7.0.0 ====

=== Major Highlights ===
Optimized Layered Navigation for pricing
Added CAPTCHA support for admin and customer users
Added different base price per customer group
Added auto generation of coupon codes
Improved the basic Backup and Rollback functionality
Added EU VAT ID validation service integration
Implemented DHL for Europe
Added REST API
Mobile theme was redesigned
Implemented the frontend Cookie Restriction functionality (EU cookie law compliance)
Added the Cash On Delivery and Bank Transfer payment methods

=== Improvements ===
XmlConnect package release v22.1
Upgraded TinyMCE to v3.4.7
Added the ability to translate action array parameter nodes in the layout.xml
Added the support for using custom currency symbols
Added the functionality for cleaning old cache files by cron tasks
Refactored rules-based modules
Improved customer address handling for PayPal Express checkout
Added the ability to customize a store logo in emails from an admin
Refactored the escaping functionality used for translations
Added the ability to turn off/on IP tracking (e.g. 'Placed from IP', displayed on the order-related pages in the backend)
Provided the logic for disabling ACL resources in configuration files
Added additional placeholders for extension developers

=== Changes ===
Added support for "memcached" PHP extension
The js/scriptaculous/dragdrop.js library is upgraded to version 1.9.0
Files in .jpg format are allowed to be used for a favicon
Added the ability to extend the list of attributes in the SELECT query for categories loaded via Mage_Catalog_Model_Resource_Category_Flat::_loadNodes()
Added changes to lib/Varien/Http/Adapter/Curl.php to provide interface for setting different cURL options
Displaying State or Province can be optional for any country
Added the ability to get Magento type from Mage.php

=== Fixes ===
Fixed: Impossible to reset Customer Password via link in Forgot Password email template
Fixed: Reference to non-existing class Mage_Catalog_Block_Seo_Searchterm
Fixed: System can't find page by the URL when Payflow Link PayPal payment method used
Fixed: Grammar issues reported by community
Fixed: Layout is broken for PDF documents, values are overlapped
Fixed: Admin Notifications in backend should not appear again after it been removed or marked as read
Fixed: Reference and contents information is absent in the shipping label for DHL
Fixed: Include commented rewrite rules to .htaccess
Fixed: Shopping Cart is cleared after pressing "Enter"
Fixed: Group Name of "Not Logged IN" Customer Groups is removed automatically after saving
Fixed: Not possible to assign one picture to two products (Media Storage = Database)
Fixed: Exception in shop when accessed by Googlebot
Fixed: SLI for DHL used credentials only from the default configuration scope
Fixed: Old copyright data and system version exist in page footer
Fixed: CMS widgets: Required validation for drop-down "Type" and "Design Package/Theme"
Fixed: On "New Widget Instance" page, drop-down "Type" doesn't have required validation
Fixed: Auto-redirect to Base URL = Yes with correct behavior may cause problems when secure URL is hardcoded
Fixed: Enable Qty Increments on global config has higher priority than product config
Fixed: Short open tag in app/design/adminhtml/default/default/template/currencysymbol/grid.phtml
Fixed: UPS, FedEx and DHL methods should work if zip code from/to isn't required
Fixed: No ability to cancel Partial Authorization checkout with Authorize.net in the frontend
Fixed: Incorrect displaying of the "New User" page
Fixed: Multiple warnings in system.log after running compilation process
Fixed: Session is lost while redirecting from secure to unsecure URL
Fixed: Redirect to base URL should consider full request URI string
Fixed: Product name with <> processed incorrect during creation order in backend
Fixed: FedEx SmartPost method doesn't appears in rate request
Fixed: 3 and 4 digits CVV should be accepted for JCB cards
Fixed: Google Checkout tax isn't applied to Bundle product
Fixed: FPT is not considered by Google Checkout
Fixed: An error occurred during second Customer authorization fail
Fixed: Property declaration typo in Mage_Bundle_Adminhtml_Catalog_Product_Edit_Tab_Bundle_Option
Fixed: Product is not shown in the Catalog when it is Out of Stock and Display Out of Stock Products = Yes
Fixed: Impossible download downloadable product (problem with secure link)
Fixed: Wrong letter case in class names may cause malfunction when Compiler is enabled
Fixed: Incorrect invoice amount in order with FPT
Fixed: Attributes not connected to any product of selected category display in layered navigation
Fixed: No feedback on creating attribute set in IE9 and IE8
Fixed: Unexpected breaking import process leads to creation phantom data into database
Fixed: Two of the same FedEx option show instead of one
Fixed: Notification for Google contains link that cover large area and blocked user work
Fixed: Possible to create user role with empty name if it starts with "less than" sign
Fixed: Impossible to use Clear Shopping Cart button in IE7
Fixed: Impossible create product with one FPT price for all State/Province
Fixed: 'Interval Division Limit' affects to global displaying of Layered Navigation
Fixed: Shipping method must be recalculated on Order Review page if Transfer Shipping Options is enabled
Fixed: Issue with different secure/unsecure URL cause session data lost
Fixed: Can't save option Country in Store Information Tab
Fixed: Rule date information has been missed after using Product Rule or Shopping Cart Price Rule
Fixed: Billing/Shipping address algorithm for PayPal Express checkout works incorrect
Fixed: Error during quick search
Fixed: Block "Description" on Catalog Price Rule page has incorrect size
Fixed: Search doesn't work if Maximum Query Length field is empty
Fixed: The Tags Product RSS doesn't update information after changing tag
Fixed: Customer Attributes and Customer Address Attributes validation
Fixed: Issue with final price calculation for Configurable product with sub products
Fixed: Blank page after customer registration with enabled compilation
Fixed: "Place Order" button must be enabled if all required fields passed the validation on PayPal Express Checkout
Fixed: Products quantity displays incorrect in price ranges after import (rounding problem)
Fixed: Layout issue in shopping cart on frontend (IE8)
Fixed: Impossible to assign user to the role if he is assigned to another role
Fixed: 'Total records found' on Reports -> Tags -> Popular page shows wrong quantity of records
Fixed: Unable to refresh lifetime statistics
Fixed: After changing Price Navigation Step calculation from Automatic(eq price range) to Automatic(eq prod count) the category is loaded very slowly
Fixed: No ability to create Shipping Label (in case with USPS First-Class Mail International Parcel method)
Fixed: It is impossible to create Shipping Label for FedEx
Fixed: Redirect Customer to Account Dashboard after Logging is in enabled and doesn't work for Wishlist
Fixed: No ability to edit values using mass actions for product in IE8, IE9
Fixed: Wrong message during checkout process in Inline Translate mode
Fixed: Default country is selected in Shipping Address during Admin order creation
Fixed: The Static block widget doesn't displayed on the Product View Extra hint for bundle product
Fixed: Bunch of W3C validation errors on frontend while using inline translate
Fixed: Product's association to root category is lost after export/import
Fixed: WYSIWYG Editor: Page is scrolled to the top after inserting variables
Fixed: Incorrect Backup/Rollback message
Fixed: FedEx Free shipping doesn't work correctly
Fixed: Configurable product displaying double price when choosing option
Fixed: Impossible to configure Admin User Emails for store view scope
Fixed: Long payment method data is printed improperly in PDF invoice
Fixed: Impossibility of changing the Rating Value title for store view in existing Rating Value with filled the Rating Value title for store view
Fixed: Trademark symbol not showing up
Fixed: Add "Delivery Option" for FedEx Configurations
Fixed: Saving product takes long time
Fixed: Notice message disappear after clearing cache
Fixed: Products qty displays incorrect in price ranges after import (rounding problem)
Fixed: Images in CSS fail when merging CSS files
Fixed: Mass action update of any attributes resets multi-select attributes to NULL
Fixed: Move CSS from Prototype Windows plug-in to the backend skin
Fixed: DB adapter should check transaction level in case of DDL query
Fixed: When Payment method additional info contains double quote it is displayed as '&quot;' in invoice PDF
Fixed: Incorrect Unit Price(Excl. Tax) in the Shopping Cart Grid after changing currency
Fixed: Incorrect total quantity of records and pagination doesn't work on Reports->Reviews->Products Reviews page
Fixed: Incorrect title of All Reviews for product page
Fixed: Invalid message in shopping cart when trying to add products amount more than allowed
Fixed: Layered Navigation: Icon "Previous" should be appear only on sub-intervals level
Fixed: Processing error occurred when big numeric value is entered to an browser URL
Fixed: Issue with credit memo for multiple bundled products (order status is Processing)
Fixed: Customer group has to be emulated even if customer is sticky assigned to the group
Fixed: "Customs Value" isn't represented in store base currency
Fixed: Layered Navigation: After clicking on interval $0.00, should be filtered and displayed products with price 0.00
Fixed: Absence of redirecting to the grid page after saving Role/User
Fixed: Incorrect logic of assignment of unique ID in Varien_Data_Collection
Fixed: Problems with sorting actions
Fixed: When product is set to be not available for selling checkout is still possible depending on its position in cart
Fixed: Impossibility of creating new order with "Reorder" button when Out of stock or disabled products had been ordered
Fixed: "Online Minute Interval" customer configuration option should have global scope
Fixed: Unable to translate Active/Inactive in promotions grid
Fixed: Response headers contains 500 error during frontend pages browsing
Fixed: Add additional button to PayPal Redirect Page
Fixed: Category Permissions: if "Display Product Price" is set to "No" the page toolbar is absent
Fixed: Layered navigation options have wrong order in backend
Fixed: The "Remember Me" check box with the "What's this?" link should be located below the "Forgot Your Password?" link
Fixed: Warning message is absent, when "Recovery Link Expiration Period" is specified within the correct range
Fixed: PayPal HSS (Website Payment Pro Hosted Solutions) France doesn't work
Fixed: Remove email from Billing address section of the PayPal Express Order Review page
Fixed: It is available enter negative digits in the "Layered Navigation Price Step" (on Category page)
Fixed: First/Last Name algorithm for PayPal Express checkout
Fixed: Asterisk isn't imported in Zip/Post Code field
Fixed: Some strings are not translated in widgets
Fixed: Session isn't stored between secure and unsecure URLs when they are located in different paths of the same domain (no SID in request)
Fixed: "USPS First Class International Parcel" will not show up as an option for customers during checkout
Fixed: UPS, FedEx and DHL methods should work if zip code from / to isn't required
Fixed: Issue when trying to create an order from the backend without selecting the state/province
Fixed: HTTP error when uploading images from a MacOS with shockwave flash 11.1.102.55
Fixed: UPS Configuration "All Methods" should be selected by default
Fixed: Cannot create a product review through backend
Fixed: Typos in Role Permission tree
Fixed: WYSIWYG button layout issue on product page
Fixed: Require Customer's Billing Address is missing option "For Virtual Quotes Only"
Fixed: Errors appears on Design Configuration page if transactional email's logo image and/or favicon files were deleted
Fixed: State/Province value is reset after page reload on some forms
Fixed: Cannot access backend after switching on and switching off "Use Custom Admin URL"
Fixed: "Unsubscribe Selected" and "Delete Selected Problems" buttons don't work
Fixed: After selecting shipping from dropdown system doesn't update order data automatically on PayPal Express Order Review page
Fixed: Buttons on the backend order page don't have titles
Fixed: ERR_RESPONSE_HEADERS_MULTIPLE_CONTENT_DISPOSITION error in Chrome browser
Fixed: Changes related with Apply and Discount Amount options for sub item, applied after clicking "Save Rule" button
Fixed: Invalid Timezone error for Asia/Calcutta when changing default country to India
Fixed: Sorting by position doesn't work for up-sells and related products
Fixed: Absent validation for "Only X left Threshold" field
Fixed: Shipping method calculation based on default shipping address instead of 'Same as billing' setting in backend
Fixed: There is no validation of the field "Handling Fee" that allows number less than zero in UPS shipping method
Fixed: Product name with "<>" processed incorrect during creation order in backend
Fixed: Billing Address Line is always blank if "REQUIREBILLING = 1" for PayPal Express
Fixed: Configuration->Inventory->Qty Increment isn't validated properly
Fixed: Absent message about not enough quantity for bundle and configurable products
Fixed: Wrong behavior of split buttons in IE8
Fixed: Warning message appears after unselecting user in the Role Users grid
Fixed: Incorrect total weight calculation in external shipping methods for products with decimal Qty Increments
Fixed: Tax calculation is incorrect if configurable product mixed up with other composite products in the shopping cart for Store Tax != Customer Tax
Fixed: Products qty displays wrong in layered navigation after changing currency
Fixed: Billing address fields are editable if "Same as shipping" selected on the PayPal Express order review page
Fixed: Incorrect location of "Clear All" link
Fixed: Incorrect price for bundle fixed product with custom option % and catalog price rule applied
Fixed: Import/Export: Append Complex Data works incorrect for customer's address and product's customs data
Fixed: Discount changes subtotal when FPT is active
Fixed: There is no ability to specify backup's name
Fixed: Multi selections fields for website scope settings are greyed out
Fixed: Persistent Shopping Cart: After deleting customers via backend, on frontend customer should be logout completely
Fixed: Incorrect logic during dividing products into multiple boxes for shipping
Fixed: Polls are not working properly in case with different domains for http and https
Fixed: "Block Reference" drop-down contains wrong list of options for frontend Apps types with Products
Fixed: "Wrong store specified" appears on order creation page
Fixed: Customer can't continue Checkout process after selecting Billing Address
Fixed: Refresh Statistics gone from Reports Role
Fixed: USPS shipping label is printed with "SAMPLE - DO NOT MAIL" sign
Fixed: Shipping methods are not refreshed after Update Order Data is pressed on PayPal Express Order Review page
Fixed: Product still invisible in frontend after required re-index
Fixed: JS error on configurable products
Fixed: Configurable product missing name in error message when exceeding quantity during order
Fixed: Added Display Product Count on the Layout Navigation
Fixed: "FedEx Priority Overnight" shipping method isn't calculated correctly
Fixed: Incorrect product price for Bundle products with fixed prices in the shopping cart
Fixed: "Ship Bundle Items" for bundle product works incorrect
Fixed: Impossible to expand settings accordions on the "Design Settings Editor" tab of Theme Customization page under IE7
Fixed: Impossibility to configure Bundle product with Disabled status and create new order with it in the backend
Fixed: Customer email isn't saved in Account Information field
Fixed: Unable to sort products by price
Fixed: Errors during creating/extracting "tar" archive with symbolic links
Fixed: Wrong message text in "Manage Coupon" tab on Shopping Cart Price Rule page
Fixed: 404 page not found error occurs when "Default Store" value is changed for Main Website
Fixed: Unable to import products if Catalog price rule enabled
Fixed: Partial Re-index isn't done for product saved in backend
Fixed: Catalog Price Rule: "Save and Apply" action leads to apply ALL rules, but it have to apply only specified rule
Fixed: Tax isn't recalculated on PayPal Express
Fixed: Backup Name field should allow entering only a limited number of characters
Fixed: In the "Subtotal" row of "Coupons Usage Report" displayed amounts for all Shopping Cart Price Rule in the system
Fixed: Shipping address isn't passed to Magento from PayPal
Fixed: Store view isn't changed when customer subscribes for newsletters
Fixed: Shopping Cart Price Rules are not marked after creating Coupons Usage Report
Fixed: Change buttons structure in prototype/windows.js to match general adminhtml buttons structure
Fixed: Wrong error message on Create New Order page in backend
Fixed: Impossible to configure order of displaying rating values in the frontend
Fixed: Incoming Message in Admin Part has the superfluous symbol '\'
Fixed: Numerous issues with promotions on complex products
Fixed: Recipient Postal-State Mismatch error seen on Shipping Label with FedEx
Fixed: Text messages "This is a required fields." are displayed in the hidden FTP section
Fixed: Incorrect popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed: Layered navigation work incorrect if attribute values defined on Store View level
Fixed: Checking import file returns blank page
Fixed: Change the VAT Number format before sending to VAT ID Validation service
Fixed: Simple products with configured customs options displayed in wishlist incorrectly
Fixed: Incorrect text message for product for which there is no enough quantity in stock
Fixed: Setting float Qty Increments is possible, but doesn't work
Fixed: SQL error during checkout when customers register at checkout and orders a nominal item
Fixed: Iframe for gateway isn't reloaded on the Payment information tab
Fixed: Incorrect behavior after placing order from backend in FF9
Fixed: Catalog price rule skips conditions specified and applies to all products in the catalog
Fixed: Price rule is applying to individual items in bundle when price is set to Dynamic
Fixed: Impossible to save payment method configurations on the Default Config scope
Fixed: "There has been an error processing your request" message is display if not CSV file was selected to import
Fixed: Wrong reindex product attributes after bundle product save
Fixed: Add Products button absent during creating order from backend
Fixed: "All methods" should be selected by default in configuration section "Allowed Methods" for UPS
Fixed: Redirect to base URL issue
Fixed: Added Backup sorting by name possibility
Fixed: Fix grammar mistakes
Fixed: Notifications are not shown if URL Rewrite used
Fixed: "Stop Further Rules Processing" option doesn't work
Fixed: Admin cannot un-assign product from the tag if already approved tag was added to the product by customer
Fixed: Inaccuracy calculation could be 10% for FedEx International Ground shipping
Fixed: Incorrect price calculation of configurable product with custom options (resolved conflicts)
Fixed: Wrong currency displayed in Recently Viewed Product App
Fixed: Tabs are grayed on admin dashboard
Fixed: JS validation for product weight attribute doesn't work
Fixed: Group Price attribute is present as text field using the mass update action
Fixed: Shopping Cart Price Rule isn't applied to Not Logged In Customers
Fixed: "Sign up for our newsletter" text appearing twice
Fixed: Newsletter problem report grid on backend throws Exception
Fixed: Special price doesn't work for Bundles with Dynamic price
Fixed: My Orders block disappears in My Account pages when Reorder functionality is disabled
Fixed: Search doesn't work in Backups grid
Fixed: Re-index "Catalog URL Rewrites" works extremely slowly
Fixed: Checkbox state is preserved for "Put store on the maintenance mode while rollback processing"
Fixed: UPS Configuration All Methods Should Be Selected by Default
Fixed: Rollback fails if database backup was performed after product import
Fixed: Incorrect behavior with 10-digit Zip code, after creating new Tax Rate
Fixed: Configurable attributes that used for create configurable product should not be applied to that product
Fixed: Default group has to be used if customer selects address without VAT number
Fixed: No ability to create Shopping Cart Price Rule
Fixed: Layout issue appears in IE9 on the export grids
Fixed: Issue when trying to view the order using a specific admin user
Fixed: System messages are not displayed at CMS pages and appears only when another message will be invoked
Fixed: On the frontend Search doesn't work properly if search value is 0 (null)
Fixed: The size of the columns in Backup grid is changed if no records were found
Fixed: Maintenance flag isn't deleted if rollback fails with not enough permissions error
Fixed: Customer's group isn't changed if his billing address modified within backend
Added Add a message and the link in the mini shopping cart, when the cart is empty
Fixed: On Edit Shipping Address page button "Validate VAT Number" should be hidden
Fixed: Fatal error when try to ship order with Flat Rate shipping method
- fixed potentially problematic chaining involved getShippingCarrier method
Fixed: No ability to open PDF file with Label
Fixed: Incorrect final price for configurable products if several custom options used
Fixed: "Length", "Width" and "Height" fields on "Create Packages" pop up are active, when "Documents" type is selected in IE7 and IE9
Fixed: HTTP 500 error on frontend for bundle fixed with percent options enabled for sub-products
Fixed: Shipment created on Magento side doesn't send to Google side for Merchant Calculated shipping
- added check for process only Google Checkout internal methods
Fixed: PDF files for invoices and credit memos are not displaying Including Tax Price
Fixed: Default value that was specified in system settings doesn't presented in Code Format drop-down on Manage Coupon Codes tab
Fixed: Qty wipes out to 0 when no qty column is included on import
Fixed: Broken controls makeup is observed after resizing window when customer's page is opened on the backend
Fixed: Values don't fit to "Date Fields Order" drop-downs in "Date & Time Custom Options" on the Catalog page
Fixed: Processing error appears for products with "Qty Uses Decimals" = No and enabled DHL International
Fixed: Apply Tax to FPT setting doesn't seem to work for products with Fixed Product Taxes
Fixed: Apply Coupon Code textbox doesn't fit in the Apply Coupon Code channel on the backend after reducing the browser window
Fixed: Tax and Shipping amounts aren't showing on the merchant reports for Websites Payments Pro PayFlow Edition
Fixed: Incorrect error popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed: No ability to create Shipping Label with New DHL shipping methods
Fixed: Indexing update on save takes too long for large catalog_product_entity_int tables
Fixed: VAT ID group validation takes Default configuration on order creation from backend
Fixed: Pagination isn't shown on My Product Reviews page when items count exceeds the "Show per page" setting
Fixed: Inline translation missing for customer account information labels
Fixed: Corrupted text if drag attribute on Manage Attribute Sets page (IE8)
Fixed: Wrong calculation price of Bundle product with Fixed price, when special price is configured
Fixed: Error Message isn't displayed during unsuccessful Shipping Label creation
Fixed: Unverified redirect is possible in Checkout controller
Fixed: Customer group in not validated again on checkout if Tax Calculation Based on = Shipping Address
Fixed: "Clear All" link doesn't work
Fixed: Wrong message appears when products quantity is updated in the Shopping Cart with enabled Qty Increments setting
Fixed: Created On field on Manage Coupon Codes grid shows incorrect date/time
Fixed: Incorrect price calculation of configurable product with custom options
Fixed: Manage Products > Custom options: Should be possible to enter negative price for custom option of 'Date' type
Fixed: HTTP 500 Internal Server Error on Admin Forgot Password page
Fixed: CSV/Excel XML export doesn't work on Sales->Invoices if filter by Selected=Yes is used
Fixed: "Same As Billing Address" check-box doesn't work
Fixed: Impossible to enter zero in the base price field for customer groups
Fixed: Group Price attribute position on the Prices tab is incorrect
Fixed: Add new column to the grid with number of used coupons
Fixed: Custom options are not stored when downloadable product is duplicated
Fixed: Broken logic for "Zero Subtotal Checkout" order statuses
Fixed: Coupon codes generation fails when trying to generate large amount of codes
Fixed: PayFlow Link: Using "Pay with PayPal" and selected shipping method that is greater than 0 doesn't process order
Fixed: User have to stay on Add New Rule page if error appears on save shopping cart price rule
Fixed: "Automatically Invoice All Items" should be inactive, when were selected "New Order Status: Pending" in "Zero Subtotal Checkout" settings
Fixed: When enormous request in search fields on the front end 414 error appears
Fixed: JS error on edit Shopping Cart Price Rule Page
Fixed: Clear Shopping Cart button add selected item to Items Ordered if check box "Add to Order" is selected
Fixed: "Clear Shopping Cart" button must be located to the left to "Update Shopping Cart" button
Fixed: Export of Group Price data doesn't work
Fixed: Incorrect translation messages definitions
Fixed: Error message isn't displayed if currency exchange rate not found (in case with DHL Int)
Fixed: User role with partial access can't edit attributes of configurable products
Fixed: Letter "n" missed in the word "handling"
Fixed: Buttons don't react for pressing on the "Widget Options" section in Insert Widget window
Fixed: Regular price displays incorrect
Fixed: {{base_url}} in (un)secure_url doesn't work since 1.6.1
Fixed: Product selection field gets cleared out with recently added products from latest page
Fixed: "Change" button while checkout doesn't work
Fixed: MySQL BIGINT field type is wrongly casted to integer
Fixed: Magento Connect Manager proceed with installation of extension if error appears on database backup
Fixed: "Set product as New from/to Date" works excluding selected dates
Fixed: Function fireEvent from lib/varien/js.js does not work in IE9
Fixed: Searching with first and last name has no results
Fixed: CMS Pages: Error in IE7 when select CMS page
Fixed: White screen appears instead of 404 Error Page when going to review a product which doesn't exist
Fixed: "Maximum Package Weight" option works incorrect in case with decimal Qty in shopping Cart
Fixed: Unable to create tables for new EAV entity via SQL upgrade script
Fixed: Customer group isn't revalidated on checkout if Enable Automatic Assignment to Customer Group = Yes
Fixed: Mistake in PayPal Payments Advanced field set title
Fixed: Zero Subtotal Checkout payment method is used, when it is disabled in settings
Fixed: Some info lost from address when customer sets this address as default for shipping
Fixed: Incorrect calculation logic during distribution products between several pieces (in case with DHL)
Fixed: No ability to get shipping rates from US to another country (in case with DHL)
Fixed: Incorrect calculation of pieces weight (in case with Bundle Product)
Fixed: Product Flat Data index causes replication lag on MySQL master/slave model
Fixed: Exception is shown, when admin user provides filtration of Newsletter problem reports by Subscriber
Fixed: Typo in JavaScript error message
Fixed: Unable to do mass action update for products
Fixed: Error Message isn't displayed if currency exchange rate not found (in case with DHL)
Fixed: Weight field is absent during Quick simple product creation
Fixed: correct helper resolving
Fixed: Shipping methods are shown twice in DHLs shipping quote
Fixed: Unable to translate shipping and billing forms on the order creation page
Fixed: Drop-down attribute with layered navigation filter doesn't work with value is set to 0
Fixed: Free Shipping options don't work (in case with DHL)
Fixed: Handling Fee doesn't applied Per Package
Fixed: Free Shipping options works incorrect
Fixed: WYSIWYG Editor: It's impossible insert Widget to CMS page content
Fixed: Customer's group is not changed if his billing address modified within backend
Fixed: Wrong behavior and exception while using invalid image
Fixed: Uninformative error message during saving two nodes with the same parameter URL Key
Fixed: Unable to change order addresses in the admin panel
Fixed: PayPal Express always uses default billing address from customer account
Fixed: Unable to place order if customer selects Register on checkout
Fixed: Performance Issue: Most Viewed product reports on large amount of items
Fixed: In "Customer Addresses" block before and after of State name is located symbols ","
Fixed: Lightbox 2.5 with IE7 returns JS error on the page
Fixed: Unable to change customer status (confirmed/not confirmed) when customer logged in
Fixed: Incorrect notification for empty field during creation catalog price rules
Fixed: Unable to save product with non-checked multiple select attribute
Fixed: Package Size setting for DHL
Fixed: No Input Validation for Catalog Fields
Fixed: Row Total Calculation in Refund
Fixed: "Maximum number of price intervals" should be written with capital letters
Fixed: Divide Order Weight options for DHL
Fixed: Impossible to create new customer in the backend
Fixed: Catalog data-upgrade-1.6.0.0.4-1.6.0.0.5.php is extremely slow
Fixed: Mage_Catalog_Helper_Product::getProduct() doesn't load product by its SKU
Fixed: Preview Template doesn't work correctly
Fixed: Some options of Bundle Product disappeared from the Invoice PDF
Fixed: "Allow Countries" affects on "Country of Manufacture" attribute
Fixed: Some phrases are not translated
Fixed: Incorrect Ordered Qty in Order (in case with decimal qty)
Fixed: Trademark character isn't being displayed properly in the PDF invoice
Fixed: Can't search transactions by order_id in manager.paypal.com
Fixed: Inline Translation: Grid headers are displayed incorrect on the Tag Edit page
Fixed: "Create Extension Package" page becomes broken after compilation
Fixed: Price including tax isn't displayed for some kinds of bundle products
Fixed: Layered navigation for prices displays incorrect price ranges in manual mode
Fixed: Pager works wrong with float page number
Fixed: Incorrect foreign key for EAV entity tables
Fixed: Misprint in downloader/lib/Mage/Connect/Command/Install.php
Fixed: URL Rewrites must be case-sensitive
Fixed: Unable to install package via uploader if author name contains dash
Fixed: Invoice subtotals for cases with partial invoice and discount
Fixed: Catalog URL Rewrites works incorrectly on creating categories
Fixed: New Oder Status setting, specified for payment method works incorrectly when only virtual products are present in Order
Fixed: Rounding issue in catalog and product view if price includes tax
Fixed: Wrong status of catalog event is displayed by editing catalog event
Fixed: Role Resources are not saved
Fixed: "Qty for Item's Status to Become Out of Stock" option works incorrect
Fixed: XML parser works incorrect
Fixed: Mage_Reports_Model_Mysql4_Product_Index_Abstract must be declared abstract
Fixed: "Date & Time" and "Time" custom options becomes required when editing product
Fixed: Unable to cancel an order for an expired Authorize.net authorization
Fixed: Custom options are not stored when downloadable product is duplicated
Fixed: "Cannot initialize the indexer process" error during Mass "Reindex Data" Action
Fixed: Search by new attribute fails, attribute is not shown in layered navigation
Fixed: Exception when "Price Navigation Step Calculation" set to "Manual" mode and FPT enabled
Fixed: WPPHS: Cancel URL doesn't work as should be
Fixed: Error about insufficient permissions is not appears on database backup creation
Fixed: After rollback admin doesn't redirected to the Log in to Admin Panel page
Fixed: Database Backup must not include indexer table data
Fixed: Scheduled Backup creation/failure isn't logged
Fixed: Deleting backup while it is used by another process
Fixed: Opening *.tar files causes an error "There are no trailing zero-filled records"
Fixed: Unable to search by "Time" and "No" in Backups table
Fixed: Backups are deleted without confirmation
Fixed: Reports must be excluded from database snapshot backup
Fixed: There are no products in filtering results, if step calculation in automatic mode
Fixed: No validation for "Default Price Navigation Step"
Fixed: "Back" button doesn't work on the Create New Order page
Fixed: Incorrect logic of Token expiration in Two Step Password Reset flow
Fixed: Tag <br/> is present in tool-tip for field "Number of results (For the last time placed)" on the Edit Search page
Fixed: Unnecessary hard code in Magento Extension
Fixed: Wrong logic in Mage_Core_Model_Resource_Db_Collection_Abstract::join()
Fixed: Description and Short Description are displayed incorrectly for products added with WYSIWYG
Fixed: Adding product to the cart from the product review page leads to 404 page
Fixed: Special symbols in Sort Order field
Fixed: Text is wrong displayed with enabled Inline translation for Admin on backend
Fixed: Inline Translation: Unable to translate some customer information
Fixed: Useless colon on frontend login page
Fixed: Unable to continue checkout for product with zero price and non-zero shipping price
Fixed: Import news_from_date field is configured poorly. It is not accepting the data from file
Fixed: When updating product data through import, attributes that have a value cannot be assigned a new value that is empty
Fixed: Unable to replace non-complex data for products with empty values during import
Fixed: "Wrong order ID" exception in PayPal Express module under heavy load
Fixed: Tax is applying on the order when creating it in the admin panel for a Customer Group with no taxes
Fixed: Issue with retrieving order statuses for array of states
Fixed: Wrong calculation product price with custom option type = Field and Fixed price
Fixed: Back ordered downloadable product is not available even when it is set to be be accessible when order status is Pending
Fixed: Missing column "position" at table catalog_category_anc_products_index_tmp
Fixed: Incorrect behavior of "Save in address book" option during admin Order creation for a new customer
- refactored Mage_Adminhtml_Model_Sales_Order_Create::_prepareCustomer()
Fixed: Terms and Conditions is named differently on different pages
Fixed: "Apply" and "Discount Amount" fields appear twice in the Catalog Price Rule
Fixed: Poll shows incorrect percentage
Fixed: Added validation ability for admin configuration forms
Fixed: UPS XML misprint
Fixed: Misprint in uploading files form
Fixed: Unnecessary check boxes for gift options
Fixed: Wrong resource section declaration in Mage_Tag module
Fixed: "Customers Submitted this Tag" section doesn't update when customer has deleted tag from his account
Fixed: Correct product in category position
Fixed: Unable to create folder in Media Storage
Fixed: Translation with single quotes breaks JavaScript
Fixed: Out of memory error with hundreds of thousands of coupons attached to a single sales rule
Fixed: Unable to translate buttons and tabs on the "Manage Category" page
Fixed: Product Categories Tree doesn't expand in Manage Products page
Fixed: Incorrect products qty returns to stock after refund for configurable product
Fixed: Swf Uploader problems with cross domain Flash Player Policy
Fixed: Unable to translate "Layout Updates" block on create/edit widget page
Fixed: IE7: "Remember Me" checkbox visible on billing information step
Fixed: CMS WYSIWYG Editor - widget is inserted as new while editing in IE8
Fixed: Currency code doesn't correspond to the amount in reports
Fixed: Mage_Adminhtml_Block_Sales_Order_View_Tab_History::getFullHistory() doesn't use unique keys for each message
Fixed: Scope labels are shown without translate wrapper
Fixed: Wrong parameters handling in Core Helper formatDate()
Fixed: Apostrophe in store name breaks Google Analytics tracking
Fixed: Customer attribute prefix is not shown on frontend
Fixed: Incorrect rounding for product with custom options (percent price)
Fixed: Invoicing only part of products results in wrong totals calculation
Fixed: Incorrect Row Total Calculation in Refund
- fixed rounding issues for partial Invoice and Refund
- refactored delta rounding
Fixed: Filter by "Allow Countries" not working for Customer Address Form in the backend
- checking added for set country to be in available list
Fixed: There are sql-installs with empty string used as defaults for table columns, while column is not null able
Fixed: Unable to translate "Note" in "Product Stock Options"
Fixed: Various warning are displayed after creating shipment for 0 items
Fixed: Invalid content in Content-header in the top of page during scrolling during order creation
Fixed: "Online invoice" button present in backend when using Zero Subtotal Checkout
Fixed: String cast type in in_array function
Fixed: Newsletter template content should not disappear when "Show" / "Hide Editor" button was clicked
Fixed: Import feature doesn't validate whether super_products_sku is existing or not
Fixed: Cannot place order with downloadable product and discount code using Paypal Express payment method
Fixed: Product still out of stock after Stock Status reindex
Fixed: Save catalog price rule gives trace if full reindex has already started
Fixed: Reindex requires notification is not shown for Stock Status when stock is updated for several products using Mass Action
Fixed: Incorrect FedEx's shipping rates (in case with non-US country origin)
Fixed: After partial reindex MSRP value is not applied (not viewed) in catalog during mass update action
Fixed: Wrong stock reindex on catalog if partial reindex done after full reindex started
Fixed: In error message string "already exists." written twice, when trying to save Product Tax Class with the same name
Fixed: Slow checkout with non-flushed cache
Fixed: Bundle product total is incorrect in Customization block
Fixed: Special price isn't considered for bundle dynamic products in "Your Customization" block
Fixed: Situation when any amount of duplicate reindex process can be running at one time
Fixed: Error with Advanced Search (in case with Date Attribute)
Fixed: Product Flat Data index isn't marked as "Reindex Required" after importing products when Flat Catalog is enabled
Fixed: User can't change root category for the store
Fixed: JS error causes the overwrite of Title field in PayPal Advanced configuration
Fixed: Mass action doesn't partially reindex catalog for product name/description
Fixed: Remove hint about $1 auth amount from informational message text (PayflowLink configuration)
Fixed: Mass action doesn't partially reindex catalog for product prices
Fixed: PayPal Payments Advanced works with $0 Auth instead of Full Auth
Fixed: Impossible to place Order using "Pay with PayPal" button from PayPal Payments Advanced iframe
Fixed: Mass action doesn't partially reindex catalog search for product if searchable attribute was updated
Fixed: "Please wait" AJAX screen doesn't appear in the middle of the page
Fixed: Checkout link on frontend is always referenced as http
Fixed: GET request is incorrectly formed during category creation
- adjusted assertion to determine last viewed store
Fixed: Display of Tier Pricing with Configurable Products
- added functionality to dynamically update tier prices accordingly to chosen product configuration
Fixed: Google Analytics e-commerce tracking not working
Fixed: URL key isn't used when product is saved
Fixed: Added validation class to 'Qty increments'
Fixed: Entered from admin customer date 1970 (or less) is saved as 2070 (or less)
Fixed: cUrl resource must be closed after checking it for errors, not before
Fixed: Exception while products mass update attributes in backend
Fixed: No ability to reindex Catalog URL Rewrites, error is shown
Fixed: Package with Core dependency
Fixed: Stock Availability isn't updated if 1: Run Price Reindex 2: Update Stock Availability on product with mass action/single product
Fixed: Blank page instead shopping cart page when compilation and PSC are enabled
Fixed: Unable to save redirect URL with special characters in search terms
Fixed: Attribute Set field should have client-side validation and appropriate information message
Fixed: "Localhost" isn't a valid domain name for installation
Fixed: Iframe for PayPal Payments Advanced is not loaded
Fixed: Retain the selected tab on editing CMS page
Fixed: Payflow Link Express Checkout (pay with PayPal button) payment
Fixed: Wrong number of reindex options is displayed
Fixed: Wrong phpDocs for Varien_Db_Select
Fixed: JavaScript calendar date range
- fixed JS calendar behavior to use 4-digits year format
Fixed: Performance issue connected with sales rules on adding product to cart
Fixed: DHL same error message appears several times
Fixed: Item Status says "Mixed" when an order has been completed, should say "Shipped"
Fixed: Product option title is absent in backend order page
Fixed: Incorrect items number during multi shipping checkout
Fixed: User name displays differently in the unsuccessful message and in the text field label (log in form)
Fixed: If one or more indexers have Update Required = Yes and all Status = READY for all indexers than there is no notification for user to do reindex action
Fixed: No space between Address line 1 and line 2 in Shipping Label (in case with FedEx)
Fixed: JS works depends on the position attributes of the product
Fixed: Char set encoding is out-of-date in Settlement reports
Fixed: Settlement reports can't be downloaded if in merchant's account 'Settlement file' is set to 6.0 version
Fixed: Unable to login when secure and unsecure URLs are different
Fixed: Customer session lost when using different domain/subdomain names for secure and unsecure URLs
Fixed: "Most Viewed" reports ignore Store View switcher
Fixed: Long FPT name (and product name) doesn't fit into "My cart" block
Fixed: Paypal IPN post back failure
Fixed: Customer was unable to receive newsletters when it was created via backend
Fixed: Wrong Comments History in notification of order creation/cancellation
Fixed: Non escaped string causes javascript error
Fixed: Unable to view pictures during product editing
Fixed: Ampersand is saved incorrect in attribute label
Fixed: IE8: JS error appears after pressing 'Add new rule' in catalog price rules menu
Fixed: Exception after sorting newsletter queue
Fixed: Customer is not able to log in from URL without "www" in some cases
Fixed: SQL error on category view with enabled and configured FPT
Fixed: Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed: Performance issue with Magento Compiler + APC results in too many I/O calls
Fixed: Website Administrator is able to change default values
Fixed: Some of wishlist blocks and templates still treat the collection of wishlist items as collection of products
Fixed: Unnecessary comments in "Share Wishlist" email



==== 1.7.0.0-rc1 ====

=== Major Highlights ===
New Layered Navigation price bucket algorithm
Added captcha functionality
Implemented different base prices for customer groups
Added auto generation of coupon codes
Backup and Rollback functionality
VAT ID Validation added 
Implemented DHL for Europe
Added REST API

=== Improvements ===
XmlConnect package release v22.1
Upgraded TinyMCE to v3.4.7
Mobile theme was redesigned
Added ability to translate action array parameter nodes via layout.xml
Added support for using custom currency symbols
Added functionality to cleaning old cache files by cron task
Refactored rules-based modules 
Improved customer address handling using PayPal Express checkout
Refactored escaping functionality used with translations
Added ability to customize logo in emails from the admin
Implemented front-end cookies restriction functionality
Added ability to turn off/on IP Tracking (e.g. 'Placed from IP') on the Sales pages in back-end (Order, Invoice, Shipment, Credit memo)
Provided logic to disable ACL resources through configuration files
Added additional placeholders for extensions developers

=== Changes ===
Added "Cash On Delivery" and "Bank Transfer" payment methods
Support for "memcached" PHP extension was added
Library js/scriptaculous/dragdrop.js is upgraded to version 1.9.0
Image file of "jpg" type are allowed for favicon
Added ability to extend list of attributes to select for categories loaded via Mage_Catalog_Model_Resource_Category_Flat::_loadNodes()
Added changes to lib/Varien/Http/Adapter/Curl.php to provide interface for setting different cURL options
Displaying State or Province can be optional for any country 
Added ability to get Magento type from Mage.php

=== Fixes ===
Fixed Multiple warnings in system.log after running compilation process
Fixed Session is lost while redirecting from secure to unsecure URL
Fixed Redirect to base URL should consider full request URI string
Fixed Product name with <> processed incorrect during creation order in backend
Fixed FedEx SmartPost method doesn't appears in rate request
Fixed 3 and 4 digits CVV should be accepted for JCB cards
Fixed Google Checkout tax isn't applied to Bundle product
Fixed FPT is not considered by Google Checkout
Fixed An error occurred during second Customer authorization fail
Fixed Property declaration typo in Mage_Bundle_Adminhtml_Catalog_Product_Edit_Tab_Bundle_Option
Fixed Product is not shown in the Catalog when it is Out of Stock and Display Out of Stock Products = Yes
Fixed Impossible download downloadable product (problem with secure link)
Fixed Wrong letter case in class names may cause malfunction when Compiler is enabled
Fixed Incorrect invoice amount in order with FPT
Fixed Attributes not connected to any product of selected category display in layered navigation
Fixed No feedback on creating attribute set in IE9 and IE8
Fixed Unexpected breaking import process leads to creation phantom data into database
Fixed Two of the same FedEx option show instead of one
Fixed Notification for Google contains link that cover large area and blocked user work
Fixed Possible to create user role with empty name if it starts with "less than" sign
Fixed Impossible to use Clear Shopping Cart button in IE7
Fixed Impossible create product with one FPT price for all State/Province
Fixed 'Interval Division Limit' affects to global displaying of Layered Navigation
Fixed Shipping method must be recalculated on Order Review page if Transfer Shipping Options is enabled
Fixed Issue with different secure/unsecure URL cause session data lost
Fixed Can't save option Country in Store Information Tab
Fixed Rule date information has been missed after using Product Rule or Shopping Cart Price Rule
Fixed Billing/Shipping address algorithm for PayPal Express checkout works incorrect
Fixed Error during quick search
Fixed Block "Description" on Catalog Price Rule page has incorrect size
Fixed Search doesn't work if Maximum Query Length field is empty
Fixed The Tags Product RSS doesn't update information after changing tag
Fixed Customer Attributes and Customer Address Attributes validation
Fixed Issue with final price calculation for Configurable product with sub products
Fixed Blank page after customer registration with enabled compilation
Fixed "Place Order" button must be enabled if all required fields passed the validation on PayPal Express Checkout
Fixed Products quantity displays incorrect in price ranges after import (rounding problem)
Fixed Layout issue in shopping cart on Frontend (IE8)
Fixed Impossible to assign user to the role if he is assigned to another role
Fixed 'Total records found' on Reports -> Tags -> Popular page shows wrong quantity of records
Fixed Unable to refresh lifetime statistics
Fixed After changing Price Navigation Step calculation from Automatic in Continuos the category is loaded very slowly
Fixed No ability to create Shipping Label (in case with USPS First-Class Mail International Parcel method)
Fixed It is impossible to create Shipping Label for FedEx
Fixed Redirect Customer to Account Dashboard after Logging is in enabled and doesn't work for Wishlist
Fixed No ability to edit values using mass actions for product in IE8, IE9
Fixed Wrong message during checkout process in Inline Translate mode
Fixed Default country is selected in Shipping Address during Admin order creation
Fixed The Static block widget doesn't displayed on the Product View Extra hint for bundle product
Fixed Bunch of W3C validation errors on frontend while using inline translate
Fixed Product's association to root category is lost after export/import
Fixed WYSIWYG Editor: Page is scrolled to the top after inserting variables
Fixed Incorrect Backup/Rollback message
Fixed FedEx Free shipping doesn't work correctly
Fixed Configurable product displaying double price when choosing option
Fixed Impossible to configure Admin User Emails for store view scope
Fixed Long payment method data is printed improperly in PDF invoice
Fixed Impossibility of changing the Rating Value title for store view in existing Rating Value with filled the Rating Value title for store view
Fixed Trademark symbol not showing up
Fixed Add "Delivery Option" for FedEx Configurations
Fixed Saving product takes long time
Fixed Notice message disappear after clearing cache
Fixed Products qty displays incorrect in price ranges after import (rounding problem)
Fixed Images in CSS fail when merging CSS files
Fixed Mass action update of any attributes resets multiselect attributes to NULL
Fixed Move CSS from Prototype Windows plug-in to the backend skin
Fixed DB adapter should check transaction level in case of DDL query
Fixed When Payment method additional info contains double quote it is displayed as '&quot;' in invoice PDF
Fixed Incorrect Unit Price(Excl. Tax) in the Shopping Cart Grid after changing currency
Fixed Incorrect total quantity of records and pagination doesn't work on Reports->Reviews->Products Reviews page
Fixed Incorrect title of All Reviews for product page
Fixed Invalid message in shopping cart when trying to add products amount more than allowed
Fixed Layered Navigation: Icon "Previous" should be appear only on sub-intervals level
Fixed Processing error occurred when big numeric value is entered to an browser URL
Fixed Issue with credit memo for multiple bundled products (order status is Processing)
Fixed Customer group has to be emulated even if customer is sticky assigned to the group
Fixed "Customs Value" isn't represented in store base currency
Fixed Layered Navigation: After clicking on interval $0.00, should be filtered and displayed products with price 0.00
Fixed Absence of redirecting to the grid page after saving Role/User
Fixed Incorrect logic of assignment of unique ID in Varien_Data_Collection
Fixed Problems with sorting actions
Fixed When product is unsaleable checkout is still possible depending on its position in cart
Fixed Impossibility of creating new order with "Reorder" button when Out of stock or disabled products had been ordered
Fixed "Online Minute Interval" customer configuration option should have global scope
Fixed Unable to translate Active/Inactive in promotions grid
Fixed Response headers contains 500 error during front-end pages browsing
Fixed Add additional button to PayPal Redirect Page
Fixed Category Permissions: if "Display Product Price" is set to "No" the page toolbar is absent
Fixed Layered navigation options have wrong order in back-end
Fixed The "Remember Me" check box with the "What's this?" link should be located below the "Forgot Your Password?" link
Fixed Warning message is absent, when "Recovery Link Expiration Period" is specified within the correct range
Fixed PayPal HSS (Website Payment Pro Hosted Solutions) France doesn't work
Fixed Remove email from Billing address section of the PayPal Express Order Review page
Fixed It is available enter negative digits in the "Layered Navigation Price Step" (on Category page)
Fixed First/Last Name algorithm for PayPal Express checkout
Fixed Asterisk isn't imported in Zip/Post Code field
Fixed Some strings are not translated in widgets
Fixed Session isn't stored between secure and usecure URLs when they are located in different paths of the same domain (no SID in request)
Fixed "USPS First Class International Parcel" will not show up as an option for customers during checkout
Fixed UPS, FedEx and DHL methods should work if zip code from / to isn't required
Fixed Issue when trying to create an order from the back-end without selecting the state/province
Fixed HTTP error when uploading images from a MacOS with shockwave flash 11.1.102.55
Fixed UPS Configuration "All Methods" should be selected by default
Fixed Cannot create a product review through back-end
Fixed Typos in Role Permission tree
Fixed WYSIWYG button layout issue on product page
Fixed Require Customer's Billing Address is missing option "For Virtual Quotes Only"
Fixed Errors appears on Design Configuration page if transactional email's logo image and/or favicon files were deleted
Fixed State/Province value is reset after page reload on some forms
Fixed Cannot access back-end after switching on and switching off "Use Custom Admin URL"
Fixed "Unsubscribe Selected" and "Delete Selected Problems" buttons don't work
Fixed After selecting shipping from dropdown system doesn't update order data automatically on PayPal Express Order Review page
Fixed Buttons on the back-end order page don't have titles
Fixed ERR_RESPONSE_HEADERS_MULTIPLE_CONTENT_DISPOSITION error in Chrome browser
Fixed Changes related with Apply and Discount Amount options for sub item, applied after clicking "Save Rule" button
Fixed Invalid Timezone error for Asia/Calcutta when changing default country to India
Fixed Sorting by position doesn't work for up-sells and related products
Fixed Absent validation for "Only X left Threshold" field
Fixed Shipping method calculation based on default shipping address instead of 'Same as billing' setting in back-end
Fixed There is no validation of the field "Handling Fee" that allows number less than zero in UPS shipping method
Fixed Product name with "<>" processed incorrect during creation order in back-end
Fixed Billing Address Line is always blank if "REQUIREBILLING = 1" for PayPal Express
Fixed SQL query for getting record count of archived orders takes too long time
Fixed Configuration->Inventory->Qty Increment isn't validated properly
Fixed Absent message about not enough quantity for bundle and configurable products
Fixed Wrong behaviour of split buttons in IE8
Fixed Warning message appears after unselecting user in the Role Users grid
Fixed Incorrect total weight calculation in external shipping methods for products with decimal Qty Increments
Fixed Tax calculation is incorrect if configurable product mixed up with other composite products in the shopping cart for Store Tax != Customer Tax
Fixed Products qty displays wrong in layered navigation after changing currency
Fixed Billing address fields are editable if "Same as shipping" selected on the PayPal Express order review page
Fixed Incorrect location of "Clear All" link
Fixed Incorrect price for bundle fixed product with custom option % and catalog price rule applied
Fixed Import/Export: Append Complex Data works incorrect for customer's address and product's customs data
Fixed Discount changes subtotal when FPT is active
Fixed There is no ability to specify backup's name
Fixed Multi selections fields for website scope settings are greyed out
Fixed "Credit Memos" is written incorrectly in Role Permission tree and on the Sales -> Archive -> Credit Memos page
Fixed Persistent Shopping Cart: After deleting customers via Back-end, on front-end customer should be logout completely
Fixed Incorrect logic during dividing products into multiple boxes for shipping
Fixed Polls are not working properly in case with different domains for http and https
Fixed "Block Reference" drop-down contains wrong list of options for front-end Apps types with Products
Fixed "Wrong store specified" appears on order creation page
Fixed Customer can't continue Checkout process after selecting Billing Address
Fixed Refresh Statistics gone from Reports Role
Fixed USPS shipping label is printed with "SAMPLE - DO NOT MAIL" sign
Fixed Shipping methods are not refreshed after Update Order Data is pressed on PayPal Express Order Review page
Fixed Product still invisible in front-end after required reindex
Fixed JS error on configurable products
Fixed Configurable product missing name in error message when exceeding quantity during order
Fixed Added Display Product Count on the Layout Navigation
Fixed "FedEx Priority Overnight" shipping method isn't calculated correctly
Fixed Incorrect product price for Bundle products with fixed prices in the shopping cart
Fixed "Ship Bundle Items" for bundle product works incorrect
Fixed Impossible to expand settings accordions on the "Design Settings Editor" tab of Theme Customization page under IE7
Fixed Impossibility to configure Bundle product with Disabled status and create new order with it in the back-end
Fixed Customer email isn't saved in Account Information field
Fixed Unable to sort products by price
Fixed Errors during creating/extracting "tar" archive with symbolic links
Fixed Wrong message text in "Manage Coupon" tab on Shopping Cart Price Rule page
Fixed 404 page not found error occurs when "Default Store" value is changed for Main Website
Fixed Unable to import products if Catalog price rule enabled
Fixed Partial Reindex isn't done for product saved in back-end
Fixed Catalog Price Rule: "Save and Apply" action leads to apply ALL rules, but it have to apply only specified rule
Fixed Tax isn't recalculated on PayPal Express
Fixed Backup Name field should allow to enter only a limited number of characters
Fixed In the "Subtotal" row of "Coupons Usage Report" displayed amounts for all Shopping Cart Price Rule in the system
Fixed Shipping address isn't passed to Magento from PayPal
Fixed Store view isn't changed when customer subscribes for newsletters
Fixed Shopping Cart Price Rules are not marked after creating Coupons Usage Report
Fixed Change buttons structure in prototype/windows.js to match general adminhtml buttons structure
Fixed Wrong error message on Create New Order page in back-end
Fixed Impossible to configure order of displaying rating values in the front-end
Fixed Incoming Message in Admin Part has the superfluous symbol '\'
Fixed Numerous issues with promotions on complex products
Fixed Recipient Postal-State Mismatch error seen on Shipping Label with FedEx
Fixed Text messages "This is a required fields." are displayed in the hidden FTP section
Fixed Incorrect popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed Layered navigation work incorrect if attribute values defined on Store View level
Fixed Checking import file returns blank page
Fixed Change the VAT Number format before sending to VAT ID Validation service
Fixed Simple products with configured customs options displayed in wishlist incorrectly
Fixed Incorrect text message for product for which there is no enough quantity in stock
Fixed Setting float Qty Increments is possible, but doesn't work
Fixed SQL error during checkout when customers register at checkout and orders a nominal item
Fixed Iframe for gateway isn't reloaded on the Payment information tab
Fixed Incorrect behavior after placing order from back-end in FF9
Fixed Catalog price rule skips conditions specified and applies to all products in the catalog
Fixed Price rule is applying to individual items in bundle when price is set to Dynamic
Fixed Impossible to save payment method configurations on the Default Config scope
Fixed "There has been an error processing your request" message is display if not CSV file was selected to import
Fixed Wrong reindex product attributes after bundle product save
Fixed Add Products button absent during creating order from back-end
Fixed "All methods" should be selected by default in configuration section "Allowed Methods" for UPS
Fixed Redirect to base URL issue
Fixed Added Backup sorting by name possibility
Fixed Fix grammar mistakes
Fixed Notifications are not shown if URL Rewrite used
Fixed "Stop Further Rules Processing" option doesn't work
Fixed Admin can not unassign product from the tag if already approved tag was added to the product by customer
Fixed Inaccuracy calculation could be 10% for FedEx International Ground shipping
Fixed Incorrect price calculation of configurable product with custom options (resolved conflicts)
Fixed Wrong currency displayed in Recently Viewed Product App
Fixed Tabs are grayed on admin dashboard
Fixed JS validation for product weight attribute doesn't work
Fixed Group Price attribute is present as text field using the mass update action
Fixed Shopping Cart Price Rule isn't applied to Not Logged In Customers
Fixed "Sign up for our newsletter" text appearing twice
Fixed Newsletter problem report grid on back-end throws Exception
Fixed Special price doesn't work for Bundles with Dynamic price
Fixed My Orders block disappears in My Account pages when Reorder functionality is disabled
Fixed Search doesn't work in Backups grid
Fixed Reindex "Catalog URL Rewrites" works extremely slowly
Fixed Checkbox state is preserved for "Put store on the maintenance mode while rollback processing"
Fixed UPS Configuration All Methods Should Be Selected by Default
Fixed Rollback fails if database backup was performed after product import
Fixed Incorrect behavior with 10-digit Zip code, after creating new Tax Rate
Fixed Configurable attributes that used for create configurable product should not be applied to that product
Fixed Default group has to be used if customer selects address without VAT number
Fixed No ability to create Shopping Cart Price Rule
Fixed Layout issue appears in IE9 on the export grids
Fixed Issue when trying to view the order using a specific admin user
Fixed System messages are not displayed at CMS pages and appears only when another message will be invoked
Fixed On the front-end Search doesn't work properly if search value is 0 (null)
Fixed The size of the columns in Backup grid is changed if no records were found
Fixed Maintenance flag isn't deleted if rollback fails with not enough permissions error
Fixed Customer's group isn't changed if his billing address modified within back-end
Added Add a message and the link in the mini shopping cart, when the cart is empty
Fixed On Edit Shipping Address page button "Validate VAT Number" should be hidden
Fixed Fatal error when try to ship order with Flat Rate shipping method 
- fixed potentially problematic chaining involved getShippingCarrier method
Fixed No ability to open PDF file with Label
Fixed Incorrect final price for configurable products if several custom options used
Fixed "Length", "Width" and "Height" fields on "Create Packages" pop up are active, when "Documents" type is selected in IE7 and IE9
Fixed HTTP 500 error on front-end for bundle fixed with percent options enabled for sub-products
Fixed Shipment created on Magento side doesn't send to Google side for Merchant Calculated shipping 
- added check for process only Google Checkout internal methods
Fixed PDF files for invoices and credit memos are not displaying Including Tax Price
Fixed Default value that was specified in system settings doesn't presented in Code Format drop-down on Manage Coupon Codes tab
Fixed Qty wipes out to 0 when no qty column is included on import
Fixed Broken controls makeup is observed after resizing window when customer's page is opened on the back-end
Fixed Values don't fit to "Date Fields Order" drop-downs in "Date & Time Custom Options" on the Catalog page
Fixed Processing error appears for products with "Qty Uses Decimals" = No and enabled DHL International
Fixed Apply Tax to FPT setting doesn't seem to work for products with Fixed Product Taxes
Fixed Apply Coupon Code textbox doesn't fit in the Apply Coupon Code channel on the back-end after reducing the browser window
Fixed Tax and Shipping amounts aren't showing on the merchant reports for Websites Payments Pro PayFlow Edition
Fixed Incorrect error popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed No ability to create Shipping Label with New DHL shipping methods
Fixed Indexing update on save takes too long for large catalog_product_entity_int tables
Fixed VAT ID group validation takes Default configuration on order creation from back-end
Fixed Pagination isn't shown on My Product Reviews page when items count exceeds the "Show per page" setting
Fixed Inline translation missing for customer account information labels
Fixed Corrupted text if drag attribute on Manage Attribute Sets page (IE8)
Fixed Wrong calculation price of Bundle product with Fixed price, when special price is configured
Fixed Error Message isn't displayed during unsuccessful Shipping Label creation
Fixed Unverified redirect is possible in Checkout controller
Fixed Customer group in not validated again on checkout if Tax Calculation Based on = Shipping Address
Fixed "Clear All" link doesn't work
Fixed Wrong message appears when products quantity is updated in the Shopping Cart with enabled Qty Increments setting
Fixed Created On field on Manage Coupon Codes grid shows incorrect date/time
Fixed Incorrect price calculation of configurable product with custom options
Fixed Manage Products > Custom options: Should be possible to enter negative price for custom option of 'Date' type
Fixed HTTP 500 Internal Server Error on Admin Forgot Password page
Fixed CSV/Excel XML export doesn't work on Sales->Invoices if filter by Selected=Yes is used
Fixed "Same As Billing Address" check-box doesn't work
Fixed Impossible to enter zero in the base price field for customer groups
Fixed Group Price attribute position on the Prices tab is incorrect
Fixed Add new column to the grid with number of used coupons
Fixed Custom options are not stored when downloadable product is duplicated 
Fixed Broken logic for "Zero Subtotal Checkout" order statuses
Fixed Coupon codes generation fails when trying to generate large amount of codes
Fixed PayFlow Link: Using "Pay with PayPal" and selected shipping method that is greater than 0 doesn't process order
Fixed User have to stay on Add New Rule page if error appears on save shopping cart price rule
Fixed "Automatically Invoice All Items" should be inactive, when were selected "New Order Status: Pending" in "Zero Subtotal Checkout" settings
Fixed When enormous request in search fields on the front end 414 error appears
Fixed JS error on edit Shopping Cart Price Rule Page
Fixed Clear Shopping Cart button add selected item to Items Ordered if check box "Add to Order" is selected
Fixed "Clear Shopping Cart" button must be located to the left to "Update Shopping Cart" button
Fixed Export of Group Price data doesn't work
Fixed Incorrect translation messages definitions
Fixed Error message isn't displayed if currency exchange rate not found (in case with DHL Int)
Fixed User role with partial access can't edit attributes of configurable products
Fixed Letter "n" missed in the word "handling"
Fixed Buttons don't react for pressing on the "Widget Options" section in Insert Widget window
Fixed Regular price displays incorrect
Fixed {{base_url}} in (un)secure_url doesn't work since 1.6.1
Fixed Product selection field gets cleared out with recently added products from latest page
Fixed "Change" button while checkout doesn't work
Fixed MySQL BIGINT field type is wrongly casted to integer
Fixed Magento Connect Manager proceed with installation of extension if error appears on database backup
Fixed "Set product as New from/to Date" works excluding selected dates
Fixed Function fireEvent from lib/varien/js.js does not work in IE9
Fixed Searching with first and last name has no results
Fixed CMS Pages: Error in IE7 when select CMS page
Fixed White screen appears instead of 404 Error Page when going to review a product which doesn't exist
Fixed "Maximum Package Weight" option works incorrect in case with decimal Qty in shopping Cart
Fixed Unable to create tables for new EAV entity via SQL upgrade script
Fixed Customer group isn't revalidated on checkout if Enable Automatic Assignment to Customer Group = Yes
Fixed Mistake in PayPal Payments Advanced fieldset title
Fixed Zero Subtotal Checkout payment method is used, when it is disabled in settings
Fixed Some info lost from address when customer sets this address as default for shipping
Fixed Incorrect calculation logic during distribution products between several pieces (in case with DHL)
Fixed No ability to get shipping rates from US to another country (in case with DHL)
Fixed Incorrect calculation of pieces weight (in case with Bundle Product)
Fixed Product Flat Data index causes replication lag on MySQL master/slave model
Fixed Exception is shown, when admin user provides filtration of Newsletter problem reports by Subscriber
Fixed Typo in JavaScript error message
Fixed Unable to do mass action update for products
Fixed Error Message isn't displayed if currency exchange rate not found (in case with DHL)
Fixed Weight field is absent during Quick simple product creation
Fixed correct helper resolving
Fixed Shipping methods are shown twice in DHLs shipping quote
Fixed Unable to translate shipping and billing forms on the order creation page
Fixed Drop-down attribute with layered navigation filter doesn't work with value is set to 0
Fixed Free Shipping options doesn't work (in case with DHL)
Fixed Handling Fee doesn't applied Per Package
Fixed Free Shipping options works incorrect
Fixed WYSIWYG Editor: It's impossible insert Widget to CMS page content
Fixed Customer's group is not changed if his billing address modified within backend
Fixed Wrong behaviour and exception while using invalid image
Fixed Uninformative error message during saving two nodes with the same parameter URL Key
Fixed Unable to change order addresses in the admin panel
Fixed PayPal Express always uses default billing address from customer account
Fixed Unable to place order if customer selects Register on checkout
Fixed Performance Issue: Most Viewed product reports on large amount of items
Fixed In "Customer Addresses" block before and after of State name is located symbols ","
Fixed Lightbox 2.5 with IE7 returns JS error on the page
Fixed Unable to change customer status (confirmed/not confirmed) when customer logged in
Fixed Incorrect notification for empty field during creation catalog price rules
Fixed Unable to save product with non-checked multiple select attribute
Fixed Package Size setting for DHL
Fixed No Input Validation for Catalog Fields
Fixed Row Total Calculation in Refund
Fixed "Maximum number of price intervals" should be written with capital letters
Fixed Divide Order Weight options for DHL
Fixed Impossible to create new customer in the backend
Fixed Catalog data-upgrade-1.6.0.0.4-1.6.0.0.5.php is exteremly slow
Fixed Free Shipping options doesn't work (in case with DHL International)
Fixed Mage_Catalog_Helper_Product::getProduct() doesn't load product by its SKU
Fixed Preview Template doesn't work correctly
Fixed Some options of Bundle Product disappeared from the Invoice PDF
Fixed "Allow Countries" affects on "Country of Manufacture" attribute
Fixed Some phrases are not translated
Fixed Incorrect Ordered Qty in Order (in case with decimal qty)
Fixed Trademark character isn't being displayed properly in the PDF invoice
Fixed Can't search transactions by order_id in manager.paypal.com
Fixed Inline Translation: Grid headers are displayed incorrect on the Tag Edit page
Fixed "Create Extension Package" page becomes broken after compilation
Fixed Price including tax isn't displayed for some kinds of bundle products
Fixed Layered navigation for prices displays incorrect price ranges in manual mode
Fixed Pager works wrong with float page number
Fixed Incorrect foreign key for EAV entity tables
Fixed Misprint in downloader/lib/Mage/Connect/Command/Install.php
Fixed URL Rewrites must be case-sensitive
Fixed Unable to install package via uploader if author name contains dash
Fixed Fixed invoice subtotals for cases with partial invoice and discount
Fixed Catalog URL Rewrites works incorrectly on creating categories
Fixed New Oder Status setting, specified for payment method works incorrectly when only virtual products are present in Order
Fixed Rounding issue in catalog and product view if price includes tax
Fixed Wrong status of catalog event is displayed by editing catalog event
Fixed Role Resources are not saved
Fixed "Qty for Item's Status to Become Out of Stock" option works incorrect
Fixed XML parser works incorrect
Fixed Mage_Reports_Model_Mysql4_Product_Index_Abstract must be declared abstract
Fixed "Date & Time" and "Time" custom options becomes required when editing product
Fixed Unable to cancel an order for an expired Authorize.net auth
Fixed Custom options are not stored when downloadable product is duplicated
Fixed "Cannot initialize the indexer process" error during Mass "Reindex Data" Action
Fixed Search by new attribute fails, attribute is not shown in layered navigation
Fixed Exception when "Price Navigation Step Calculation" set to "Manual" mode and FPT enabled
Fixed WPPHS: Cancel URL doesn't work as should be
Fixed Error about insufficient permissions is not appears on database backup creation
Fixed After rollback admin doesn't redirected to the Log in to Admin Panel page
Fixed Database Backup must not include indexer table data
Fixed Scheduled Backup creation/failure isn't logged
Fixed Deleting backup while it is used by another process
Fixed Opening *.tar files causes an error "There are no trailing zero-filled records"
Fixed Unable to search by "Time" and "No" in Backups table
Fixed Backups are deleted without confirmation
Fixed Reports must be excluded from database snapshot backup
Fixed There are no products in filtering results, if step calculation in automatic mode
Fixed No validation for "Default Price Navigation Step"
Fixed "Back" button doesn't work on the Create New Order page
Fixed Incorrect logic of Token expiration in Two Step Password Reset flow
Fixed Tag <br/> is present in tool-tip for field "Number of results (For the last time placed)" on the Edit Search page
Fixed Unnecessary hard code in Magento Extension
Fixed Wrong logic in Mage_Core_Model_Resource_Db_Collection_Abstract::join()
Fixed Description and Short Description are displayed incorrectly for products added with WYSIWYG
Fixed Adding product to the cart from the product review page leads to 404 page
Fixed Special symbols in Sort Order field
Fixed Text is wrong displayed with enabled Inline translation for Admin on back-end
Fixed Inline Translation: Unable to translate some customer information
Fixed Useless colon on front-end login page
Fixed Unable to continue checkout for product with zero price and non-zero shipping price
Fixed Import news_from_date field is configured poorly. It is not accepting the data from file
Fixed When updating product data through import, attributes that have a value cannot be assigned a new value that is empty
Fixed Unable to replace non-complex data for products with empty values during import
Fixed "Wrong order ID" exception in PayPal Express module under heavy load
Fixed Tax is applying on the order when creating it in the admin panel for a Customer Group with no taxes
Fixed Issue with retrieving order statuses for array of states
Fixed Wrong calculation product price with custom option type = Field and Fixed price
Fixed Back ordered downloadable product is not available even when it is set to be be accessible when order status is Pending
Fixed Missing column "position" at table catalog_category_anc_products_index_tmp
Fixed Incorrect behavior of "Save in address book" option during admin Order creation for a new customer
- refactored Mage_Adminhtml_Model_Sales_Order_Create::_prepareCustomer()
Fixed Terms and Conditions is named differently on different pages
Fixed "Apply" and "Discount Amount" fields appear twice in the Catalog Price Rule
Fixed Poll shows incorrect percentage
Fixed Added validation ability for admin configuration forms
Fixed UPS XML misprint
Fixed Misprint in uploading files form
Fixed Unnecessary check boxes for gift options
Fixed Wrong resource section declaration in Mage_Tag module
Fixed "Customers Submitted this Tag" section doesn't update when customer has deleted tag from his account
Fixed Correct product in category position
Fixed Unable to create folder in Media Storage
Fixed Translation with single quotes breaks JavaScript
Fixed Out of memory error with hundreds of thousands of coupons attached to a single sales rule
Fixed Unable to translate buttons and tabs on the "Manage Category" page
Fixed Product Categories Tree doesn't expand in Manage Products page
Fixed Incorrect products qty returns to stock after refund for configurable product
Fixed Swf Uploader problems with cross domain Flash Player Policy
Fixed Unable to translate "Layout Updates" block on create/edit widget page
Fixed IE7: "Remember Me" checkbox visible on billing information step
Fixed CMS WYSIWYG Editor - widget is inserted as new while editing in IE8
Fixed Currency code doesn't correspond to the amount in reports
Fixed Mage_Adminhtml_Block_Sales_Order_View_Tab_History::getFullHistory() doesn't use unique keys for each message
Fixed Scope labels are shown without translate wrapper
Fixed Wrong parameters handling in Core Helper formatDate()
Fixed Apostrophe in store name breaks Google Analytics tracking
Fixed Customer attribute prefix is not shown on frontend
Fixed Incorrect rounding for product with custom options (percent price)
Fixed Invoicing only part of products results in wrong totals calculation
Fixed Incorrect Row Total Calculation in Refund
- fixed rounding issues for partial Invoice and Refund
- refactored delta rounding
Fixed Filter by "Allow Countries" not working for Customer Address Form in the Backend
- checking added for set country to be in available list
Fixed There are sql-installs with empty string used as defaults for table columns, while column is not null able
Fixed Unable to translate "Note" in "Product Stock Options"
Fixed Various warning are displayed after creating shipment for 0 items
Fixed Invalid content in Content-header in the top of page during scrolling during order creation
Fixed "Online invoice" button present in backend when using Zero Subtotal Checkout
Fixed String cast type in in_array function
Fixed Newsletter template content should not disappear when "Show" / "Hide Editor" button was clicked
Fixed Import feature doesn't validate whether super_products_sku is existing or not
Fixed Cannot place order with downloadable product and discount code using Paypal Express payment method
Fixed Product still out of stock after Stock Status reindex
Fixed Save catalog price rule gives trace if full reindex has already started
Fixed Reindex requires notification is not shown for Stock Status when stock is updated for several products using Mass Action
Fixed Incorrect FedEx's shipping rates (in case with non-US country origin)
Fixed After partial reindex MSRP value is not applied (not viewed) in catalog during mass update action
Fixed Wrong stock reindex on catalog if partial reindex done after full reindex started
Fixed In error message string "already exists." written twice, when trying to save Product Tax Class with the same name
Fixed Slow checkout with non-flushed cache
Fixed Bundle product total is incorrect in Customization block
Fixed Special price isn't considered for bundle dynamic products in "Your Customization" block
Fixed Situation when any amount of duplicate reindex process can be running at one time
Fixed Error with Advanced Search (in case with Date Attribute)
Fixed Product Flat Data index isn't marked as "Reindex Required" after importing products when Flat Catalog is enabled
Fixed User can't change root category for the store
Fixed JS error causes the overwrite of Title field in PayPal Advanced configuration
Fixed Mass action doesn't partially reindex catalog for product name/description
Fixed Remove hint about $1 auth amount from informational message text (PayflowLink configuration)
Fixed Mass action doesn't partially reindex catalog for product prices
Fixed PayPal Payments Advanced works with $0 Auth instead of Full Auth
Fixed Impossible to place Order using "Pay with PayPal" button from PayPal Payments Advanced iframe
Fixed Mass action doesn't partially reindex catalog search for product if searchable attribute was updated
Fixed "Please wait" AJAX screen doesn't appear in the middle of the page
Fixed Checkout link on frontend is always referenced as http
Fixed GET request is incorrectly formed during category creation
- adjusted assertion to determine last viewed store
Fixed Display of Tier Pricing with Configurable Products
- added functionality to dynamically update tier prices accordingly to chosen product configuration
Fixed Google Analytics e-commerce tracking not working
Fixed URL key isn't used while product save
Fixed Added validation class to 'Qty increments'
Fixed Entered from admin customer date 1970 (or less) is saved as 2070 (or less)
Fixed cUrl resource must be closed after checking it for errors, not before
Fixed Exception while products mass update attributes in backend
Fixed No ability to reindex Catalog URL Rewrites, error is shown
Fixed Package with Core dependency
Fixed Stock Availability isn't updated if 1: Run Price Reindex 2: Update Stock Availability on product with mass action/single product
Fixed Blank page instead shopping cart page when compilation and PSC are enabled
Fixed Unable to save redirect URL with special characters in search terms
Fixed Attribute Set field should have client-side validation and appropriate information message
Fixed "Localhost" isn't a valid domain name for installation
Fixed Iframe for PayPal Payments Advanced is not loaded
Fixed Retain the selected tab on editing CMS page
Fixed Payflow Link Express Checkout (pay with PayPal button) payment
Fixed Wrong number of reindex options is displayed
Fixed Wrong phpDocs for Varien_Db_Select
Fixed JavaScript calendar date range
- fixed JS calendar behavior to use 4-digits year format
Fixed Performance issue connected with sales rules on adding product to cart
Fixed DHL same error message appears several times
Fixed Item Status says "Mixed" when an order has been completed, should say "Shipped"
Fixed Product option title is absent in backend order page
Fixed Incorrect items number during multi shipping checkout
Fixed User name displays differently in the unsuccessful message and in the text field label (log in form)
Fixed If one or more indexers have Update Required = Yes and all Status = READY for all indexers than there is no notification for user to do reindex action
Fixed No space between Address line 1 and line 2 in Shipping Label (in case with FedEx)
Fixed JS works depends on the position attributes of the product
Fixed Char set encoding is out-of-date in Settlement reports
Fixed Settlement reports can't be downloaded if in merchant's account 'Settlement file' is set to 6.0 version
Fixed Unable to login when secure and unsecure URLs are different
Fixed Customer session lost when using different domain/subdomain names for secure and unsecure URLs
Fixed "Most Viewed" reports ignore Store View switcher
Fixed Long FPT name (and product name) doesn't fit into "My cart" block
Fixed Paypal IPN post back failure
Fixed Customer was unable to receive newsletters when it was created via backend
Fixed Wrong Comments History in notification of order creation/cancellation
Fixed Non escaped string causes javascript error
Fixed Unable to view pictures during product editing
Fixed Ampersand is saved incorrect in attribute label
Fixed IE8: JS error appears after pressing 'Add new rule' in catalog price rules menu
Fixed Exception after sorting newsletter queue
Fixed Customer is not able to log in from URL without "www" in some cases
Fixed SQL error on category view with enabled and configured FPT
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Performance issue with Magento Compiler + APC results in too many I/O calls
Fixed Website Administrator is able to change default values
Fixed Some of wishlist blocks and templates still treat the collection of wishlist items as collection of products
Fixed Unnecessary comments in "Share Wishlist" email



==== 1.7.0.0-beta1 ====

=== Improvements ===
Added ability to translate action array parameter nodes via layout.xml
Added support for using custom currency symbols
Added functionality to cleaning old cache files by cron task
Refactored rules-based modules 
Improved customer address handling using PayPal Express checkout
Refactored escaping functionality used with translations
Added ability to customize logo in emails from the admin
Implemented front-end cookies restriction functionality
Added ability to turn off/on IP Tracking (e.g. 'Placed from IP') on the Sales pages in back-end (Order, Invoice, Shipment, Credit memo)
Provided logic to disable ACL resources through configuration files


=== Changes ===
Support for "memcached" PHP extension was added
Library js/scriptaculous/dragdrop.js is upgraded to version 1.9.0
Image file of "jpg" type are allowed for favicon
Added ability to extend list of attributes to select for categories loaded via Mage_Catalog_Model_Resource_Category_Flat::_loadNodes()
Added changes to lib/Varien/Http/Adapter/Curl.php to provide interface for setting different cURL options
Displaying State or Province can be optional for any country 
Added ability to get Magento type from Mage.php


=== Fixes ===
Fixed Impossibility of changing the Rating Value title for store view in existing Rating Value with filled the Rating Value title for store view
Fixed Trademark symbol not showing up
Fixed Add "Delivery Option" for FedEx Configurations
Fixed Saving product takes long time
Fixed Notice message disappear after clearing cache
Fixed Products qty displays incorrect in price ranges after import (rounding problem)
Fixed User role with partial access can't edit attributes of configurable products
Fixed Images in CSS fail when merging CSS files
Fixed Mass action update of any attributes resets multiselect attributes to NULL
Fixed Move CSS from Prototype Windows plugin to the backend skin
Fixed DB adapter should check transaction level in case of DDL query
Fixed When Payment method additional info contains double quote it is displayed as '&quot;' in invoice PDF
Fixed Incorrect Unit Price(Excl. Tax) in the Shopping Cart Grid after changing currency
Fixed Incorrect total quantity of records and pagination doesn't work on Reports->Reviews->Products Reviews page
Fixed Incorrect title of All Reviews for product page
Fixed Invalid message in shopping cart when trying to add products amount more than allowed
Fixed Layered Navigation: Icon "Previous" should be appear only on sub-intervals level
Fixed Group Price attribute position on the Prices tab is incorrect
Fixed Processing error occurred when big numeric value is entered to an browser URL
Fixed Issue with credit memo for multiple bundled products (order status is Processing)
Fixed Customer group has to be emulated even if customer is sticky assigned to the group
Fixed "Customs Value" isn't represented in store base currency
Fixed Layered Navigation: After clicking on interval $0.00, should be filtered and displayed products with price 0.00
Fixed Absence of redirecting to the grid page after saving Role/User
Fixed Incorrect logic of assignment of unique ID in Varien_Data_Collection
Fixed Problems with sorting actions
Fixed When product is unsaleable checkout is still possible depending on its position in cart
Fixed Impossibility of creating new order with "Reorder" button when Out of stock or disabled products had been ordered
Fixed "Online Minute Interval" customer configuration option should have global scope
Fixed Unable to translate Active/Inactive in promotions grid
Fixed Session is lost while redirecting from secure to unsecure URL
Fixed Response headers contains 500 error during front-end pages browsing
Fixed Add additional button to PayPal Redirect Page
Fixed Category Permissions: if "Display Product Price" is set to "No" the page toolbar is absent
Fixed Layered navigation options have wrong order in back-end
Fixed The "Remember Me" check box with the "What's this?" link should be located below the "Forgot Your Password?" link
Fixed Warning message is absent, when "Recovery Link Expiration Period" is specified within the correct range
Fixed After changing Price Navigation Step calculation from Automatic in Continuos the category is loaded very slowly
Fixed PayPal HSS (Website Payment Pro Hosted Solutions) France doesn't work
Fixed Remove email from Billing address section of the PayPal Express Order Review page
Fixed It is available enter negative digits in the "Layered Navigation Price Step" (on Category page)
Fixed First/Last Name algorithm for PayPal Express checkout
Fixed Asterisk isn't imported in Zip/Post Code field
Fixed Some strings are not translated in widgets
Fixed Session isn't stored between secure and usecure URLs when they are located in different paths of the same domain (no SID in request)
Fixed "USPS First Class International Parcel" will not show up as an option for customers during checkout
Fixed UPS, FedEx and DHL methods should work if zip code from / to isn't required
Fixed Issue when trying to create an order from the back-end without selecting the state/province
Fixed HTTP error when uploading images from a MacOS with shockwave flash 11.1.102.55
Fixed UPS Configuration "All Methods" should be selected by default
Fixed Cannot create a product review through back-end
Fixed Typos in Role Permission tree
Fixed WYSIWYG button layout issue on product page
Fixed Require Customer's Billing Address is missing option "For Virtual Quotes Only"
Fixed Errors appears on Design Configuration page if transactional email's logo image and/or favicon files were deleted
Fixed State/Province value is reset after page reload on some forms
Fixed Cannot access back-end after switching on and switching off "Use Custom Admin URL"
Fixed "Unsubscribe Selected" and "Delete Selected Problems" buttons don't work
Fixed After selecting shipping from dropdown system doesn't update order data automatically on PayPal Express Order Review page
Fixed Buttons on the back-end order page don't have titles
Fixed ERR_RESPONSE_HEADERS_MULTIPLE_CONTENT_DISPOSITION error in Chrome browser
Fixed Changes related with Apply and Discount Amount options for sub item, applied after clicking "Save Rule" button
Fixed Invalid Timezone error for Asia/Calcutta when changing default country to India
Fixed Sorting by position doesn't work for up-sells and related products
Fixed Absent validation for "Only X left Threshold" field
Fixed Shipping method calculation based on default shipping address instead of 'Same as billing' setting in back-end
Fixed There is no validation of the field "Handling Fee" that allows number less than zero in UPS shipping method
Fixed Product name with "<>" processed incorrect during creation order in back-end
Fixed Billing Address Line is always blank if "REQUIREBILLING = 1" for PayPal Express
Fixed SQL query for getting record count of archived orders takes too long time
Fixed Configuration->Inventory->Qty Increment isn't validated properly
Fixed Absent message about not enough quantity for bundle and configurable products
Fixed Wrong behaviour of split buttons in IE8
Fixed Warning message appears after unselecting user in the Role Users grid
Fixed Incorrect total weight calculation in external shipping methods for products with decimal Qty Increments
Fixed Tax calculation is incorrect if configurable product mixed up with other composite products in the shopping cart for Store Tax != Customer Tax
Fixed No validation for "Default Price Navigation Step"
Fixed Products qty displays wrong in layered navigation after changing currency
Fixed Billing address fields are editable if "Same as shipping" selected on the PayPal Express order review page
Fixed Incorrect location of "Clear All" link
Fixed Incorrect price for bundle fixed product with custom option % and catalog price rule applied
Fixed Import/Export: Append Complex Data works incorrect for customer's address and product's customs data
Fixed Discount changes subtotal when FPT is active
Fixed There is no ability to specify backup's name
Fixed Multi selections fields for website scope settings are greyed out
Fixed "Credit Memos" is written incorrectly in Role Permission tree and on the Sales -> Archive -> Credit Memos page
Fixed Persistent Shopping Cart: After deleting customers via Back-end, on front-end customer should be logout completely
Fixed Incorrect logic during dividing products into multiple boxes for shipping
Fixed Polls are not working properly in case with different domains for http and https
Fixed "Block Reference" drop-down contains wrong list of options for front-end Apps types with Products
Fixed "Wrong store specified" appears on order creation page
Fixed Customer can't continue Checkout process after selecting Billing Address
Fixed Refresh Statistics gone from Reports Role
Fixed USPS shipping label is printed with "SAMPLE - DO NOT MAIL" sign
Fixed Shipping methods are not refreshed after Update Order Data is pressed on PayPal Express Order Review page
Fixed Product still invisible in front-end after required reindex
Fixed JS error on configurable products
Fixed Configurable product missing name in error message when exceeding quantity during order
Fixed Added Display Product Count on the Layout Navigation
Fixed "FedEx Priority Overnight" shipping method isn't calculated correctly
Fixed Incorrect product price for Bundle products with fixed prices in the shopping cart
Fixed "Ship Bundle Items" for bundle product works incorrect
Fixed Impossible to expand settings accordions on the "Design Settings Editor" tab of Theme Customization page under IE7
Fixed Impossibility to configure Bundle product with Disabled status and create new order with it in the back-end
Fixed Customer email isn't saved in Account Information field
Fixed Unable to sort products by price
Fixed Errors during creating/extracting "tar" archive with symbolic links
Fixed Wrong message text in "Manage Coupon" tab on Shopping Cart Price Rule page
Fixed 404 page not found error occurs when "Default Store" value is changed for Main Website
Fixed Unable to import products if Catalog price rule enabled
Fixed Partial Reindex isn't done for product saved in back-end
Fixed Catalog Price Rule: "Save and Apply" action leads to apply ALL rules, but it have to apply only specified rule
Fixed Tax isn't recalculated on PayPal Express
Fixed CMS Pages: Error in IE7 when select CMS page
Fixed Backup Name field should allow to enter only a limited number of characters
Fixed In the "Subtotal" row of "Coupons Usage Report" displayed amounts for all Shopping Cart Price Rule in the system
Fixed Shipping address isn't passed to Magento from PayPal
Fixed Store view isn't changed when customer subscribes for newsletters
Fixed Shopping Cart Price Rules are not marked after creating Coupons Usage Report
Fixed Change buttons structure in prototype/windows.js to match general adminhtml buttons structure
Fixed Wrong error message on Create New Order page in back-end
Fixed Impossible to configure order of displaying rating values in the front-end
Fixed Incoming Message in Admin Part has the superfluous symbol '\'
Fixed Numerous issues with promotions on complex products
Fixed Recipient Postal-State Mismatch error seen on Shipping Label with FedEx
Fixed Text messages "This is a required fields." are displayed in the hidden FTP section
Fixed Incorrect popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed Layered navigation work incorrect if attribute values defined on Store View level
Fixed Checking import file returns blank page
Fixed Change the VAT Number format before sending to VAT ID Validation service
Fixed Simple products with configured customs options displayed in wishlist incorrectly
Fixed Incorrect text message for product for which there is no enough quantity in stock
Fixed Setting float Qty Increments is possible, but doesn't work
Fixed SQL error during checkout when customers register at checkout and orders a nominal item
Fixed Iframe for gateway isn't reloaded on the Payment information tab
Fixed Incorrect behavior after placing order from back-end in FF9
Fixed Catalog price rule skips conditions specified and applies to all products in the catalog
Fixed Price rule is applying to individual items in bundle when price is set to Dynamic
Fixed Impossible to save payment method configurations on the Default Config scope
Fixed "There has been an error processing your request" message is display if not CSV file was selected to import
Fixed "Maximum Package Weight" option works incorrect in case with decimal Qty in shopping Cart
Fixed Wrong reindex product attributes after bundle product save
Fixed Add Products button absent during creating order from back-end
Fixed "All methods" should be selected by default in configuration section "Allowed Methods" for UPS
Fixed Redirect to base URL issue
Fixed Added Backup sorting by name possibility
Fixed Entered from admin customer date 1970 (or less) is saved as 2070 (or less)
Fixed Fix grammar mistakes
Fixed Notifications are not shown if URL Rewrite used
Fixed "Stop Further Rules Processing" option doesn't work
Fixed Admin can not unassign product from the tag if already approved tag was added to the product by customer
Fixed Inaccuracy calculation could be 10% for FedEx International Ground shipping
Fixed Incorrect price calculation of configurable product with custom options (resolved conflicts)
Fixed Wrong currency displayed in Recently Viewed Product App
Fixed Tabs are grayed on admin dashboard
Fixed JS validation for product weight attribute doesn't work
Fixed Group Price attribute is present as text field using the mass update action
Fixed Shopping Cart Price Rule isn't applied to Not Logged In Customers
Fixed "Sign up for our newsletter" text appearing twice
Fixed Newsletter problem report grid on back-end throws Exception
Fixed Special price doesn't work for Bundles with Dynamic price
Fixed My Orders block disappears in My Account pages when Reorder functionality is disabled
Fixed Search doesn't work in Backups grid
Fixed Reindex "Catalog URL Rewrites" works extremely slowly
Fixed Checkbox state is preserved for "Put store on the maintenance mode while rollback processing"
Fixed UPS Configuration All Methods Should Be Selected by Default
Fixed Rollback fails if database backup was performed after product import
Fixed Incorrect behavior with 10-digit Zip code, after creating new Tax Rate
Fixed Configurable attributes that used for create configurable product should not be applied to that product
Fixed Default group has to be used if customer selects address without VAT number
Fixed No ability to create Shopping Cart Price Rule
Fixed Layout issue appears in IE9 on the export grids
Fixed Issue when trying to view the order using a specific admin user
Fixed System messages are not displayed at CMS pages and appears only when another message will be invoked
Fixed On the front-end Search doesn't work properly if search value is 0 (null)
Fixed The size of the columns in Backup grid is changed if no records were found
Fixed Maintenance flag isn't deleted if rollback fails with not enough permissions error
Fixed Customer's group isn't changed if his billing address modified within back-end
Added Add a message and the link in the mini shopping cart, when the cart is empty
Fixed On Edit Shipping Address page button "Validate VAT Number" should be hidden
Fixed Fatal error when try to ship order with Flat Rate shipping method 
- fixed potentially problematic chaining involved getShippingCarrier method
Fixed No ability to open PDF file with Label
Fixed Incorrect final price for configurable products if several custom options used
Fixed "Length", "Width" and "Height" fields on "Create Packages" pop up are active, when "Documents" type is selected in IE7 and IE9
Fixed HTTP 500 error on front-end for bundle fixed with percent options enabled for sub-products
Fixed Shipment created on Magento side doesn't send to Google side for Merchant Calculated shipping 
- added check for process only Google Checkout internal methods
Fixed PDF files for invoices and credit memos are not displaying Including Tax Price
Fixed Default value that was specified in system settings doesn't presented in Code Format drop-down on Manage Coupon Codes tab
Fixed Unable to place order if customer selects Register on checkout
Fixed Qty wipes out to 0 when no qty column is included on import
Fixed Broken controls makeup is observed after resizing window when customer's page is opened on the back-end
Fixed Values don't fit to "Date Fields Order" drop-downs in "Date & Time Custom Options" on the Catalog page
Fixed Processing error appears for products with "Qty Uses Decimals" = No and enabled DHL International
Fixed Apply Tax to FPT setting doesn't seem to work for products with Fixed Product Taxes
Fixed Apply Coupon Code textbox doesn't fit in the Apply Coupon Code channel on the back-end after reducing the browser window
Fixed Tax and Shipping amounts aren't showing on the merchant reports for Websites Payments Pro PayFlow Edition
Fixed Incorrect error popup on Manage Coupon Codes tab in Shopping Cart Price Rule
Fixed No ability to create Shipping Label with New DHL shipping methods
Fixed Indexing update on save takes too long for large catalog_product_entity_int tables
Fixed VAT ID group validation takes Default configuration on order creation from back-end
Fixed Pagination isn't shown on My Product Reviews page when items count exceeds the "Show per page" setting
Fixed Inline translation missing for customer account information labels
Fixed Corrupted text if drag attribute on Manage Attribute Sets page (IE8)
Fixed Wrong calculation price of Bundle product with Fixed price, when special price is configured
Fixed Error Message isn't displayed during unsuccessful Shipping Label creation
Fixed Unverified redirect is possible in Checkout controller
Fixed Customer group in not validated again on checkout if Tax Calculation Based on = Shipping Address
Fixed "Clear All" link doesn't work
Fixed Wrong message appears when products quantity is updated in the Shopping Cart with enabled Qty Increments setting
Fixed Created On field on Manage Coupon Codes grid shows incorrect date/time
Fixed Incorrect price calculation of configurable product with custom options
Fixed Manage Products > Custom options: Should be possible to enter negative price for custom option of 'Date' type
Fixed HTTP 500 Internal Server Error on Admin Forgot Password page
Fixed CSV/Excel XML export doesn't work on Sales->Invoices if filter by Selected=Yes is used
Fixed "Same As Billing Address" check-box doesn't work
Fixed Impossible to enter zero in the base price field for customer groups
Fixed Group Price attribute position on the Prices tab is incorrect
Fixed Add new column to the grid with number of used coupons
Fixed Custom options are not stored when downloadable product is duplicated 
Fixed Broken logic for "Zero Subtotal Checkout" order statuses
Fixed Coupon codes generation fails when trying to generate large amount of codes
Fixed PayFlow Link: Using "Pay with PayPal" and selected shipping method that is greater than 0 doesn't process order
Fixed "Clear Shopping Cart" button add selected item to Items Ordered if check box "Add to Order" is selected
Fixed User have to stay on Add New Rule page if error appears on save shopping cart price rule
Fixed "Automatically Invoice All Items" should be inactive, when were selected "New Order Status: Pending" in "Zero Subtotal Checkout" settings
Fixed When enormous request in search fields on the front end 414 error appears
Fixed JS error on edit Shopping Cart Price Rule Page
Fixed "Clear Shopping Cart" button must be located to the left to "Update Shopping Cart" button
Fixed Export of Group Price data doesn't work



==== 1.6.2.0 ====

=== Improvements ===
Refactored indexing process:
- Changed logic around reindexing to prevent conflicts between partial and full reindexing 
- Prevented situations where concurrent indexing processes run at the same time and overwrite each other's data

=== Changes ===
Implemented localized PayPal settings for Japan
Added PayPal Payments Advanced

=== Fixes ===
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Bundle product totals are incorrect in Customization block
Fixed Product option title is absent in backend order page
Fixed SQL error on category view with enabled and configured FPT
Fixed Special price isn't considered for bundle dynamic products in "Your Customization" block
Fixed Cannot place order with downloadable product and discount code using Paypal Express payment method
Fixed Payflow Link Express Checkout ("Pay with PayPal" button) payment
Fixed Char set encoding is out-of-date in Settlement reports
Fixed Settlement reports can not be downloaded if in merchant's account "Settlement file" is set to 6.0 version
Fixed Updates for Payflow Link texts
Fixed Impossible to place Order using "Pay with PayPal" button from Payflow Link iframe, when Payment Action is Sale
Fixed Remove hint about $1 authorization amount from informational message text (Payflow Link configuration)
Fixed Missing column "position" at table catalog_category_anc_products_index_tmp
Fixed Translation with single quotes breaks JS
Fixed Two-step password reset
Fixed Unable to change root category for the store
Fixed Exception while products mass update attributes in backend



==== 1.7.0.0-alpha1 ====

=== Major Highlights ===
New Layered Navigation price bucket algorithm
Added captcha functionality
Implemented different base prices for customer groups
Added auto generation of coupon codes
Backup and Rollback functionality
VAT ID Validation added 
Implemented DHL for Europe

=== Improvements ===
XmlConnect package release v22.1
Upgraded TinyMCE to v3.4.7
Indexers refactoring
Theme for iPhone was redesigned

=== Changes ===
Implemented localized PayPal settings for Japan
Added PayPal Advanced payment method

=== Fixes ===
Fixed Incorrect translation messages definitions
Fixed Error message isn't displayed if currency exchange rate not found (in case with DHL Int)
Fixed Handling Fee doesn't applied Per Package
Fixed User role with partial access can't edit attributes of configurable products
Fixed Letter "n" missed in the word "handling"
Fixed Buttons don't react for pressing on the "Widget Options" section in Insert Widget window
Fixed Regular price displays incorrect
Fixed {{base_url}} in (un)secure_url doesn't work since 1.6.1
Fixed Product selection field gets cleared out with recently added products from latest page
Fixed "Change" button while checkout doesn't work
Fixed MySQL BIGINT field type is wrongly casted to integer
Fixed Magento Connect Manager proceed with installation of extension if error appears on database backup
Fixed "Set product as New from/to Date" works excluding selected dates
Fixed Function fireEvent from lib/varien/js.js does not work in IE9
Fixed Searching with first and last name has no results
Fixed CMS Pages: Error in IE7 when select CMS page
Fixed White screen appears instead of 404 Error Page when going to review a product which doesn't exist
Fixed "Maximum Package Weight" option works incorrect in case with decimal Qty in shopping Cart
Fixed Unable to create tables for new EAV entity via SQL upgrade script
Fixed Customer group isn't revalidated on checkout if Enable Automatic Assignment to Customer Group = Yes
Fixed Mistake in PayPal Payments Advanced fieldset title
Fixed Zero Subtotal Checkout payment method is used, when it is disabled in settings
Fixed Some info lost from address when customer sets this address as default for shipping
Fixed Incorrect calculation logic during distribution products between several pieces (in case with DHL)
Fixed No ability to get shipping rates from US to another country (in case with DHL)
Fixed Incorrect calculation of pieces weight (in case with Bundle Product)
Fixed Product Flat Data index causes replication lag on MySQL master/slave model
Fixed Exception is shown, when admin user provides filtration of Newsletter problem reports by Subscriber
Fixed Typo in JavaScript error message
Fixed Unable to do mass action update for products
Fixed Error Message isn't displayed if currency exchange rate not found (in case with DHL)
Fixed Weight field is absent during Quick simple product creation
Fixed Fixed correct helper resolving
Fixed Shipping methods are shown twice in DHLs shipping quote
Fixed Unable to translate shipping and billing forms on the order creation page
Fixed Drop-down attribute with layered navigation filter doesn't work with value is set to 0
Fixed Free Shipping options doesn't work (in case with DHL)
Fixed Handling Fee doesn't applied Per Package
Fixed Free Shipping options works incorrect
Fixed WYSIWYG Editor: It's impossible insert Widget to CMS page content
Fixed Customer's group is not changed if his billing address modified within backend
Fixed Wrong behaviour and exception while using invalid image
Fixed Layered navigation for prices displays incorrect price ranges in manual mode
Fixed Uninformative error message during saving two nodes with the same parameter URL Key
Fixed Unable to change order addresses in the admin panel
Fixed PayPal Express always uses default billing address from customer account
Fixed Unable to place order if customer selects Register on checkout
Fixed Performance Issue: Most Viewed product reports on large amount of items
Fixed In "Customer Addresses" block before and after of State name is located symbols ","
Fixed Lightbox 2.5 with IE7 returns JS error on the page
Fixed Unable to change customer status (confirmed/not confirmed) when customer logged in
Fixed Incorrect notification for empty field during creation catalog price rules
Fixed Unable to save product with non-checked multiple select attribute
Fixed "Ship Bundle Items" for bundle product works incorrect
Fixed Package Size setting for DHL
Fixed No Input Validation for Catalog Fields
Fixed Row Total Calculation in Refund
Fixed "Maximum number of price intervals" should be written with capital letters
Fixed Divide Order Weight options for DHL
Fixed Incorrect Row Total Calculation in Refund
Fixed Impossible to create new customer in the backend
Fixed Catalog data-upgrade-1.6.0.0.4-1.6.0.0.5.php is exteremly slow
Fixed Free Shipping options doesn't work (in case with DHL International)
Fixed Mage_Catalog_Helper_Product::getProduct() doesn't load product by its SKU
Fixed Preview Template doesn't work correctly
Fixed Some options of Bundle Product disappeared from the Invoice PDF
Fixed "Allow Countries" affects on "Country of Manufacture" attribute
Fixed Some phrases are not translated
Fixed Incorrect Ordered Qty in Order (in case with decimal qty)
Fixed Trademark character isn't being displayed properly in the PDF invoice
Fixed Can't search transactions by order_id in manager.paypal.com
Fixed Inline Translation: Grid headers are displayed incorrect on the Tag Edit page
Fixed "Create Extension Package" page becomes broken after compilation
Fixed Price including tax isn't displayed for some kinds of bundle products
Fixed Layered navigation for prices displays incorrect price ranges in manual mode
Fixed Pager works wrong with float page number
Fixed Incorrect foreign key for EAV entity tables
Fixed Misprint in downloader/lib/Mage/Connect/Command/Install.php
Fixed URL Rewrites must be case-sensitive
Fixed Unable to install package via uploader if author name contains dash
Fixed Fixed invoice subtotals for cases with partial invoice and discount
Fixed Catalog URL Rewrites works incorrectly on creating categories
Fixed New Oder Status setting, specified for payment method works incorrectly when only virtual products are present in Order
Fixed Rounding issue in catalog and product view if price includes tax
Fixed Wrong status of catalog event is displayed by editing catalog event
Fixed Role Resources are not saved
Fixed "Qty for Item's Status to Become Out of Stock" option works incorrect
Fixed XML parser works incorrect
Fixed Mage_Reports_Model_Mysql4_Product_Index_Abstract must be declared abstract
Fixed "Date & Time" and "Time" custom options becomes required when editing product
Fixed Unable to cancel an order for an expired Authorize.net auth
Fixed Custom options are not stored when downloadable product is duplicated
Fixed "Cannot initialize the indexer process" error during Mass "Reindex Data" Action
Fixed Search by new attribute fails, attribute is not shown in layered navigation
Fixed Exception when "Price Navigation Step Calculation" set to "Manual" mode and FPT enabled
Fixed WPPHS: Cancel URL doesn't work as should be
Fixed Error about insufficient permissions is not appears on database backup creation
Fixed After rollback admin doesn't redirected to the Log in to Admin Panel page
Fixed Database Backup must not include indexer table data
Fixed Scheduled Backup creation/failure isn't logged
Fixed Deleting backup while it is used by another process
Fixed Opening *.tar files causes an error "There are no trailing zero-filled records"
Fixed Unable to search by "Time" and "No" in Backups table
Fixed Backups are deleted without confirmation
Fixed Reports must be excluded from database snapshot backup
Fixed There are no products in filtering results, if step calculation in automatic mode
Fixed No validation for "Default Price Navigation Step"
Fixed "Back" button doesn't work on the Create New Order page
Fixed Incorrect logic of Token expiration in Two Step Password Reset flow
Fixed Tag <br/> is present in tool-tip for field "Number of results (For the last time placed)" on the Edit Search page
Fixed Unnecessary hard code in Magento Extension
Fixed Wrong logic in Mage_Core_Model_Resource_Db_Collection_Abstract::join()
Fixed Description and Short Description are displayed incorrectly for products added with WYSIWYG
Fixed Adding product to the cart from the product review page leads to 404 page
Fixed Special symbols in Sort Order field
Fixed Text is wrong displayed with enabled Inline translation for Admin on back-end
Fixed Inline Translation: Unable to translate some customer information
Fixed Useless colon on front-end login page
Fixed Unable to continue checkout for product with zero price and non-zero shipping price
Fixed Import news_from_date field is configured poorly. It is not accepting the data from file
Fixed When updating product data through import, attributes that have a value cannot be assigned a new value that is empty
Fixed Unable to replace non-complex data for products with empty values during import
Fixed "Wrong order ID" exception in PayPal Express module under heavy load
Fixed Tax is applying on the order when creating it in the admin panel for a Customer Group with no taxes
Fixed Issue with retrieving order statuses for array of states
Fixed Wrong calculation product price with custom option type = Field and Fixed price
Fixed Back ordered downloadable product is not available even when it is set to be be accessible when order status is Pending
Fixed Missing column "position" at table catalog_category_anc_products_index_tmp
Fixed Incorrect behavior of "Save in address book" option during admin Order creation for a new customer
- refactored Mage_Adminhtml_Model_Sales_Order_Create::_prepareCustomer()
Fixed Terms and Conditions is named differently on different pages
Fixed "Apply" and "Discount Amount" fields appear twice in the Catalog Price Rule
Fixed Poll shows incorrect percentage
Fixed Added validation ability for admin configuration forms
Fixed UPS XML misprint
Fixed Misprint in uploading files form
Fixed Unnecessary check boxes for gift options
Fixed Wrong resource section declaration in Mage_Tag module
Fixed "Customers Submitted this Tag" section doesn't update when customer has deleted tag from his account
Fixed Correct product in category position
Fixed Unable to create folder in Media Storage
Fixed Translation with single quotes breaks JavaScript
Fixed Out of memory error with hundreds of thousands of coupons attached to a single sales rule
Fixed Unable to translate buttons and tabs on the "Manage Category" page
Fixed Product Categories Tree doesn't expand in Manage Products page
Fixed Incorrect products qty returns to stock after refund for configurable product
Fixed Swf Uploader problems with cross domain Flash Player Policy
Fixed Unable to translate "Layout Updates" block on create/edit widget page
Fixed IE7: "Remember Me" checkbox visible on billing information step
Fixed CMS WYSIWYG Editor - widget is inserted as new while editing in IE8
Fixed Currency code doesn't correspond to the amount in reports
Fixed Mage_Adminhtml_Block_Sales_Order_View_Tab_History::getFullHistory() doesn't use unique keys for each message
Fixed Scope labels are shown without translate wrapper
Fixed Wrong parameters handling in Core Helper formatDate()
Fixed Apostrophe in store name breaks Google Analytics tracking
Fixed Customer attribute prefix is not shown on frontend
Fixed Incorrect rounding for product with custom options (percent price)
Fixed Invoicing only part of products results in wrong totals calculation
Fixed Incorrect Row Total Calculation in Refund
- fixed rounding issues for partial Invoice and Refund
- refactored delta rounding
Fixed Filter by "Allow Countries" not working for Customer Address Form in the Backend
- checking added for set country to be in available list
Fixed There are sql-installs with empty string used as defaults for table columns, while column is not null able
Fixed Unable to translate "Note" in "Product Stock Options"
Fixed Various warning are displayed after creating shipment for 0 items
Fixed Invalid content in Content-header in the top of page during scrolling during order creation
Fixed "Online invoice" button present in backend when using Zero Subtotal Checkout
Fixed String cast type in in_array function
Fixed Newsletter template content should not disappear when "Show" / "Hide Editor" button was clicked
Fixed Import feature doesn't validate whether super_products_sku is existing or not
Fixed Cannot place order with downloadable product and discount code using Paypal Express payment method
Fixed Product still out of stock after Stock Status reindex
Fixed No ability to reindex Catalog URL Rewrites, error is shown
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Save catalog price rule gives trace if full reindex has already started
Fixed Reindex requires notification is not shown for Stock Status when stock is updated for several products using Mass Action
Fixed Incorrect FedEx's shipping rates (in case with non-US country origin)
Fixed After partial reindex MSRP value is not applied (not viewed) in catalog during mass update action
Fixed Wrong stock reindex on catalog if partial reindex done after full reindex started
Fixed In error message string "already exists." written twice, when trying to save Product Tax Class with the same name
Fixed Slow checkout with non-flushed cache
Fixed Bundle product total is incorrect in Customization block
Fixed Special price isn't considered for bundle dynamic products in "Your Customization" block
Fixed Situation when any amount of duplicate reindex process can be running at one time
Fixed Error with Advanced Search (in case with Date Attribute)
Fixed Product Flat Data index isn't marked as "Reindex Required" after importing products when Flat Catalog is enabled
Fixed User can't change root category for the store
Fixed JS error causes the overwrite of Title field in PayPal Advanced configuration
Fixed Mass action doesn't partially reindex catalog for product name/description
Fixed Remove hint about $1 auth amount from informational message text (PayflowLink configuration)
Fixed Mass action doesn't partially reindex catalog for product prices
Fixed PayPal Payments Advanced works with $0 Auth instead of Full Auth
Fixed Impossible to place Order using "Pay with PayPal" button from PayPal Payments Advanced iframe
Fixed Mass action doesn't partially reindex catalog search for product if searchable attribute was updated
Fixed "Please wait" AJAX screen doesn't appear in the middle of the page
Fixed Checkout link on frontend is always referenced as http
Fixed GET request is incorrectly formed during category creation
- adjusted assertion to determine last viewed store
Fixed Display of Tier Pricing with Configurable Products
- added functionality to dynamically update tier prices accordingly to chosen product configuration
Fixed Google Analytics e-commerce tracking not working
Fixed URL key isn't used while product save
Fixed Added validation class to 'Qty increments'
Fixed Entered from admin customer date 1970 (or less) is saved as 2070 (or less)
Fixed cUrl resource must be closed after checking it for errors, not before
Fixed Exception while products mass update attributes in backend
Fixed No ability to reindex Catalog URL Rewrites, error is shown
Fixed Package with Core dependency
Fixed Stock Availability isn't updated if 1: Run Price Reindex 2: Update Stock Availability on product with mass action/single product
Fixed Blank page instead shopping cart page when compilation and PSC are enabled
Fixed Unable to save redirect URL with special characters in search terms
Fixed Attribute Set field should have client-side validation and appropriate information message
Fixed "Localhost" isn't a valid domain name for installation
Fixed Iframe for PayPal Payments Advanced is not loaded
Fixed Retain the selected tab on editing CMS page
Fixed Payflow Link Express Checkout (pay with PayPal button) payment
Fixed Wrong number of reindex options is displayed
Fixed Wrong phpDocs for Varien_Db_Select
Fixed JavaScript calendar date range
- fixed JS calendar behavior to use 4-digits year format
Fixed Performance issue connected with sales rules on adding product to cart
Fixed DHL same error message appears several times
Fixed Item Status says "Mixed" when an order has been completed, should say "Shipped"
Fixed Product option title is absent in backend order page
Fixed Incorrect items number during multi shipping checkout
Fixed User name displays differently in the unsuccessful message and in the text field label (log in form)
Fixed If one or more indexers have Update Required = Yes and all Status = READY for all indexers than there is no notification for user to do reindex action
Fixed No space between Address line 1 and line 2 in Shipping Label (in case with FedEx)
Fixed JS works depends on the position attributes of the product
Fixed Char set encoding is out-of-date in Settlement reports
Fixed Settlement reports can't be downloaded if in merchant's account 'Settlement file' is set to 6.0 version
Fixed Unable to login when secure and unsecure urls are different
Fixed Customer session lost when using different domain/subdomain names for secure and unsecure urls
Fixed "Most Viewed" reports ignore Store View switcher
Fixed Long FPT name (and product name) doesn't fit into "My cart" block
Fixed Paypal IPN post back failure
Fixed Customer was unable to receive newsletters when it was created via backend
Fixed Wrong Comments History in notification of order creation/cancellation
Fixed Non escaped string causes javascript error
Fixed Unable to view pictures during product editing
Fixed Ampersand is saved incorrect in attribute label
Fixed IE8: JS error appears after pressing 'Add new rule' in catalog price rules menu
Fixed Exception after sorting newsletter queue
Fixed Customer is not able to log in from URL without "www" in some cases
Fixed SQL error on category view with enabled and configured FPT
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Performance issue with Magento Compiler + APC results in too many I/O calls
Fixed Website Administrator is able to change default values
Fixed Some of wishlist blocks and templates still treat the collection of wishlist items as collection of products
Fixed Unnecessary comments in "Share Wishlist" email



==== 1.6.x-devel-139014 ====

=== Major Highlights ===
Implemented different base prices for customer groups
Added auto generation of coupon codes

=== Fixes ===
Fixed Incorrect translation messages definitions
Fixed Error message isn't displayed if currency exchange rate not found (in case with DHL Int)
Fixed Handling Fee doesn't applied Per Package
Fixed User role with partial access can't edit attributes of configurable products
Fixed Letter "n" missed in the word "handling"
Fixed Buttons don't react for pressing on the "Widget Options" section in Insert Widget window
Fixed Regular price displays incorrect
Fixed {{base_url}} in (un)secure_url doesn't work since 1.6.1
Fixed Product selection field gets cleared out with recently added products from latest page
Fixed "Change" button while checkout doesn't work
Fixed MySQL BIGINT field type is wrongly casted to integer
Fixed Magento Connect Manager proceed with installation of extension if error appears on database backup
Fixed "Set product as New from/to Date" works excluding selected dates
Fixed Function fireEvent from lib/varien/js.js does not work in IE9
Fixed Searching with first and last name has no results
Fixed CMS Pages: Error in IE7 when select CMS page
Fixed White screen appears instead of 404 Error Page when going to review a product which doesn't exist
Fixed "Maximum Package Weight" option works incorrect in case with decimal Qty in shopping Cart



==== 1.6.x-devel-138051 ====
Fixed Unable to create tables for new EAV entity via SQL upgrade script
Fixed Customer group isn't revalidated on checkout if Enable Automatic Assignment to Customer Group = Yes
Fixed VAT ID validation must not run if added address is outside EU
Fixed Mistake in PayPal Payments Advanced fieldset title
Fixed Zero Subtotal Checkout payment method is used, when it is disabled in settings
Fixed Some info lost from address when customer sets this address as default for shipping
Fixed Incorrect calculation logic during distribution products between several pieces (in case with DHL)
Fixed No ability to get shipping rates from US to another country (in case with DHL)
Fixed Incorrect calculation of pieces weight (in case with Bundle Product)
Fixed Divide Order Weight options for new DHL
Fixed Product Flat Data index causes replication lag on MySQL master/slave model
Fixed Exception is shown, when admin user provides filtration of Newsletter problem reports by Subscriber
Fixed Gap in the section background appears on the Login page when CAPTCHA is enabled
Fixed Typo in JavaScript error message
Fixed Unable to do mass action update for products
Fixed Error Message isn't displayed if currency exchange rate not found (in case with DHL)
Fixed Weight field is absent during Quick simple product creation
Fixed Fixed correct helper resolving
Fixed Shipping methods are shown twice in DHLs shipping quote
Fixed Unable to translate shipping and billing forms on the order creation page
Fixed Drop-down attribute with layered navigation filter doesn't work with value is set to 0
Fixed Free Shipping options doesn't work (in case with DHL)
Fixed Handling Fee doesn't applied Per Package



==== 1.6.x-devel-136760 ====
Fixed Free Shipping options works incorrect
Fixed Wrong massage appears if VAT ID is invalid
Fixed WYSIWYG Editor: It's impossible insert Widget to CMS page content
Fixed After removing VAT Number, customer continues to be assigned to "Valid VAT ID Domestic" group
Fixed Customer's group is not changed if his billing address modified within backend
Fixed Wrong behaviour and exception while using invalid image
Fixed Layered navigation for prices displays incorrect price ranges in manual mode
Fixed Uninformative error message during saving two nodes with the same parameter URL Key
Fixed Unable to change order addresses in the admin panel
Fixed PayPal Express always uses default billing address from customer account
Fixed Unable to place order if customer selects Register on checkout
Fixed Performance Issue: Most Viewed product reports on large amount of items
Fixed In "Customer Addresses" block before and after of State name is located symbols ","
Fixed Lightbox 2.5 with IE7 returns JS error on the page
Fixed Unable to change customer status (confirmed/not confirmed) when customer logged in
Fixed Incorrect notification for empty field during creation catalog price rules
Fixed Unable to save product with non-checked multiple select attribute
Fixed "Ship Bundle Items" for bundle product works incorrect
Fixed Package Size setting for DHL
Fixed No Input Validation for Catalog Fields
Fixed Row Total Calculation in Refund
Fixed "Maximum number of price intervals" should be written with capital letters
Fixed Divide Order Weight options for DHL



==== 1.6.x-devel-135464 ====
Fixed Incorrect Row Total Calculation in Refund
Fixed Impossible to create new customer in the backend
Fixed Catalog data-upgrade-1.6.0.0.4-1.6.0.0.5.php is exteremly slow
Fixed Free Shipping options doesn't work (in case with DHL International)
Fixed Mage_Catalog_Helper_Product::getProduct() doesn't load product by its SKU
Fixed Preview Template doesn't work correctly
Fixed Some options of Bundle Product disappeared from the Invoice PDF
Fixed "Allow Countries" affects on "Country of Manufacture" attribute
Fixed Some phrases are not translated
Fixed Incorrect Ordered Qty in Order (in case with decimal qty)
Fixed Trademark character isn't being displayed properly in the PDF invoice
Fixed Can't search transactions by order_id in manager.paypal.com
Fixed Inline Translation: Grid headers are displayed incorrect on the Tag Edit page
Fixed Scheduled Backup creation/failure isn't logged
Fixed "Create Extension Package" page becomes broken after compilation
Fixed Price including tax isn't displayed for some kinds of bundle products
Fixed Layered navigation for prices displays incorrect price ranges in manual mode
Fixed Pager works wrong with float page number
Fixed VAT Number for country that isn't selected in "European Union Countries" validated
Fixed Incorrect foreign key for EAV entity tables
Fixed VAT ID: Warning message about not-valid VAT Number displayed in green frame
Fixed Misprint in downloader/lib/Mage/Connect/Command/Install.php
Fixed URL Rewrites must be case-sensitive
Fixed Incorrect notification when customer's billing address updated with VAT ID within frontend
Fixed Unable to install package via uploader if author name contains dash
Fixed Fixed invoice subtotals for cases with partial invoice and discount
Fixed Incorrect work of "Disable Automatic Group Changes Based on VAT ID Default Value" option
Fixed Catalog URL Rewrites works incorrectly on creating categories



==== 1.6.x-devel-134386 ====

=== Major Highlights ===
Added VAT ID Validation
Implemented DHL for Europe

=== Improvements ===
Theme for iPhone was redesigned

=== Fixes ===
Fixed New Oder Status setting, specified for payment method works incorrectly when only virtual products are present in Order
Fixed Rounding issue in catalog and product view if price includes tax
Fixed Wrong status of catalog event is displayed by editing catalog event
Fixed Role Resources are not saved
Fixed "Qty for Item's Status to Become Out of Stock" option works incorrect
Fixed XML parser works incorrect
Fixed Mage_Reports_Model_Mysql4_Product_Index_Abstract must be declared abstract
Fixed "Date & Time" and "Time" custom options becomes required when editing product
Fixed Unable to cancel an order for an expired Authorize.net auth
Fixed Custom options are not stored when downloadable product is duplicated
Fixed "Cannot initialize the indexer process" error during Mass "Reindex Data" Action
Fixed Search by new attribute fails, attribute is not shown in layered navigation
Fixed Exception when "Price Navigation Step Calculation" set to "Manual" mode and FPT enabled
Fixed WPPHS: Cancel URL doesn't work as should be
Fixed Error about insufficient permissions is not appears on database backup creation
Fixed After rollback admin doesn't redirected to the Log in to Admin Panel page
Fixed Database Backup must not include indexer table data
Fixed Scheduled Backup creation/failure isn't logged
Fixed Deleting backup while it is used by another process
Fixed Opening *.tar files causes an error "There are no trailing zero-filled records"
Fixed Unable to search by "Time" and "No" in Backups table
Fixed Backups are deleted without confirmation
Fixed Reports must be excluded from database snapshot backup
Fixed There are no products in filtering results, if step calculation in automatic mode
Fixed No validation for "Default Price Navigation Step"
Fixed "Back" button doesn't work on the Create New Order page
Fixed Incorrect logic of Token expiration in Two Step Password Reset flow
Fixed Tag <br/> is present in tool-tip for field "Number of results (For the last time placed)" on the Edit Search page
Fixed Impossible to use CAPTCHA that longer than 12 symbols
Fixed CAPTCHA with space symbol in it works incorrectly
Fixed System backup doesn't complete
Fixed Unnecessary hard code in Magento Extension
Fixed It's impossible specify form where CAPTCHA could be used
Fixed Wrong logic in Mage_Core_Model_Resource_Db_Collection_Abstract::join()
Fixed Description and Short Description are displayed incorrectly for products added with WYSIWYG
Fixed Adding product to the cart from the product review page leads to 404 page
Fixed Special symbols in Sort Order field
Fixed Text is wrong displayed with enabled Inline translation for Admin on back-end
Fixed Inline Translation: Unable to translate some customer information
Fixed Useless colon on front-end login page
Fixed Unable to continue checkout for product with zero price and non-zero shipping price
Fixed Import news_from_date field is configured poorly. It is not accepting the data from file
Fixed When updating product data through import, attributes that have a value cannot be assigned a new value that is empty
Fixed Unable to replace non-complex data for products with empty values during import
Fixed Customer can't understand is CAPTCHA case sensitive or not
Fixed Incorrect CAPTCHA's default configuration values
Fixed "Wrong order ID" exception in PayPal Express module under heavy load
Fixed Tax is applying on the order when creating it in the admin panel for a Customer Group with no taxes
Fixed Issue with retrieving order statuses for array of states
Fixed Wrong calculation product price with custom option type = Field and Fixed price
Fixed Back ordered downloadable product is not available even when it is set to be be accessible when order status is Pending



==== 1.6.x-devel-133001 ====

=== Major Highlights ===
Implemented Backup and Rollback functionality

=== Fixes ===
Fixed Full Product Price reindex started instead of partial if prices updated with mass action
Fixed Missing column "position" at table catalog_category_anc_products_index_tmp
Fixed Incorrect behavior of "Save in address book" option during admin Order creation for a new customer
- refactored Mage_Adminhtml_Model_Sales_Order_Create::_prepareCustomer()
Fixed Terms and Conditions is named differently on different pages
Fixed "Apply" and "Discount Amount" fields appear twice in the Catalog Price Rule
Fixed Poll shows incorrect percentage
Fixed Added validation ability for admin configuration forms
Fixed UPS XML misprint
Fixed Misprint in uploading files form
Fixed Unnecessary check boxes for gift options
Fixed Wrong resource section declaration in Mage_Tag module
Fixed "Customers Submitted this Tag" section doesn't update when customer has deleted tag from his account
Fixed Correct product in category position
Fixed Unable to create folder in Media Storage
Fixed Translation with single quotes breaks JavaScript
Fixed Out of memory error with hundreds of thousands of coupons attached to a single sales rule
Fixed Unable to translate buttons and tabs on the "Manage Category" page
Fixed Product Categories Tree doesn't expand in Manage Products page
Fixed Incorrect products qty returns to stock after refund for configurable product
Fixed Swf Uploader problems with cross domain Flash Player Policy
Fixed Unable to translate "Layout Updates" block on create/edit widget page
Fixed IE7: "Remember Me" checkbox visible on billing information step
Fixed CMS WYSIWYG Editor - widget is inserted as new while editing in IE8
Fixed Currency code doesn't correspond to the amount in reports
Fixed Mage_Adminhtml_Block_Sales_Order_View_Tab_History::getFullHistory() doesn't use unique keys for each message
Fixed Scope labels are shown without translate wrapper
Fixed Wrong parameters handling in Core Helper formatDate()
Fixed Apostrophe in store name breaks Google Analytics tracking
Fixed Customer attribute prefix is not shown on frontend
Fixed Incorrect rounding for product with custom options (percent price)
Fixed Invoicing only part of products results in wrong totals calculation
Fixed Incorrect Row Total Calculation in Refund
- fixed rounding issues for partial Invoice and Refund
- refactored delta rounding
Fixed Filter by "Allow Countries" not working for Customer Address Form in the Backend
- checking added for set country to be in available list
Fixed There are sql-installs with empty string used as defaults for table columns, while column is not null able
Fixed Unable to translate "Note" in "Product Stock Options"
Fixed Various warning are displayed after creating shipment for 0 items
Fixed Invalid content in Content-header in the top of page during scrolling during order creation
Fixed "Online invoice" button present in backend when using Zero Subtotal Checkout
Fixed String cast type in in_array function
Fixed Newsletter template content should not disappear when "Show" / "Hide Editor" button was clicked
Fixed Import feature doesn't validate whether super_products_sku is existing or not



==== 1.6.x-devel-131783 ====

=== Major Highlights ===
Implemented new Layered Navigation price bucket algorithm
Added captcha functionality

=== Improvements ===
XmlConnect package release v22.1
Upgraded TinyMCE to v3.4.7

=== Fixes ===
Fixed Cannot place order with downloadable product and discount code using Paypal Express payment method
Fixed Product still out of stock after Stock Status reindex
Fixed No ability to reindex Catalog URL Rewrites, error is shown
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Save catalog price rule gives trace if full reindex has already started
Fixed Reindex requires notification is not shown for Stock Status when stock is updated for several products using Mass Action
Fixed Incorrect FedEx's shipping rates (in case with non-US country origin)
Fixed After partial reindex MSRP value is not applied (not viewed) in catalog during mass update action
Fixed Wrong stock reindex on catalog if partial reindex done after full reindex started
Fixed In error message string "already exists." written twice, when trying to save Product Tax Class with the same name
Fixed Wrong stock reindex on catalog if partial reindex done after full reindex started
Fixed Slow checkout with non-flushed cache



==== 1.6.x-devel-130478 ====
Fixed Bundle product total is incorrect in Customization block
Fixed Special price isn't considered for bundle dynamic products in "Your Customization" block
Fixed Situation when any amount of duplicate reindex process can be running at one time
Fixed Error with Advanced Search (in case with Date Attribute)
Fixed Product Flat Data index isn't marked as "Reindex Required" after importing products when Flat Catalog is enabled
Fixed User can't change root category for the store
Fixed JS error causes the overwrite of Title field in PayPal Advanced configuration
Fixed Mass action doesn't partially reindex catalog for product name/description
Fixed Remove hint about $1 auth amount from informational message text (PayflowLink configuration)
Fixed Mass action doesn't partially reindex catalog for product prices
Fixed PayPal Payments Advanced works with $0 Auth instead of Full Auth
Fixed Impossible to place Order using "Pay with PayPal" button from PayPal Payments Advanced iframe
Fixed Mass action doesn't partially reindex catalog search for product if searchable attribute was updated
Fixed "Please wait" AJAX screen doesn't appear in the middle of the page
Fixed Checkout link on frontend is always referenced as http
Fixed GET request is incorrectly formed during category creation
- adjusted assertion to determine last viewed store
Fixed Display of Tier Pricing with Configurable Products
- added functionality to dynamically update tier prices accordingly to chosen product configuration
Fixed Google Analytics e-commerce tracking not working
Fixed URL key isn't used while product save
Fixed Added validation class to 'Qty increments'
Fixed Entered from admin customer date 1970 (or less) is saved as 2070 (or less)
Fixed cUrl resource must be closed after checking it for errors, not before
Fixed Exception while products mass update attributes in backend
Fixed Impossible to place Order using Pay with PayPal button from PayflowLink iframe, when Payment Action is Sale
Fixed No ability to reindex Catalog URL Rewrites, error is shown
Fixed Package with Core dependency



==== 1.6.x-devel-129596 ====
Fixed Stock Availability isn't updated if 1: Run Price Reindex 2: Update Stock Availability on product with mass action/single product
Fixed PayPal Payments Advanced update descriptions
Fixed Blank page instead shopping cart page when compilation and PSC are enabled
Fixed Unable to save redirect URL with special characters in search terms
Fixed Attribute Set field should have client-side validation and appropriate information message
Fixed "Localhost" isn't a valid domain name for installation
Fixed Iframe for PayPal Payments Advanced is not loaded
Fixed Retain the selected tab on editing CMS page
Fixed Payflow Link Express Checkout (pay with PayPal button) payment
Fixed Wrong number of reindex options is displayed
Fixed Wrong phpDocs for Varien_Db_Select
Fixed JavaScript calendar date range
- fixed JS calendar behavior to use 4-digits year format
Fixed Performance issue connected with sales rules on adding product to cart
Fixed DHL same error message appears several times
Fixed Item Status says "Mixed" when an order has been completed, should say "Shipped"
Fixed Product option title is absent in backend order page
Fixed Incorrect items number during multi shipping checkout
Fixed User name displays differently in the unsuccessful message and in the text field label (log in form)
Fixed If one or more indexers have Update Required = Yes and all Status = READY for all indexers than there is no notification for user to do reindex action
Fixed No space between Address line 1 and line 2 in Shipping Label (in case with FedEx)



==== 1.6.x-devel-128838 ====

=== Improvements ===
Indexers refactoring

=== Changes ===
Implemented localized PayPal settings for Japan
Added PayPal Payments Advanced

=== Fixes ===
Fixed JS works depends on the position attributes of the product
Fixed Char set encoding is out-of-date in Settlement reports
Fixed Settlement reports can't be downloaded if in merchant's account 'Settlement file' is set to 6.0 version
Fixed Unable to login when secure and unsecure urls are different
Fixed Customer session lost when using different domain/subdomain names for secure and unsecure urls
Fixed "Most Viewed" reports ignore Store View switcher
Fixed Long FPT name (and product name) doesn't fit into "My cart" block
Fixed Paypal IPN post back failure
Fixed Customer was unable to receive newsletters when it was created via backend
Fixed Wrong Comments History in notification of order creation/cancellation
Fixed Non escaped string causes javascript error
Fixed Unable to view pictures during product editing
Fixed Ampersand is saved incorrect in attribute label
Fixed IE8: JS error appears after pressing 'Add new rule' in catalog price rules menu
Fixed Exception after sorting newsletter queue
Fixed Customer is not able to log in from URL without "www" in some cases
Fixed SQL error on category view with enabled and configured FPT
Fixed Automatic reindexing based on matched events doesn't change "Status" and "Last Run" columns at process list grid
Fixed Performance issue with Magento Compiler + APC results in too many I/O calls
Fixed Website Administrator is able to change default values
Fixed Some of wishlist blocks and templates still treat the collection of wishlist items as collection of products
Fixed Unnecessary comments in "Share Wishlist" email



==== 1.6.1.0 ====

=== Major Highlights ===
Added two-step password reset flow

=== Improvements ===
XmlConnect package release v22.0
Added support for using Shift-Click to select a range of grid rows when clicking check boxes
Added ability to register during checkout when using PayPal Express
Updated PayflowLink HSS user interface in checkout
"Add to Wishlist", "Add to Compare" were added on the Product Details Page for configurable, bundled and downloadable products
Updated webservices API

=== Changes ===
TheFind integration was removed
Google Optimizer was removed (it will be supported as a core extension)
Improved how discounts are applied to sub products

=== Fixes ===
Fixed Incorrect tax summary if taxes applied has different priorities
Fixed Shipping method extension after disable module returns error
Fixed Approved Review of a product is not displayed in the catalog
Fixed Special price is not considered for bundle dynamic products in "Your Customization" block
Fixed Incorrect behavior of changing quantity for composite products in Wishlist tab of customer's page in backend
Fixed MAP: Exc. Tax. amount is not shown on product's page when set apply map = 'On Gesture'
Fixed There has been an error processing your request is displayed by searching in Manage Checkout Terms and Conditions
Fixed Button Reorder is absent when Order contains Configurable product
Fixed Unable to place order if several tax rates with different priorities applied to bundle product
Fixed Incorrect Tracking Request to shipping carrier (in case with FedEx)
Fixed 'Click for price' not clickable after pressing 'Review' link in category
Fixed XML Connect: Impossible to submit application
Fixed MAP: with IE8 JS error appears in catalog
Fixed Error message appears after successful checkout with PayPal Express Checkout on IE9
Fixed Incorrect invoice document creation behaviour for bundle dynamic product
Fixed XML Connect: Impossible to save template
Fixed Wrong focusing in WYSIWYG on IE9, impossible to save data after inserting content
Fixed Unable to set zero price for item in bundle product
Fixed Incorrect tax summary if several tax rates with different priorities applied to bundle product
Fixed Unable to create order from backend if Tax Calculation Method Based On = Unit Price/Row Total
Fixed Incorrect Tracking Request to shipping carrier (in case with FedEx)
Fixed Incorrect tax summary for partial documents if Tax Calculation Method Based On = Row Total/Unit Price
Fixed Problems with partial authorization process (Authorize.net) during Admin Order creation
Fixed Incorrect HTML markup of Installer page in IE7 and IE9
Fixed "Apply Rules" button works incorrect in some cases
Fixed Incorrect behavior of changing quantity for composite products in Wishlist tab of customer's page in backend
Fixed Incorrect tax summary if product prices exclude tax
Fixed Redirect to blank page, when click Add Wishlist on the Bundle product page
Fixed Reviews not showing in category list page
Fixed QTY is wrong calculated for Bundle, Virtual, Simple, Configurable, Downloadable products after editing them in wishlist
Fixed Customer is redirected to shopping cart page instead to the "Ship to Multiple Addresses" page after login or register as a new customer
Fixed Configurable product with selected option is deleted from wishlist after updating another configurable product
Fixed After redirecting to product using tag 'click for price' doesn't work
Fixed "Notify for Quantity Below" doesn't work
Fixed Pending Reviews RSS doesn't show reviews, created for products, that are assigned not to Main Website
Fixed Authorize Direct Post: no successful notification about place order if do 'Edit' or 'Reorder'
Fixed Impossible to place Order with Payfowlink when Payment Action = Sale
Fixed Poll shows incorrect percentage
Fixed Message 'Cannot specify wishlist item.' is displayed by configuring products in wishlist in back-end
Fixed Billing Agreements: Order status is not updated if do actions from sandbox PayPal account
Fixed Additional authorization transaction is not displayed in Order's Transactions tab
Fixed Unable to update already created role by Admin
Fixed CDN Secure URL is used instead of non-secure
Fixed Attributes name disappeared during sorting
Fixed Typo in app/design/adminhtml/default/default/template/paypal/system/config/payflowlink/info.phtml
Fixed Report of Reviews shows all customer reviews when select certain user
Fixed Address Line Formats Incorrectly on PDF Invoices
Fixed Can't search transactions by order_id in manager.paypal.com
Fixed Wishlist Index Controller does unneeded logging of exception
Fixed Incorrect SQL generated in review product collection resource
Fixed Added shipping address rates collecting schedule for shipping method when shipping information step bypassed
Fixed Customer marked as guest in "Newsletter Subscribers" grid, after subscribing to newsletters in Google Checkout
Fixed Error is displayed by unchecking "Same As Billing Address" by creating order in admin
Fixed Tooltip doesn't appear if you put mouse pointer in to disabled package type field (in case with USPS Domestic)
Fixed Unable to select custom theme with underscores in name when creating a widget instance
Fixed When Redirect to Shopping Cart = No, choosing Remove item from shopping cart sidebar while editing an item leads to endless redirect loop
Fixed Saved CC form is not displayed, when there are no other available payment methods except Saved CC
Fixed It's impossible to create Catalog Price Rule
Fixed Fatal error on Multiple Addresses Checkout
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Stock item product getter not correspond to product setter
- added method getProduct()
Fixed Admin user interface: mistakes in labels names
Fixed Typo in Mage_Eav_Model_Resource_Entity_Attribute_Option model
Fixed Billing Agreement error
Fixed Payflow Link UI Changes
Fixed 'Website Payments Pro' impossible to place order during onepage checkout
Fixed Table rates works incorrect with asterisk
Fixed Typo in Category Resource Model
Fixed 3D secure with Saved CC works incorrectly
- removed unrelated message which told validation failed (even if it has actually succeeded) when trying to re-validate a card
Fixed Bug in Role Permission
Fixed Orders placed via Google Checkout were not created on the Magento side
Fixed When using direct Export, the _super_product_sku and _super_product_option on the configurable product does not match
Fixed Composite product price in grid is displayed incorrectly with some currencies due to JS regexp problem
Fixed No error message on Payflow link iframe
Fixed Flex uploader elements overlaps hovering menu items in backend
Fixed Unable to upload images in Magento installed on local server
Fixed Configurable Products - Use Default (attribute name) does not work correctly on IE9
Fixed Capture failed when Verification Authorization Amount is set to Zero
Fixed Attribute is sorted like a string even when Input Validation for Store Owner is an Integer Number
Fixed Void and Cancel Order doesn't work (PayflowLink HSS)
Fixed Grand Total (Excl Tax) with negative value displays in the printed Credit Memo
Fixed Resource model of Media module is wrongly declared
Fixed Constraint violation with core_cache_tag table
Fixed Misprint in \downloader\lib\Mage\Connect\Validator.php
Fixed XMLRPC API attribute status changing
Fixed Typo in Mage_Rss_Block_Catalog_Category::_toHtml() method
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed SSL is not used for links in email templates when admin area is configured to use HTTPS
Fixed Incorrect style on product page
Fixed Error is displayed by editing product or by creating product on back-end in IE8
Fixed Catalog price rules for composite products changes
Fixed Moving modules to the correct place
Fixed Wishlist shows items per store scope, not website
Fixed Products in Wishlist disappears, when Store View is changed
Fixed Wrong Comments History in notification of order creation/cancellation 
Fixed In AJAX popup fields "From" and "To" have behavior as mandatory fields
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed Product price lower than 0 (after catalog price rule applying)
Fixed Google Checkout throws error if Zip Range is used for Tax Rate
- changed part of XML request to Google responsible for postal codes
- made changes to correctly fetch tax rules for postal code ranges
Fixed Website config object is not being cached
Fixed Select groups in grid view doesn't work under IE7
Fixed No products name in Popular tags report file .csv
Fixed Qty Increments should work when it was defined in the default scope configuration
Fixed Products in catalog displays as "out of stock"
Fixed "Get help for this page" in each tab under System->Configuration links to the same help page
Fixed Unable to translate submenu
Fixed Redirect to main page of front-end during deleting Product Tax Class which is used in Tax Rule
Fixed Redirect to base URL should consider full request URI string
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Problem of generation URL between different domains
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit Order without creating new one functionality saves invalid changes in non-default customer address attributes
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Admin can Reorder order with status On Hold
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Tax not displaying on PayPal side for Express orders
Fixed Wishlist: Not configured grouped product has unneeded link "Show Details"
Fixed Removed the ability to work with customise admin url through the parameter base_url
Fixed Roles not displaying selected resources
Fixed Unable to use Import when compiler is enabled
Fixed Missing Translation Capability in Transactional Email Variable
Fixed productConfigure is undefined error is occurred during creation Order in Backend in IE8 browser
Fixed Zend Full Page Cache. Lifetime of the cookie is not equal to specified on "Cookie Lifetime" field
Fixed Incorrect price values for Bundle Product
Fixed Link does not pass validation if ends with .html
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect reports with updated_at filter
Fixed paypal_payment_transaction_clean job takes credentials form default config instead of website for Payflow Link
Fixed Wrong schedule time setup for paypal_payment_transaction_clean job for Payflow Link
Fixed Backend Error message "SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'qwe' for key 2" appears after saving new Email Template with existing name
Fixed Rule Conditions logic
Fixed Error appears after Customer Group saving with name length more than 32
Fixed Category product index run time
Fixed Sidebar cart is missing composite product options on category page
Fixed Missed validation for space character at the begin of unique fields
- improved validation of Attribute Set Name and validation of unique fields in Mage_Core_Model_Resource_Db_Abstract class
Fixed Ability to input uppercase, space, specials symbols in Order Status Code
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed No ability to create Shipping Label with "plus-four codes" Zip Code (in case with USPS Domestic)
Fixed Changing language twice -> Error 404
Fixed The sort order in products page doesn't work
Fixed When a grouped product with configured price=0 is added to the wishlist and shared, adding the product to the cart leads to 404 error
Fixed Media Saves Incorrect Cached Config
- added options that disallow saving cache
Fixed Bundle Product items shows randomly instead of according to option
Fixed Ajax loader does not appears after click on Verify Card on Payflow Link
Fixed "Google Checkout - Carrier" in Magento backend as shipping method rather than the actual shipping method chosen
Fixed JavaScript error appears in checkout because of PSC after press 'Proceed to Checkout'
Fixed Admin user interface: mistakes in labels names
Fixed Problems with grid sorting on edit customer backend page
Fixed It is possible to change the price of the Bundle product from fixed to the dynamic at my store
Fixed Set special price via Catalog Product API is not working
Fixed Price is wrong calculated for bundle product with a zero price for its items on product details page
- subitem price calculation were fixed
Fixed Layout issue appears in IE9 on the grids (example Customers)
Fixed Impossible to press 'Continue' button to place in onepage
Fixed "Add to Wishlist", "Add to Compare" aren't presented for Configurable, bundle, downloadable, simple products on Product Details Page
Fixed Register during checkout with PayPal Express Checkout
Fixed Extension Packager does not read recursive directory if include expression use file mask
Fixed Newsletter Subscription Confirmation Message
Fixed Discount is wrong calculated for Shopping Cart Price Rules when some of them created with Coupon and another without Coupon
Fixed Subtotal (Incl.Tax) on invoices must not include tax applied to shipping amount
- shippingTax amount were excluded from subTotal value
Fixed "Maximum shipping amount allowed to refund" message shows amount excl. tax if Display Shipping Amount set to Including Tax
- adjusted function to include tax into allowed amount for shipping refund
Fixed Display Out of Stock Products must not be considered during admin order creation
Fixed Check box is not working correctly under "prices" of the Bundle products
Fixed CSS class missing
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Website config object is not being cached
- added functionality for memcache backend to split down data that is larger than slab size into chunks
Fixed Removed the ability to work with base_url
Fixed Custom design should be updated via import functionality
Fixed JS error during onepage checkout
Fixed Unable to translate "First name" and "Last name" fields on "Create an Account" page
Fixed After upgrading  dashboard "Top 5 Search Terms" grid doesn't show search terms



==== 1.6.1.0-rc1 ====

=== Major Highlights ===
Added two-step password reset flow

=== Improvements ===
XmlConnect package release v22.0
Added support for using Shift-Click to select a range of grid rows when clicking check boxes
Added ability to register during checkout when using PayPal Express
Updated PayflowLink HSS user interface in checkout
"Add to Wishlist", "Add to Compare" were added on the Product Details Page for configurable, bundled and downloadable products

=== Changes ===
TheFind integration was removed
Google Optimizer was removed (it will be supported as a core extension)
Improved how discounts are applied to sub products

=== Fixes ===
Fixed Incorrect behavior of changing quantity for composite products in Wishlist tab of customer's page in backend
Fixed Incorrect tax summary if product prices exclude tax
Fixed Redirect to blank page, when click Add Wishlist on the Bundle product page
Fixed Reviews not showing in category list page
Fixed QTY is wrong calculated for Bundle, Virtual, Simple, Configurable, Downloadable products after editing them in wishlist
Fixed Customer is redirected to shopping cart page instead to the "Ship to Multiple Addresses" page after login or register as a new customer
Fixed Configurable product with selected option is deleted from wishlist after updating another configurable product
Fixed After redirecting to product using tag 'click for price' doesn't work
Fixed "Notify for Quantity Below" doesn't work
Fixed Pending Reviews RSS doesn't show reviews, created for products, that are assigned not to Main Website
Fixed Authorize Direct Post: no successful notification about place order if do 'Edit' or 'Reorder'
Fixed Impossible to place Order with Payfowlink when Payment Action = Sale
Fixed Poll shows incorrect percentage
Fixed Message 'Cannot specify wishlist item.' is displayed by configuring products in wishlist in back-end
Fixed Billing Agreements: Order status is not updated if do actions from sandbox PayPal account
Fixed Additional authorization transaction is not displayed in Order's Transactions tab
Fixed Unable to update already created role by Admin
Fixed CDN Secure URL is used instead of non-secure
Fixed Attributes name disappeared during sorting
Fixed Typo in app/design/adminhtml/default/default/template/paypal/system/config/payflowlink/info.phtml
Fixed Report of Reviews shows all customer reviews when select certain user
Fixed Address Line Formats Incorrectly on PDF Invoices
Fixed Can't search transactions by order_id in manager.paypal.com
Fixed Wishlist Index Controller does unneeded logging of exception
Fixed Incorrect SQL generated in review product collection resource
Fixed Added shipping address rates collecting schedule for shipping method when shipping information step bypassed
Fixed Customer marked as guest in "Newsletter Subscribers" grid, after subscribing to newsletters in Google Checkout
Fixed Error is displayed by unchecking "Same As Billing Address" by creating order in admin
Fixed Tooltip doesn't appear if you put mouse pointer in to disabled package type field (in case with USPS Domestic)
Fixed Unable to select custom theme with underscores in name when creating a widget instance
Fixed When Redirect to Shopping Cart = No, choosing Remove item from shopping cart sidebar while editing an item leads to endless redirect loop
Fixed Saved CC form is not displayed, when there are no other available payment methods except Saved CC
Fixed It's impossible to create Catalog Price Rule
Fixed Fatal error on Multiple Addresses Checkout
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Stock item product getter not correspond to product setter
- added method getProduct()
Fixed Admin user interface: mistakes in labels names
Fixed Typo in Mage_Eav_Model_Resource_Entity_Attribute_Option model
Fixed Billing Agreement error
Fixed Payflow Link UI Changes
Fixed 'Website Payments Pro' impossible to place order during onepage checkout
Fixed Table rates works incorrect with asterisk
Fixed Typo in Category Resource Model
Fixed 3D secure with Saved CC works incorrectly
- removed unrelated message which told validation failed (even if it has actually succeeded) when trying to re-validate a card
Fixed Bug in Role Permission
Fixed Orders placed via Google Checkout were not created on the Magento side
Fixed When using direct Export, the _super_product_sku and _super_product_option on the configurable product does not match
Fixed Composite product price in grid is displayed incorrectly with some currencies due to JS regexp problem
Fixed No error message on Payflow link iframe
Fixed Flex uploader elements overlaps hovering menu items in backend
Fixed Unable to upload images in Magento installed on local server
Fixed Configurable Products - Use Default (attribute name) does not work correctly on IE9
Fixed Capture failed when Verification Authorization Amount is set to Zero
Fixed Attribute is sorted like a string even when Input Validation for Store Owner is an Integer Number
Fixed Void and Cancel Order doesn't work (PayflowLink HSS)
Fixed Grand Total (Excl Tax) with negative value displays in the printed Credit Memo
Fixed Resource model of Media module is wrongly declared
Fixed Constraint violation with core_cache_tag table
Fixed Misprint in \downloader\lib\Mage\Connect\Validator.php
Fixed XMLRPC API attribute status changing
Fixed Typo in Mage_Rss_Block_Catalog_Category::_toHtml() method
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed SSL is not used for links in email templates when admin area is configured to use HTTPS
Fixed Incorrect style on product page
Fixed Error is displayed by editing product or by creating product on back-end in IE8
Fixed Catalog price rules for composite products changes
Fixed Moving modules to the correct place
Fixed Wishlist shows items per store scope, not website
Fixed Products in Wishlist disappears, when Store View is changed
Fixed Wrong Comments History in notification of order creation/cancellation 
Fixed In AJAX popup fields "From" and "To" have behavior as mandatory fields
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed Product price lower than 0 (after catalog price rule applying)
Fixed Google Checkout throws error if Zip Range is used for Tax Rate
- changed part of XML request to Google responsible for postal codes
- made changes to correctly fetch tax rules for postal code ranges
Fixed Website config object is not being cached
Fixed Select groups in grid view doesn't work under IE7
Fixed No products name in Popular tags report file .csv
Fixed Qty Increments should work when it was defined in the default scope configuration
Fixed Products in catalog displays as "out of stock"
Fixed "Get help for this page" in each tab under System->Configuration links to the same help page
Fixed Unable to translate submenu
Fixed Redirect to main page of front-end during deleting Product Tax Class which is used in Tax Rule
Fixed Redirect to base URL should consider full request URI string
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Problem of generation URL between different domains
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit Order without creating new one functionality saves invalid changes in non-default customer address attributes
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Admin can Reorder order with status On Hold
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Tax not displaying on PayPal side for Express orders
Fixed Wishlist: Not configured grouped product has unneeded link "Show Details"
Fixed Removed the ability to work with customise admin url through the parameter base_url
Fixed Roles not displaying selected resources
Fixed Unable to use Import when compiler is enabled
Fixed Missing Translation Capability in Transactional Email Variable
Fixed productConfigure is undefined error is occurred during creation Order in Backend in IE8 browser
Fixed Zend Full Page Cache. Lifetime of the cookie is not equal to specified on "Cookie Lifetime" field
Fixed Incorrect price values for Bundle Product
Fixed Link does not pass validation if ends with .html
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect reports with updated_at filter
Fixed paypal_payment_transaction_clean job takes credentials form default config instead of website for Payflow Link
Fixed Wrong schedule time setup for paypal_payment_transaction_clean job for Payflow Link
Fixed Backend Error message "SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'qwe' for key 2" appears after saving new Email Template with existing name
Fixed Rule Conditions logic
Fixed Error appears after Customer Group saving with name length more than 32
Fixed Category product index run time
Fixed Sidebar cart is missing composite product options on category page
Fixed Missed validation for space character at the begin of unique fields
- improved validation of Attribute Set Name and validation of unique fields in Mage_Core_Model_Resource_Db_Abstract class
Fixed Ability to input uppercase, space, specials symbols in Order Status Code
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed No ability to create Shipping Label with "plus-four codes" Zip Code (in case with USPS Domestic)
Fixed Changing language twice -> Error 404
Fixed The sort order in products page doesn't work
Fixed When a grouped product with configured price=0 is added to the wishlist and shared, adding the product to the cart leads to 404 error
Fixed Media Saves Incorrect Cached Config
- added options that disallow saving cache
Fixed Bundle Product items shows randomly instead of according to option
Fixed Ajax loader does not appears after click on Verify Card on Payflow Link
Fixed "Google Checkout - Carrier" in Magento backend as shipping method rather than the actual shipping method chosen
Fixed JavaScript error appears in checkout because of PSC after press 'Proceed to Checkout'
Fixed Admin user interface: mistakes in labels names
Fixed Problems with grid sorting on edit customer backend page
Fixed It is possible to change the price of the Bundle product from fixed to the dynamic at my store
Fixed Set special price via Catalog Product API is not working
Fixed Price is wrong calculated for bundle product with a zero price for its items on product details page
- subitem price calculation were fixed
Fixed Layout issue appears in IE9 on the grids (example Customers)
Fixed Impossible to press 'Continue' button to place in onepage
Fixed "Add to Wishlist", "Add to Compare" aren't presented for Configurable, bundle, downloadable, simple products on Product Details Page
Fixed Register during checkout with PayPal Express Checkout
Fixed Extension Packager does not read recursive directory if include expression use file mask
Fixed Newsletter Subscription Confirmation Message
Fixed Discount is wrong calculated for Shopping Cart Price Rules when some of them created with Coupon and another without Coupon
Fixed Subtotal (Incl.Tax) on invoices must not include tax applied to shipping amount
- shippingTax amount were excluded from subTotal value
Fixed "Maximum shipping amount allowed to refund" message shows amount excl. tax if Display Shipping Amount set to Including Tax
- adjusted function to include tax into allowed amount for shipping refund
Fixed Display Out of Stock Products must not be considered during admin order creation
Fixed Check box is not working correctly under "prices" of the Bundle products
Fixed CSS class missing
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Website config object is not being cached
- added functionality for memcache backend to split down data that is larger than slab size into chunks
Fixed Removed the ability to work with base_url
Fixed Custom design should be updated via import functionality
Fixed JS error during onepage checkout
Fixed Unable to translate "First name" and "Last name" fields on "Create an Account" page
Fixed After upgrading  dashboard "Top 5 Search Terms" grid doesn't show search terms



==== 1.6.1.0-beta1 ====

=== Major Highlights ===
Added two-step password reset flow

=== Improvements ===
Added support for using Shift-Click to select a range of grid rows when clicking check boxes
Added ability to register during checkout when using PayPal Express
Updated PayflowLink HSS user interface in checkout
"Add to Wishlist", "Add to Compare" were added on the Product Details Page for configurable, bundled and downloadable products

=== Changes ===
TheFind integration was removed
Google Optimizer was removed (it will be supported as a core extension)
Improved how discounts are applied to sub products 

=== Fixes ===
Fixed Saved CC form is not displayed, when there are no other available payment methods except Saved CC
Fixed It's impossible to create Catalog Price Rule
Fixed Fatal error on Multiple Addresses Checkout
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Stock item product getter not correspond to product setter
- added method getProduct()
Fixed Admin user interface: mistakes in labels names
Fixed Typo in Mage_Eav_Model_Resource_Entity_Attribute_Option model
Fixed Billing Agreement error
Fixed Payflow Link UI Changes
Fixed 'Website Payments Pro' impossible to place order during onepage checkout
Fixed Table rates works incorrect with asterisk
Fixed Typo in Category Resource Model
Fixed 3D secure with Saved CC works incorrectly
- removed unrelated message which told validation failed (even if it has actually succeeded) when trying to re-validate a card
Fixed Bug in Role Permission
Fixed Orders placed via Google Checkout were not created on the Magento side
Fixed When using direct Export, the _super_product_sku and _super_product_option on the configurable product does not match
Fixed Composite product price in grid is displayed incorrectly with some currencies due to JS regexp problem
Fixed No error message on Payflow link iframe
Fixed Flex uploader elements overlaps hovering menu items in backend
Fixed Unable to upload images in Magento installed on local server
Fixed Configurable Products - Use Default (attribute name) does not work correctly on IE9
Fixed Capture failed when Verification Authorization Amount is set to Zero
Fixed Attribute is sorted like a string even when Input Validation for Store Owner is an Integer Number
Fixed Void and Cancel Order doesn't work (PayflowLink HSS)
Fixed Grand Total (Excl Tax) with negative value displays in the printed Credit Memo
Fixed Resource model of Media module is wrongly declared
Fixed Constraint violation with core_cache_tag table
Fixed Misprint in \downloader\lib\Mage\Connect\Validator.php
Fixed XMLRPC API attribute status changing
Fixed Typo in Mage_Rss_Block_Catalog_Category::_toHtml() method
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed SSL is not used for links in email templates when admin area is configured to use HTTPS
Fixed Incorrect style on product page
Fixed Error is displayed by editing product or by creating product on back-end in IE8
Fixed Catalog price rules for composite products changes
Fixed Moving modules to the correct place
Fixed Wishlist shows items per store scope, not website
Fixed Products in Wishlist disappears, when Store View is changed
Fixed Wrong Comments History in notification of order creation/cancellation 
Fixed In AJAX popup fields "From" and "To" have behavior as mandatory fields
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed Product price lower than 0 (after catalog price rule applying)
Fixed Google Checkout throws error if Zip Range is used for Tax Rate
- changed part of XML request to Google responsible for postal codes
- made changes to correctly fetch tax rules for postal code ranges
Fixed Website config object is not being cached
Fixed Select groups in grid view doesn't work under IE7
Fixed No products name in Popular tags report file .csv
Fixed Qty Increments should work when it was defined in the default scope configuration
Fixed Products in catalog displays as "out of stock"
Fixed "Get help for this page" in each tab under System->Configuration links to the same help page
Fixed Unable to translate submenu
Fixed Redirect to main page of front-end during deleting Product Tax Class which is used in Tax Rule
Fixed Redirect to base URL should consider full request URI string
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Problem of generation URL between different domains
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit Order without creating new one functionality saves invalid changes in non-default customer address attributes
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Admin can Reorder order with status On Hold
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Tax not displaying on PayPal side for Express orders
Fixed Wishlist: Not configured grouped product has unneeded link "Show Details"
Fixed Removed the ability to work with customise admin url through the parameter base_url
Fixed Roles not displaying selected resources
Fixed Unable to use Import when compiler is enabled
Fixed Missing Translation Capability in Transactional Email Variable
Fixed productConfigure is undefined error is occurred during creation Order in Backend in IE8 browser
Fixed Zend Full Page Cache. Lifetime of the cookie is not equal to specified on "Cookie Lifetime" field
Fixed Incorrect price values for Bundle Product
Fixed Link does not pass validation if ends with .html
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect reports with updated_at filter
Fixed paypal_payment_transaction_clean job takes credentials form default config instead of website for Payflow Link
Fixed Wrong schedule time setup for paypal_payment_transaction_clean job for Payflow Link
Fixed Backend Error message "SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'qwe' for key 2" appears after saving new Email Template with existing name
Fixed Rule Conditions logic
Fixed Error appears after Customer Group saving with name length more than 32
Fixed Category product index run time
Fixed Sidebar cart is missing composite product options on category page
Fixed Missed validation for space character at the begin of unique fields
- improved validation of Attribute Set Name and validation of unique fields in Mage_Core_Model_Resource_Db_Abstract class
Fixed Ability to input uppercase, space, specials symbols in Order Status Code
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed No ability to create Shipping Label with "plus-four codes" Zip Code (in case with USPS Domestic)
Fixed Changing language twice -> Error 404
Fixed The sort order in products page doesn't work
Fixed When a grouped product with configured price=0 is added to the wishlist and shared, adding the product to the cart leads to 404 error
Fixed Media Saves Incorrect Cached Config
- added options that disallow saving cache
Fixed Bundle Product items shows randomly instead of according to option
Fixed Unable to place order with Payflow Link if store credit or reward point applied
Fixed Ajax loader does not appears after click on Verify Card on Payflow Link
Fixed "Google Checkout - Carrier" in Magento backend as shipping method rather than the actual shipping method chosen
Fixed JavaScript error appears in checkout because of PSC after press 'Proceed to Checkout'
Fixed Admin user interface: mistakes in labels names
Fixed Problems with grid sorting on edit customer backend page
Fixed It is possible to change the price of the Bundle product from fixed to the dynamic at my store
Fixed Set special price via Catalog Product API is not working
Fixed Price is wrong calculated for bundle product with a zero price for its items on product details page
- subitem price calculation were fixed
Fixed Layout issue appears in IE9 on the grids (example Customers)
Fixed Impossible to press 'Continue' button to place in onepage
Fixed "Add to Wishlist", "Add to Compare" aren't presented for Configurable, bundle, downloadable, simple products on Product Details Page
Fixed Register during checkout with PayPal Express Checkout
Fixed Extension Packager does not read recursive directory if include expression use file mask
Fixed Newsletter Subscription Confirmation Message
Fixed Discount is wrong calculated for Shopping Cart Price Rules when some of them created with Coupon and another without Coupon
Fixed Subtotal (Incl.Tax) on invoices must not include tax applied to shipping amount
- shippingTax amount were excluded from subTotal value
Fixed "Maximum shipping amount allowed to refund" message shows amount excl. tax if Display Shipping Amount set to Including Tax
- adjusted function to include tax into allowed amount for shipping refund
Fixed Display Out of Stock Products must not be considered during admin order creation
Fixed Check box is not working correctly under "prices" of the Bundle products.
Fixed CSS class missing
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Website config object is not being cached
- added functionality for memcache backend to split down data that is larger than slab size into chunks
Fixed Removed the ability to work with base_url
Fixed Custom design should be updated via import functionality
Fixed JS error during onepage checkout
Fixed Unable to translate "First name" and "Last name" fields on "Create an Account" page
Fixed After upgrading  dashboard "Top 5 Search Terms" grid doesn't show search terms



==== 1.6.1.0-alpha1 ====

=== Major Highlights ===
Added two-step password reset flow

=== Improvements ===
Added support for using Shift-Click to select a range of grid rows when clicking check boxes
Added ability to register during checkout when using PayPal Express
Updated PayflowLink HSS user interface in checkout
"Add to Wishlist", "Add to Compare" were added on the Product Details Page for configurable, bundled and downloadable products

=== Changes ===
TheFind integration was removed
Google Optimizer was removed (it will be supported as a core extension)
Improved how discounts are applied to sub products 

=== Fixes ===
Fixed When using direct Export, the _super_product_sku and _super_product_option on the configurable product does not match
Fixed Composite product price in grid is displayed incorrectly with some currencies due to JS regexp problem
Fixed No error message on Payflow link iframe
Fixed Flex uploader elements overlaps hovering menu items in backend
Fixed Unable to upload images in Magento installed on local server
Fixed Configurable Products - Use Default (attribute name) does not work correctly on IE9
Fixed Capture failed when Verification Authorization Amount is set to Zero
Fixed Attribute is sorted like a string even when Input Validation for Store Owner is an Integer Number
Fixed Void and Cancel Order doesn't work (PayflowLink HSS)
Fixed Grand Total (Excl Tax) with negative value displays in the printed Credit Memo
Fixed Resource model of Media module is wrongly declared
Fixed Constraint violation with core_cache_tag table
Fixed Misprint in \downloader\lib\Mage\Connect\Validator.php
Fixed XMLRPC API attribute status changing
Fixed Typo in Mage_Rss_Block_Catalog_Category::_toHtml() method
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed SSL is not used for links in email templates when admin area is configured to use HTTPS
Fixed Incorrect style on product page
Fixed Error is displayed by editing product or by creating product on back-end in IE8
Fixed Catalog price rules for composite products changes
Fixed Moving modules to the correct place
Fixed Wishlist shows items per store scope, not website
Fixed Products in Wishlist disappears, when Store View is changed
Fixed Wrong Comments History in notification of order creation/cancellation 
Fixed In AJAX popup fields "From" and "To" have behavior as mandatory fields
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed Product price lower than 0 (after catalog price rule applying)
Fixed Google Checkout throws error if Zip Range is used for Tax Rate
- changed part of XML request to Google responsible for postal codes
- made changes to correctly fetch tax rules for postal code ranges
Fixed Website config object is not being cached
Fixed Select groups in grid view doesn't work under IE7
Fixed No products name in Popular tags report file .csv
Fixed Qty Increments should work when it was defined in the default scope configuration
Fixed Products in catalog displays as "out of stock"
Fixed "Get help for this page" in each tab under System->Configuration links to the same help page
Fixed Unable to translate submenu
Fixed Redirect to main page of front-end during deleting Product Tax Class which is used in Tax Rule
Fixed Redirect to base URL should consider full request URI string
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Problem of generation URL between different domains
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit Order without creating new one functionality saves invalid changes in non-default customer address attributes
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Admin can Reorder order with status On Hold
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Tax not displaying on PayPal side for Express orders
Fixed Wishlist: Not configured grouped product has unneeded link "Show Details"
Fixed Removed the ability to work with customise admin url through the parameter base_url
Fixed Roles not displaying selected resources
Fixed Unable to use Import when compiler is enabled
Fixed Missing Translation Capability in Transactional Email Variable
Fixed productConfigure is undefined error is occurred during creation Order in Backend in IE8 browser
Fixed Zend Full Page Cache. Lifetime of the cookie is not equal to specified on "Cookie Lifetime" field
Fixed Incorrect price values for Bundle Product
Fixed Link does not pass validation if ends with .html
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect reports with updated_at filter
Fixed paypal_payment_transaction_clean job takes credentials form default config instead of website for Payflow Link
Fixed Wrong schedule time setup for paypal_payment_transaction_clean job for Payflow Link
Fixed Backend Error message "SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'qwe' for key 2" appears after saving new Email Template with existing name
Fixed Rule Conditions logic
Fixed Error appears after Customer Group saving with name length more than 32
Fixed Category product index run time
Fixed Sidebar cart is missing composite product options on category page
Fixed Missed validation for space character at the begin of unique fields
- improved validation of Attribute Set Name and validation of unique fields in Mage_Core_Model_Resource_Db_Abstract class
Fixed Ability to input uppercase, space, specials symbols in Order Status Code
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed No ability to create Shipping Label with "plus-four codes" Zip Code (in case with USPS Domestic)
Fixed Changing language twice -> Error 404
Fixed The sort order in products page doesn't work
Fixed When a grouped product with configured price=0 is added to the wishlist and shared, adding the product to the cart leads to 404 error
Fixed Media Saves Incorrect Cached Config
- added options that disallow saving cache
Fixed Bundle Product items shows randomly instead of according to option
Fixed Unable to place order with Payflow Link if store credit or reward point applied
Fixed Ajax loader does not appears after click on Verify Card on Payflow Link
Fixed "Google Checkout - Carrier" in Magento backend as shipping method rather than the actual shipping method chosen
Fixed JavaScript error appears in checkout because of PSC after press 'Proceed to Checkout'
Fixed Admin user interface: mistakes in labels names
Fixed Problems with grid sorting on edit customer backend page
Fixed It is possible to change the price of the Bundle product from fixed to the dynamic at my store
Fixed Set special price via Catalog Product API is not working
Fixed Price is wrong calculated for bundle product with a zero price for its items on product details page
- subitem price calculation were fixed
Fixed Layout issue appears in IE9 on the grids (example Customers)
Fixed Impossible to press 'Continue' button to place in onepage
Fixed "Add to Wishlist", "Add to Compare" aren't presented for Configurable, bundle, downloadable, simple products on Product Details Page
Fixed Register during checkout with PayPal Express Checkout
Fixed Extension Packager does not read recursive directory if include expression use file mask
Fixed Newsletter Subscription Confirmation Message
Fixed Discount is wrong calculated for Shopping Cart Price Rules when some of them created with Coupon and another without Coupon
Fixed Subtotal (Incl.Tax) on invoices must not include tax applied to shipping amount
- shippingTax amount were excluded from subTotal value
Fixed "Maximum shipping amount allowed to refund" message shows amount excl. tax if Display Shipping Amount set to Including Tax
- adjusted function to include tax into allowed amount for shipping refund
Fixed Display Out of Stock Products must not be considered during admin order creation
Fixed Check box is not working correctly under "prices" of the Bundle products.
Fixed CSS class missing
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Website config object is not being cached
- added functionality for memcache backend to split down data that is larger than slab size into chunks
Fixed Removed the ability to work with base_url
Fixed Custom design should be updated via import functionality
Fixed JS error during onepage checkout
Fixed Unable to translate "First name" and "Last name" fields on "Create an Account" page
Fixed After upgrading  dashboard "Top 5 Search Terms" grid doesn't show search terms



==== 1.6.x-devel-119961 ====

=== Fixes ===
Fixed Wrong Comments History in notification of order creation/cancellation 
Fixed In AJAX popup fields "From" and "To" have behavior as mandatory fields
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed Product price lower than 0 (after catalog price rule applying)
Fixed Google Checkout throws error if Zip Range is used for Tax Rate
- changed part of XML request to Google responsible for postal codes
- made changes to correctly fetch tax rules for postal code ranges
Fixed Website config object is not being cached
Fixed Select groups in grid view doesn't work under IE7
Fixed No products name in Popular tags report file .csv
Fixed Qty Increments should work when it was defined in the default scope configuration
Fixed Products in catalog displays as "out of stock"
Fixed "Get help for this page" in each tab under System->Configuration links to the same help page
Fixed Unable to translate submenu
Fixed Redirect to main page of front-end during deleting Product Tax Class which is used in Tax Rule
Fixed Redirect to base URL should consider full request URI string



==== 1.6.x-devel-119217 ====

=== Fixes ===
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Problem of generation URL between different domains
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit Order without creating new one functionality saves invalid changes in non-default customer address attributes
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Admin can Reorder order with status On Hold
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Tax not displaying on PayPal side for Express orders
Fixed Wishlist: Not configured grouped product has unneeded link "Show Details"
Fixed Removed the ability to work with customise admin url through the parameter base_url
Fixed Roles not displaying selected resources
Fixed Unable to use Import when compiler is enabled
Fixed Missing Translation Capability in Transactional Email Variable
Fixed productConfigure is undefined error is occurred during creation Order in Backend in IE8 browser
Fixed Zend Full Page Cache. Lifetime of the cookie is not equal to specified on "Cookie Lifetime" field
Fixed Incorrect price values for Bundle Product
Fixed Link does not pass validation if ends with .html
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect reports with updated_at filter
Fixed paypal_payment_transaction_clean job takes credentials form default config instead of website for Payflow Link
Fixed Wrong schedule time setup for paypal_payment_transaction_clean job for Payflow Link
Fixed Backend Error message "SQLSTATE[23000]: Integrity constraint violation: 1062 Duplicate entry 'qwe' for key 2" appears after saving new Email Template with existing name
Fixed Rule Conditions logic
Fixed Error appears after Customer Group saving with name length more than 32
Fixed Category product index run time
Fixed Sidebar cart is missing composite product options on category page
Fixed Missed validation for space character at the begin of unique fields
- improved validation of Attribute Set Name and validation of unique fields in Mage_Core_Model_Resource_Db_Abstract class
Fixed Ability to input uppercase, space, specials symbols in Order Status Code
Fixed Filter by Allow Countries not working for Customer Address Form in the Backend
Fixed No ability to create Shipping Label with "plus-four codes" Zip Code (in case with USPS Domestic)
Fixed Changing language twice -> Error 404
Fixed The sort order in products page doesn't work
Fixed When a grouped product with configured price=0 is added to the wishlist and shared, adding the product to the cart leads to 404 error
Fixed Media Saves Incorrect Cached Config
- added options that disallow saving cache
Fixed Bundle Product items shows randomly instead of according to option
Fixed Unable to place order with Payflow Link if store credit or reward point applied
Fixed Ajax loader does not appears after click on Verify Card on Payflow Link
Fixed "Google Checkout - Carrier" in Magento backend as shipping method rather than the actual shipping method chosen
Fixed JavaScript error appears in checkout because of PSC after press 'Proceed to Checkout'
Fixed Admin user interface: mistakes in labels names
Fixed Problems with grid sorting on edit customer backend page
Fixed It is possible to change the price of the Bundle product from fixed to the dynamic at my store
Fixed Set special price via Catalog Product API is not working
Fixed Price is wrong calculated for bundle product with a zero price for its items on product details page
- subitem price calculation were fixed
Fixed Layout issue appears in IE9 on the grids (example Customers)
Fixed Impossible to press 'Continue' button to place in onepage
Fixed "Add to Wishlist", "Add to Compare" aren't presented for Configurable, bundle, downloadable, simple products on Product Details Page
Fixed Register during checkout with PayPal Express Checkout
Fixed Extension Packager does not read recursive directory if include expression use file mask
Fixed Newsletter Subscription Confirmation Message
Fixed Discount is wrong calculated for Shopping Cart Price Rules when some of them created with Coupon and another without Coupon
Fixed Subtotal (Incl.Tax) on invoices must not include tax applied to shipping amount
- shippingTax amount were excluded from subTotal value
Fixed "Maximum shipping amount allowed to refund" message shows amount excl. tax if Display Shipping Amount set to Including Tax
- adjusted function to include tax into allowed amount for shipping refund
Fixed Display Out of Stock Products must not be considered during admin order creation
Fixed Check box is not working correctly under "prices" of the Bundle products.
Fixed CSS class missing
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Website config object is not being cached
- added functionality for memcache backend to split down data that is larger than slab size into chunks
Fixed Removed the ability to work with base_url
Fixed Custom design should be updated via import functionality
Fixed JS error during onepage checkout
Fixed Unable to translate "First name" and "Last name" fields on "Create an Account" page
Fixed After upgrading  dashboard "Top 5 Search Terms" grid doesn't show search terms



==== 1.6.0.0 ====

=== Major Highlights ===
Minimum Advertised Price
Persistent Shopping Cart
Shipping Integration with Label printing support

=== Improvements ===
XmlConnect package release v21
Order Payment Action for Express Checkout (PayPal)
- Added settings Authorization Honor Period and Order Valid Period into EC tab in the backend
- Automatically new authorize transaction created after order transaction
- Automatically cancel order after the expiration of Order Valid Period
- Automatically authorize transaction void\create after the expiration of Authorization Honor Period
Implemented Authorize.Net 'hold for review' status shows up as 'declined' in Magento
Add Dynamic sku option for configurable products
Moneybookers Multistore System Configuration
Moneybookers OBT Defaults
PrototypeJS upgraded to 1.7

=== Changes ===
Removed deprecation.js because its not compatible with prototype 1.7
Relations between models and resource models were revised for better support of multiple databases
- Varien_Db_Adapter_Pdo_Mysql revised
- Introduced Varien_Db_Adapter_Interface,  Varien_Db_Ddl_Table
- Introduced new classes named resource helpers
- Backwards comatibility and known issues
-- Error appears after Customer Group saving with name length more than 32
Deprecated GoogleBase module (http://googlemerchantblog.blogspot.com/2010/12/new-shopping-apis-and-deprecation-of.html)
- Google Shopping Extension is available for the replacement

=== Fixes ===
Fixed Google checkout shipping (merchant and carrier calculated) returns only default prices
Fixed Custom option prices for simple products are GLOBAL
- fixed website price scope for simple products when product is linked to few websites with separate store views
Fixed Custom Price for Bundled Product should be disabled in Admin Panel
Fixed Configurable products. Incorrect pricing with super attributes price in percents
- percentage of price is taken from final product price
Fixed Label of system Customer Attribute, that was changed, is not displayed
Fixed Taxes are not correctly calculated if bundle with dynamic price is about to partially return
Fixed No ability to create Shipping Labels with several packages (in case with decimals Qty of products)
Fixed Special symbols as search keywords return error page
Fixed Changes in URL rewrite suffix cannot be reverted
Fixed Taxes are not correctly calculated if bundle with dynamic price is about to partially return
Fixed Product is deleted from shopping cart by editing grouped product
Fixed Product view page doesn't reflect last visited category
Fixed Customer is linked in order even if it is deleted from Magento
Fixed Exception is shown when Email to a Friend page is opened using URL in case when this feature is disabled
Fixed Missing "?" placeholders in class Varien_Cache_Backend_Database
Fixed There are no server side validation of first character of Attribute Code (it should be letter)
Fixed Edit cart item return unnecessary error message
Fixed Product Custom Option values titles are not saved
Fixed Newsletters are not sent
Fixed Preview URL for CMS Pages template contain two question mark
Fixed Partial refund orders with downloadable products affect status of all downloadable links
Fixed AddToCart takes forever if a configurable has massive count of child products
Fixed Mage_Tag_IndexController::saveAction() contains business logic of creating tag relation
Fixed Frontend: If second customer logs in and does not select the "Remember Me" then the previous long-term cookie does not removes
Fixed Frontend: After new customer registration with "Remember Me" and pressing "Logout" the long-term cookie session doesn't apply if in configuration on backend ""Remember Me" Default Value" - No
Fixed Currency problems. Back office TAX calculation on the product edit page
Fixed UPS shipping quotes are incorrect
Fixed Quote CollectTotals performance issue
Fixed PayPal Checkout Error Duplicate Order ID
- added additional exception handling which sets transaction to pending
Fixed In report Products Ordered configurable and its associated simple product appear and are counted
Fixed Multi select attributes not importing/exporting correctly
Fixed Google Bot User Agent and compare product issue
Fixed Bundle price display issue with tier pricing
Fixed No validation of Customs Value field
Fixed Form for adding new customer is shown instead customer's information page
- correct customer ID passed to URL generator
Fixed With IE9 impossible to do drag and drop actions in Admin
- added support of Range.createContextualFragment for IE9
Fixed Countries with no Zip code still have it as required field in address
Fixed Anchor category does not display products from subcategories
Fixed Place of "Options Details" is wrong in wishlist for composite products
Fixed 3D Secure + PayPal Website Payments Pro in UK prevents non-3D secure cards from working
Fixed When creating new order for customer registered on multiple websites, account/website mismatch causes issues
Fixed Shipping method is calculating based on default shipping address instead of 'Same as billing' setting in backend
Fixed Global variables in js.js
Fixed Observers from adminhtml are do not work when use Soap
Fixed Item quantity changed to 1 if added space
Fixed Row total is incorrectly calculated as negative number
Fixed HTML validation fails for pages with multiple grids
Fixed Can not log in to MCM if connect.cfg is incorrect
Fixed Incorrect use of chmod in Varien_Io_File::streamClose()
Fixed Unable to return full amount on PayPal if partial credit memo is done and customer applied Store Credit
Fixed Import Issue when attribute values not unique
Fixed Wrong customer group in order creation process in Admin panel
Fixed "Unable to save invoice" message appears when admin captures money when authorization transaction is no longer valid
Fixed Wishlist doesn't save configured composite products if MAP is enabled
Fixed Empty items grid is present, after deleting last item
Fixed Incorrect Tax Calculation when "Apply Tax On:Original price only" but custom price is not entered
Fixed Unable to place order with Authorize.net Direct Post payment method in IE 9
Fixed Ability to bypass configuration setting for the Admin area URL route
Fixed Ability to create package with decimals Qty of products, for which "Qty Uses Decimals" set to "No"
Fixed Excess semicolon in warning message, during creating Shipping Labels (in case with invalid Packaging Type)
Fixed msrp_display_actual_price_type (MAP:Display Actual Price) field is not exported
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect warning message, after Additions products with Qty that exceeds maximum available quantity
Fixed Catalog price rule doesn't work with contains condition and value which contains only cents
Fixed No store base currency beside Customs Value
Fixed Catalog Price Rule not applying to imported products
Fixed Incorrect "Shipper" and "Ship to" information in Shipping Label (in case with UPS)
Fixed Images are not imported via new Import functionality
Fixed Packages Print looks incorrectly
Fixed MAP. In the JS pop-up link "Checkout with PayPal" displayed only under FF
Fixed Extra double-quote in transactional email template app/locale/en_US/template/email/password_new.html
Fixed No ability to create Shipping Label for product with non-integer weight in Ounces (USPS - First-Class Mail International Package)
Fixed Layout issue if RSS is On
Fixed Previous customer information stays on the page header while one page checkout in process
Fixed Out of Stock Configurable product is displayed as In Stock
Fixed In the up-sell products "click to see price" link displayed, when settings "In cart", "Before Order Confirmation" is used
Fixed MAP. On the onepage, in the Wishlist block, link "Click for Price" is not active
Fixed Frontend: the products in Shopping Cart is transferred to other customer, if this customer is logged in in "My Account" page
Fixed Wrong prices are displayed for placed order with downloadable product
Fixed Shipping amount display issue when placing an order on the backend
Fixed Length, Width, Height are not passed to shipping carrier, during package creation (in case with DHL)
Fixed Disabled fields in Create Packages Pop-up with Girth field looks incorrectly
Fixed Customer address that affect tax calculation does not affect persistent customer
Fixed Ability to create more products in Shipping Labels than products in the order/shipment (in case with decimals Qty of products)
Fixed No ability to create Shipping Labels with several packages (in case with decimals Qty of products)
Fixed Formed items grid looks incorrectly, during package creation
Fixed Incorrect total weight of bundle product
Fixed Shopping Cart Rule Not Working Properly
Fixed Javascript error on "forgot your password" validation
Fixed When custom price is applied on an order in the admin, Price Incl tax on the order is the same as Excl tax
Fixed Edit cart item return unnecessary error message
Fixed Unable to save HTML code in attribute options
Fixed In the Wishlist text message appears in 2 rows, when MAP is applied for product that is in the wishlist
Fixed Unable to apply coupon code to order with zero subtotal
Fixed Nonexistent blank option in multiple select form attribute
Fixed Cannot add widget to packages or themes containing underscore in name
Fixed Product's sort order by position works incorrect with negative numbers
- allowed negative numbers
- corrected sorting by position
Fixed Incorrect Grand Total calculation when "Buy X get Y free" discount applied
Fixed Wrong product's quantity in the Wishlist after updating 'Shopping Cart'
Fixed Unneeded URL translation in admin template
Fixed Incorrect subtotal on invoice creation page (Order with Tax and Discount)
- hidden tax amount was added to collect process
Fixed When we add new address to address book during onepage checkout, not shown customer address attributes are taken from saved address attribute value
Fixed Street Address input box missing on create order form in admin
Fixed MAP enabled. In the wishlist block product price displayed when it should not
Fixed Qty field is not disabled if even check-box unselected
Fixed No ability to create Shipping Label with decimals Qty of products (in case with FedEx International)
Fixed FedEx Shipping Method unavailable (in case with Request Courier drop off type)
Fixed Unable to upgrade Magento when installed extension without max version
Fixed Wrong calculation price of Bundle product
- fixed sub item prices calculation
Fixed Incorrect products weight in Shipping Label (in case with USPS Int.,FedEx Int. and decimal Qty)
Fixed Gateway URL Absent in FedEx Shipping Module
Fixed Google checkout shipping (merchant and carrier calculated) returns only default prices
Fixed Frontend: the products in the Shopping Cart is not transferred to other customer, if this customer is logged in or register after clicks on "Checkout with Multiple Addresses", "Google Checkout" or "PayPal"
Fixed Unable to login to site after adding SID to URL
Fixed Image in description doesn't shown in compare grid
Fixed Missed validation for space charter in begin of unique fields
Fixed Impossible to sort blocks
Fixed Incorrect behavior of Offline Refunds for an Order when Adjustment fee is specified
Fixed Order saving error on backend
Fixed Customer logged out by wrong SID cached in blocks
Fixed System->Configuration->Advanced->Admin->Startup page->"Startup Page" drop-down - Optgroups are displayed after child elements
Fixed Removed unused code from Varien_File_Uploader
Fixed DHL Shipping Methods unavailable (in case with package type letter)
Fixed Error via using Global Search [Search in Admin]
Fixed Error is presented by saving address, creating order with created attributes type Image File or file(attachment)
Fixed Package contents should be specified dynamically while creating shipping labels for the USPS International shipping methods
Fixed Product option with file type input is not being transferred from wishlist to the cart
- add mergeBuyRequest method to Mage_Wishlist_Model_Item
- add checking of custom add to cart URL in Mage_Catalog_Block_Product_View
Fixed Import: Imported file is not saved to var/importexport
Fixed Reports for Sales do not work except PayPal Settlement if several order statutes were selected
Fixed No disabling of package type and dimensions fields (in case with USPS Domestic)
Fixed Wrong behavior of composite configurable product during adding to the Shopping Cart via backend
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
- added/removed several methods/packages for UPS shipping according to SRS
Fixed "Notify for Quantity Below" does not work
Fixed Frontend: Tier price not always applied to Mini Shopping Cart
Fixed Void button is present on Order page, Authorization transaction is not closed when payment action is set to "authorize and charge" - Google Checkout
Fixed MAP is applied to a Bundle product with dynamic price
Fixed No ability to create Shipping Label with package size "Oversize"
Fixed Button "Add to Cart" located in JS-popup (with Display Actual Price = On Gesture) doesn't work
Fixed Incorrect Shipping Label for USPS Library Mail Shipping Methods
Fixed Duplicating customer's addresses through placing order (backend)
Fixed Updating the qty of products from backend does not allow checkout on Frontend
- added ability to Quote and Quote items to track errors and remove them, when fixed, so whole 'error' status from Quote/Quote Item can be removed
- removed duplicating messages on Cart View page
Fixed No ability to create Shipping Label even if "Residential Delivery" set to "Yes" (in case with FedEx Home Delivery)
Fixed Button "Add new address" for customer works incorrect (backend)
Fixed It should be possible to set Minimum Qty Allowed in Shopping Cart setting via backend
Fixed Cart Subtotal is shown incorrect in sidebar shopping cart
Fixed Grid/list view settings do not save
Fixed Cannot assign custom filter to the grid column
Fixed Wishlist - product custom options are lost after customer login
Fixed Saved products will be matched each target rule
Fixed Taxes are not displayed in the catalog from frontend for Bundle products
- re-factored work with taxes for bundle product
Fixed Unable to save year less than 1970 in DOB customer attribute
- added DATETIME type to DDL
- fixed customer attributes to have same as pre-MMDB default values
Fixed "Grand Total" is not displayed for a configurable product that contains product where DAP = display before order confirmation
Fixed 'Click for price' not clickable after pressing 'Review' link in category
Fixed Bundle price display issue with tier pricing
- not considering tier price at bundle product's view page in price range
Fixed Frontend: In the block "Recently Viewed Products" the products of two customers are mixed
Fixed Error with Advanced Search (in case with Date Attribute)
Fixed Tax Rate ignores set values of Post/Zip codes Range From-To and applies it to Address with any Zip codes
Fixed Wishlist - Comment lost on config update
Fixed Import cannot handle UTF-8 characters
Fixed Welcome email template for store view scope is being ignored
Fixed Incorrect behavior of bundle product during creating Shipping Label with Customs value (in case when Price: Fixed, Ship Bundle Items" set to Separately)
Fixed Order status isn't changed when payed via PayPal if registered email differs characters cases (upper and lower)
Fixed Unwanted orders are shown in Sales->Orders list when the date filter affects to the day when DST changes apply
Fixed Payment method "Credit Card (saved)" does not display fields for fill in card information when product price is 0.00
Fixed Available to create online invoice after performing void for order
Fixed MAP configuration must contain default text for "Default Popup Text Message" and "Default "What's This" Text Message"
Fixed Backwards compatibility loss results in fatal error in Google Shopping module
- added all previous DDL constants to DDL Table, they are deprecated and being converted to new supported types
- added support for 'char' attributes
- fixed several incompatibilities in DDL Table
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Frontend: The block "Compare Products" with product is present on catalog page after adding the product to this block and clicking on "Not..?"
Fixed Fatal error when trying to open configurable product with super attribute not in the appropriate attribute set
Fixed Unable to return full amount on PayPal if partial credit memo is done and customer applied Store Credit
Fixed When creating new order for customer registered on multiple websites, account/website mismatch causes issues
Fixed Import Issue when attribute values not unique
Fixed After upgrading Magento website left in the maintenance mode
Fixed Ability to create more Shipping Labels than products in the order(shipment)
Fixed Street Address and Street Address 2 are mixed up in request to shipping carrier (in case with USPS International)
Fixed PayflowLink doesn't work (error "Payment has been declined. Please try again." is shown, Order is canceled)
Fixed Shopping cart price rule with attribute does not work when "Use Flat Catalog Product" enabled
Fixed Upgrade checking after cache flushed
Fixed Frontend: Tier price not always applied to Mini Shopping Cart
Fixed A message for the case when shipping label is created from the order should be modified
Fixed Spelling mistake in abbreviations unit of mass measurement (lbs, kgs)
Fixed FedEx Ground Shipping Method unavailable (if others FedEx Shipping Methods unavailable)
Fixed Incorrect Signature Confirmation options in the drop-down (in case with UPS)
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- add recollect total prices for quote on customer register
Fixed Fatal error when requesting non-existent file from Media directory
Fixed Button "Add to Cart" located in JS-popup (with Display Actual Price = On Gesture) doesn't work
Fixed Headers sent twice or three times when file downloading
Fixed Shipping method is calculating based on default shipping address instead of 'Same as billing' setting in backend
Fixed No ability to create more that one online Partial Invoice with Google Checkout
- parent transaction will be closed on payment model level;
- fixed exception error in Mage_Tax_Model_Resource_Calculation
Fixed Cross Sell Sorting Not Working
Fixed No ability to create Shipping Label for USPS - First-Class Mail International Package
Fixed Notification remove link in admin redirects to homepage on frontend in IE8
Fixed Incorrect behavior of image gallery
Fixed 'On Gesture' option is not applied on products' level
Fixed The message that appears instead or totals in the shopping cart and mini shopping cart should be modified
Fixed Void button present when order is fully invoiced
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed PayflowLink doesn't work (error "Payment has been declined. Please try again." is shown, Order is canceled)
Fixed Incorrect Online Refund amount in Magento, when Adjustment Fee is specified (Google Checkout)
Fixed Brazil PayPal requirements upgrade
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Issue with add to cart action, possible to add to cart a quantity of N+1 for a product
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
Fixed Wrong content in export file (all export types)
Fixed "Mysql" must be renamed to "MySQL" in installer
Fixed File overwriting during Import/Export
Fixed Reuse of adapter utilities in helper
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed When changing locale that has Unicode characters, the countries are not sorting correctly
Fixed Importing customers via CSV
Fixed Two void transactions created when using Payment Action = Order in PayPal Express
Fixed Issue with newsletter subscriptions and logged in customers
Fixed Frontend: Long-term cookie session is not over after click on "(Not..?)" link
Fixed Mismatch counts of products for different scope
Fixed Wrong config setting are implemented for MAP functionality in admin on product's level
Fixed Street Address and Street Address 2 are mixed up in request to shipping carrier (in case with USPS International)
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
- fixed MonetaryValue to be whole number
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Add verification into predispatch observers used in persistent shopping cart
Fixed Canceled orders should be excluded from Tax Reports
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Import/Export: Append Complex Data works incorrect with grouped products
- check behavior was added
Fixed Fatal error appears on get shipping rates for UPS if system base currency <> merchant country currency
Fixed Map in the frontend link has "Click to see price" name, but must be "Click for price"
Fixed Taxes are not displayed in the catalog from frontend for Bundle products
Fixed Available to delete drop down attribute which used in configurable product
Fixed MySQL error with "max_allowed_packet" during check data step for a huge .csv file
- Changed value for constant DB_MAX_PACKET_COEFFICIENT in Mage_ImportExport_Model_Resource_Helper_Mysql4
Fixed Invalid requests to USPS API
Fixed No ability to input some value in dimensions field in case for package type with non-standard dimensions
Fixed Packages Pop-up looks incorrectly
Fixed Caching config in Database results in endless recursion
Fixed No Signature Confirmation in Packages pop-up
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed "NaN" instead of two dashes in Package pop-up (in case with disabled Length, Width and Height fields)
Fixed Prefix and suffix aren't visible in Register Form
- Modified persistent customer templates
Fixed Unable to Checkout with Multiple Addresses with Registration
Fixed Not work shipping methods Fedex & DHL
- Re-factored DHL, FedEx, Ups, USPS
- Fixed minor bugs for frontend(package.phtml, view.phtml) and backend (popup.phtml, shippingmethod.phtml)
Fixed When we do reindex from console, folder var/log changes permissions from 0777 to 0775
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Orders placed through PayPal marked as "Suspected Fraud"
- Added formatting amount  into comparing
Fixed Enable Log Cleaning option is not working properly
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Value from Total Weight field is not passed to shipping carrier (in case with DHL and UPS)
Fixed After enabling dashboard chart admin user is unable to login to admin panel
Fixed Sorting on Please Select products to Add doesn't work
Fixed Catalog Price Rules - the rule is saved but not applied
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Cross Sell Sorting Not Working
Fixed Error when obtaining missed file over get.php
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Unable to save Poll for more than one Store
Fixed Mage_Directory_Helper_Data::getRegionJson doesn't translate region names
Fixed Static block in the Main Content Area overlaps border of the catalog of products
Fixed 3D secure with Saved CC works incorrectly
Fixed Unable add Gift Options for Individual Items
Fixed Customer Reports
- avoid selections group by null customer id
Fixed Mysql4 install error
Fixed "What's this?" link is absent, "Click for price" link doesn't work for shared Wishlist page
Fixed Incorrect Row Total Calculation in Refund
- changed tax counting algorithm(now it counts tax for single item)
Fixed Incorrect recipient name of Shipping Label
Fixed Missing "Street Address Line 2" in Shipping Label (in case with DHL)
Fixed After upgrading Magento website left in the maintenance mode
Fixed Frontend: JavaScript error appears if user registered on Checkout Page
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Information is not saved in DB after placing order during checkout
Fixed Reports data wrong even after refreshing lifetime statistics
Fixed Frontend can be broken by recursion
Fixed Sub items are not displayed for the order for bundles, if user use Return and Orders link
- added renderers for non-simple product types
Fixed Error message for the case when store information is incomplete should be changed
Fixed MAP behavior for RSS feed pages should be changed accordingly to SRS (only "Click for price" link should be present)
Fixed Exception after upgrade Magento via diff files
Fixed Frontend: The block "Compare Products" is empty after relogin
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- remove checking if customerGroupId exists because quote is loaded with existed customerGroupId as guest
Fixed Unable to delete product with tag in pending status
Fixed Images not imported using new Import/Export

=== Known issues ===
If you see the Service Temporarily Unavailable page after refreshing the frontend, open the Magento installation directory on the server and remove the maintenance.flag file. Then go to Magento var directory and remove the cache directory
- this issue only exists immediately after upgrading correct
Incorrect address in request to shipping carrier (DHL International) in case when address contains letter with diacritic
No ability to save created package when origin address in Germany (in case with UPS Express)
Two products are in the same row in Shipping Label (in case with FedEx International Priority)
Incorrect tracking number in the Shipping Label (in case with "Federal Express - Ground" shipping method)
No ability to save created package when origin and destination in Europe (in case with UPS Standard)



==== 1.6.x-devel-115929 ====

=== Fixes ===
Fixed Currency problems. Back office TAX calculation on the product edit page
Fixed UPS shipping quotes are incorrect
Fixed Quote CollectTotals performance issue
Fixed PayPal Checkout Error Duplicate Order ID
- added additional exception handling which sets transaction to pending
Fixed In report Products Ordered configurable and its associated simple product appear and are counted
Fixed Multi select attributes not importing/exporting correctly
Fixed Google Bot User Agent and compare product issue
Fixed Bundle price display issue with tier pricing
Fixed No validation of Customs Value field
Fixed Form for adding new customer is shown instead customer's information page
- correct customer ID passed to URL generator
Fixed With IE9 impossible to do drag and drop actions in Admin
- added support of Range.createContextualFragment for IE9
Fixed Countries with no Zip code still have it as required field in address
Fixed Anchor category does not display products from subcategories
Fixed Place of "Options Details" is wrong in wishlist for composite products
Fixed 3D Secure + PayPal Website Payments Pro in UK prevents non-3D secure cards from working
Fixed When creating new order for customer registered on multiple websites, account/website mismatch causes issues
Fixed Shipping method is calculating based on default shipping address instead of 'Same as billing' setting in backend
Fixed Global variables in js.js
Fixed Observers from adminhtml are do not work when use Soap
Fixed Item quantity changed to 1 if added space
Fixed Row total is incorrectly calculated as negative number
Fixed HTML validation fails for pages with multiple grids
Fixed Can not log in to MCM if connect.cfg is incorrect
Fixed Incorrect use of chmod in Varien_Io_File::streamClose()
Fixed Unable to return full amount on PayPal if partial credit memo is done and customer applied Store Credit
Fixed Import Issue when attribute values not unique
Fixed Wrong customer group in order creation process in Admin panel
Fixed "Unable to save invoice" message appears when admin captures money when authorization transaction is no longer valid
Fixed Whishlist doesn't save configured composite products if MAP is enabled
Fixed Empty items grid is present, after deleting last item
Fixed Incorrect Tax Calculation when "Apply Tax On:Original price only" but custom price is not entered
Fixed Unable to place order with Authorize.net Direct Post payment method in IE 9
Fixed Ability to bypass configuration setting for the Admin area URL route
Fixed Ability to create package with decimals Qty of products, for which "Qty Uses Decimals" set to "No"
Fixed Excess semicolon in warning message, during creating Shipping Labels (in case with invalid Packaging Type)
Fixed msrp_display_actual_price_type (MAP:Display Actual Price) field is not exported
Fixed Incorrect Customs Value in Create Packages in case when price value contains decimals
Fixed Incorrect warning message, after Additions products with Qty that exceeds maximum available quantity
Fixed Catalog price rule doesn't work with contains condition and value which contains only cents
Fixed No store base currency beside Customs Value
Fixed Catalog Price Rule not applying to imported products
Fixed Incorrect "Shipper" and "Ship to" information in Shipping Label (in case with UPS)
Fixed Images are not imported via new Import functionality
Fixed Packages Print looks incorrectly
Fixed MAP. In the JS pop-up link "Checkout with PayPal" displayed only under FF
Fixed Extra double-quote in transactional email template app/locale/en_US/template/email/password_new.html
Fixed No ability to create Shipping Label for product with non-integer weight in Ounces (USPS - First-Class Mail International Package)
Fixed Layout issue if RSS is On
Fixed Previous customer information stays on the page header while one page checkout in process
Fixed Out of Stock Configurable product is displayed as In Stock
Fixed In the up-sell products "click to see price" link displayed, when settings "In cart", "Before Order Confirmation" is used
Fixed MAP. On the onepage, in the Wishlist block, link "Click for Price" is not active
Fixed Frontend: the products in Shopping Cart is transferred to other customer, if this customer is logged in in "My Account" page
Fixed Wrong prices are displayed for placed order with downloadable product
Fixed Shipping amount display issue when placing an order on the backend
Fixed Length, Width, Height are not passed to shipping carrier, during package creation (in case with DHL)
Fixed Disabled fields in Create Packages Pop-up with Girth field looks incorrectly
Fixed Customer address that affect tax calculation does not affect persistent customer
Fixed Ability to create more products in Shipping Labels than products in the order/shipment (in case with decimals Qty of products)
Fixed No ability to create Shipping Labels with several packages (in case with decimals Qty of products)
Fixed Formed items grid looks incorrectly, during package creation
Fixed Incorrect total weight of bundle product
Fixed Shopping Cart Rule Not Working Properly
Fixed Javascript error on "forgot your password" validation
Fixed When custom price is applied on an order in the admin, Price Incl tax on the order is the same as Excl tax
Fixed Edit cart item return unnecessary error message
Fixed Unable to save HTML code in attribute options
Fixed In the Wishlist text message appears in 2 rows, when MAP is applied for product that is in the wishlist
Fixed Unable to apply coupon code to order with zero subtotal
Fixed Nonexistent blank option in multiple select form attribute
Fixed Cannot add widget to packages or themes containing underscore in name
Fixed Product's sort order by position works incorrect with negative numbers
- allowed negative numbers
- corrected sorting by position
Fixed Incorrect Grand Total calculation when "Buy X get Y free" discount applied
Fixed Wrong product's quantity in the Wishlist after updating 'Shopping Cart'
Fixed Unneeded URL translation in admin template
Fixed Incorrect subtotal on invoice creation page (Order with Tax and Discount)
- hidden tax amount was added to collect process
Fixed When we add new address to address book during onepage checkout, not shown customer address attributes are taken from saved address attribute value.
Fixed Street Address input box missing on create order form in admin
Fixed MAP enabled. In the wishlist block product price displayed when it should not
Fixed Qty field is not disabled if even check-box unselected
Fixed No ability to create Shipping Label with decimals Qty of products (in case with FedEx International)
Fixed FedEx Shipping Method unavailable (in case with Request Courier drop off type)
Fixed Unable to upgrade Magento when installed extension without max version
Fixed Wrong calculation price of Bundle product
- fixed sub item prices calculation
Fixed Incorrect products weight in Shipping Label (in case with USPS Int.,FedEx Int. and decimal Qty)
Fixed Gateway URL Absent in Fedex Shipping Module
Fixed Google checkout shipping (merchant and carrier calculated) returns only default prices
Fixed Frontend: the products in the Shopping Cart is not transferred to other customer, if this customer is logged in or register after clicks on "Checkout with Multiple Addresses", "Google Checkout" or "PayPal"
Fixed Unable to login to site after adding SID to URL
Fixed Image in description doesn't shown in compare grid
Fixed Missed validation for space charter in begin of unique fields
Fixed Impossible to sort blocks
Fixed Incorrect behavior of Offline Refunds for an Order when Adjustment fee is specified
Fixed Order saving error on backend
Fixed Customer logged out by wrong SID cached in blocks
Fixed System->Configuration->Advanced->Admin->Startup page->"Startup Page" drop-down - Optgroups are displayed after child elements
Fixed Removed unused code from Varien_File_Uploader
Fixed DHL Shipping Methods unavailable (in case with package type letter)
Fixed Error via using Global Search [Search in Admin]
Fixed Error is presented by saving address, creating order with created attributes type Image File or file(attachment)



==== 1.6.0.0-rc2 ====

=== Major Highlights ===
Minimum Advertised Price
Persistent Shopping Cart
Known issues: if you see the Service Temporarily Unavailable page after refreshing the frontend, open the Magento installation 
directory on the server and remove the maintenance.flag file. Then go to Magento var directory and remove the cache directory.

=== Improvements ===
XmlConnect package release v21
Order Payment Action for Express Checkout (PayPal)
- Added settings Authorization Honor Period and Order Valid Period into EC tab in the backend
- Automatically new authorize transaction created after order transaction
- Automatically cancel order after the expiration of Order Valid Period
- Automatically authorize transaction void\create after the expiration of Authorization Honor Period
Implemented Authorize.Net 'hold for review' status shows up as 'declined' in Magento.
Add Dynamic sku option for configurable products
Moneybookers Multistore System Configuration
Moneybookers OBT Defaults
PrototypeJS upgraded to 1.7

=== Changes ===
Removed deprecation.js because its not compatible with prototype 1.7
Relations between models and resource models were revised for better support of multiple databases
* Varien_Db_Adapter_Pdo_Mysql revised
* Introduced Varien_Db_Adapter_Interface,  Varien_Db_Ddl_Table
* Introduced new classes named resource helpers
* Backwards comatibility and known issues
** Flat attribute definition is not backward compatible
** Old columns names are not fully mapped to new ones
** Error appears after Customer Group saving with name length more than 32
** Caching config in Database results in endless recursion
** There's no sql upgrade for media storage tables
Deprecated GoogleBase module (http://googlemerchantblog.blogspot.com/2010/12/new-shopping-apis-and-deprecation-of.html)

=== Fixes ===
Fixed Package contents should be specified dynamically while creating shipping labels for the USPS International shipping methods
Fixed Product option with file type input is not being transferred from wishlist to the cart
- add mergeBuyRequest method to Mage_Wishlist_Model_Item
- add checking of custom add to cart url in Mage_Catalog_Block_Product_View
Fixed Import: Imported file is not saved to var/importexport
Fixed Reports for Sales do not work except Paypal Settlement if several order statutes were selected
Fixed No disabling of package type and dimensions fields (in case with USPS Domestic)
Fixed Wrong behavior of composite configurable product during adding to the Shopping Cart via backend
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
- added/removed several methods/packages for UPS shipping according to SRS
Fixed "Notify for Quantity Below" does not work
Fixed Frontend: Tier price not always applied to Mini Shopping Cart
Fixed Void button is present on Order page, Authorization transaction is not closed when payment action is set to "authorize and charge" - Google Checkout
Fixed MAP is applied to a Bundle product with dynamic price
Fixed No ability to create Shipping Label with package size "Oversize"
Fixed Button "Add to Cart" located in JS-popup (with Display Actual Price = On Gesture) doesn't work
Fixed Incorrect Shipping Label for USPS Library Mail Shipping Methods
Fixed Duplicating customer's addresses through placing order (backend)
Fixed Updating the qty of products from backend does not allow checkout on Frontend
- added ability to Quote and Quote items to track errors and remove them, when fixed, so whole 'error' status from Quote/Quote Item can be removed
- removed duplicating messages on Cart View page
Fixed No ability to create Shipping Label even if "Residential Delivery" set to "Yes" (in case with FedEx Home Delivery)
Fixed Button "Add new address" for customer works incorrect (backend)
Fixed It should be possible to set Minimum Qty Allowed in Shopping Cart setting via backend
Fixed Cart Subtotal is shown incorrect in sidebar shopping cart
Fixed Grid/list view settings do not save
Fixed Cannot assign custom filter to the grid column
Fixed Wishlist - product custom options are lost after customer login
Fixed Saved products will be matched each target rule
Fixed Taxes are not displayed in the catalog from frontend for Bundle products
- re-factored work with taxes for bundle product
Fixed Unable to save year less than 1970 in DOB customer attribute
- added DATETIME type to DDL
- fixed customer attributes to have same as pre-MMDB default values
Fixed "Grand Total" is not displayed for a configurable product that contains product where DAP = display before order confirmation
Fixed 'Click for price' not clickable after pressing 'Review' link in category
Fixed Bundle price display issue with tier pricing
- not considering tier price at bundle product's view page in price range
Fixed Frontend: In the block "Recently Viewed Products" the products of two customers are mixed
Fixed Error with Advanced Search (in case with Date Attribute)
Fixed Tax Rate ignores set values of Post/Zip codes Range From-To and applies it to Address with any Zip codes
Fixed Wishlist - Comment lost on config update
Fixed Import cannot handle UTF-8 characters
Fixed Welcome email template for store view scope is being ignored
Fixed Incorrect behavior of bundle product during creating Shipping Label with Customs value (in case when Price: Fixed, Ship Bundle Items" set to Separately)
Fixed Order status isn't changed when payed via Paypal if registered email differs characters cases (upper and lower)
Fixed Unwanted orders are shown in Sales->Orders list when the date filter affects to the day when DST changes apply
Fixed Payment method "Credit Card (saved)" does not display fields for fill in card information when product price is 0.00
Fixed Available to create online invoice after performing void for order
Fixed MAP configuration must contain default text for "Default Popup Text Message" and "Default "What's This" Text Message"
Fixed Backwards compatibility loss results in fatal error in Google Shopping module
- added all previous DDL constants to DDL Table, they are deprecated and being converted to new supported types
- added support for 'char' attributes
- fixed several incompatibilities in DDL Table
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Frontend: The block "Compare Products" with product is present on catalog page after adding the product to this block and clicking on "Not..?"
Fixed Fatal error when trying to open configurable product with super attribute not in the appropriate attribute set
Fixed Unable to return full amount on PayPal if partial credit memo is done and customer applied Store Credit
Fixed When creating new order for customer registered on multiple websites, account/website mismatch causes issues
Fixed Import Issue when attribute values not unique
Fixed After upgrading Magento website left in the maintenance mode
Fixed Ability to create more Shipping Labels than products in the order(shipment)
Fixed Street Address and Street Address 2 are mixed up in request to shipping carrier (in case with USPS International)
Fixed PayflowLink doesn't work (error "Payment has been declined. Please try again." is shown, Order is canceled)
Fixed Shopping cart price rule with attribute does not work when "Use Flat Catalog Product" enabled
Fixed Upgrade checking after cache flushed
Fixed Frontend: Tier price not always applied to Mini Shopping Cart
Fixed A message for the case when shipping label is created from the order should be modified
Fixed Spelling mistake in abbreviations unit of mass measurement (lbs, kgs)
Fixed FedEx Ground Shipping Method unavailable (if others FedEx Shipping Methods unavailable)
Fixed Incorrect Signature Confirmation options in the drop-down (in case with UPS)
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- add recollect total prices for quote on customer register
Fixed Fatal error when requesting non-existent file from Media directory
Fixed Button "Add to Cart" located in JS-popup (with Display Actual Price = On Gesture) doesn't work.
Fixed Headers sent twice or three times when file downloading
Fixed Shipping method is calculating based on default shipping address instead of 'Same as billing' setting in backend
Fixed No ability to create more that one online Partial Invoice with Google Checkout
- parent transaction will be closed on payment model level;
- fixed exception error in Mage_Tax_Model_Resource_Calculation
Fixed Cross Sell Sorting Not Working
Fixed No ability to create Shipping Label for USPS - First-Class Mail International Package
Fixed Notification remove link in admin redirects to homepage on frontend in IE8
Fixed Incorrect behavior of image gallery
Fixed 'On Gesture' option is not applied on products' level
Fixed The message that appears instead or totals in the shopping cart and mini shopping cart should be modified
Fixed Void button present when order is fully invoiced
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed PayflowLink doesn't work (error "Payment has been declined. Please try again." is shown, Order is canceled)
Fixed Incorrect Online Refund amount in Magento, when Adjustment Fee is specified (Google Checkout)
Fixed Brazil PayPal requirements upgrade
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Issue with add to cart action, possible to add to cart a quantity of N+1 for a product.
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
Fixed Wrong content in export file (all export types)
Fixed "Mysql" must be renamed to "MySQL" in installer
Fixed File overwriting during Import/Export.
Fixed Reuse of adapter utilities in helper
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed When changing locale that has Unicode characters, the countries are not sorting correctly
Fixed Importing customers via csv
Fixed Two void transactions created when using Payment Action = Order in PayPal Express
Fixed Issue with newsletter subscriptions and logged in customers
Fixed Frontend: Long-term cookie session is not over after click on "(Not..?)" link
Fixed Mismatch counts of products for different scope
Fixed Wrong config setting are implemented for MAP functionality in admin on product's level
Fixed Street Address and Street Address 2 are mixed up in request to shipping carrier (in case with USPS International)
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
- fixed MonetaryValue to be whole number
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Add verification into predispatch observers used in persistent shopping cart
Fixed Canceled orders should be excluded from Tax Reports
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Import/Export: Append Complex Data works incorrect with grouped products
- check behavior was added
Fixed Fatal error appears on get shipping rates for UPS if system base currency <> merchant country currency
Fixed Map in the frontend link has "Click to see price" name, but must be "Click for price"
Fixed Taxes are not displayed in the catalog from frontend for Bundle products
Fixed Available to delete dropdown attribute which used in configurable product
Fixed MySQL error with "max_allowed_packet" during check data step for a huge .csv file
- Changed value for constant DB_MAX_PACKET_COEFFICIENT in Mage_ImportExport_Model_Resource_Helper_Mysql4
Fixed Invalid requests to USPS API
Fixed No ability to input some value in dimensions field in case for package type with non-standard dimensions
Fixed Packages Pop-up looks incorrectly
Fixed Caching config in Database results in endless recursion
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed No Signature Confirmation in Packages pop-up
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed "NaN" instead of two dashes in Package pop-up (in case with disabled Length, Width and Height fields)
Fixed Prefix and suffix aren't visible in Register Form
- Modified persistent customer templates
Fixed Unable to Checkout with Multiple Addresses with Registration
Fixed Not work shipping methods Fedex & DHL
- Re-factored DHL, Fedex, Ups, Usps
- Fixed minor bugs for frontend(package.phtml, view.phtml) and backend(popup.phtml, shippingmethod.phtml)
Fixed When we do reindex from console, folder var/log changes permissions from 0777 to 0775
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Orders placed through PayPal marked as "Suspected Fraud"
- Added formatting amount  into comparing
Fixed Enable Log Cleaning option is not working properly
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Value from Total Weight field is not passed to shipping carrier (in case with DHL and UPS)
Fixed After enabling dashboard chart admin user is unable to login to admin panel
Fixed Sorting on Please Select products to Add doesn't work
Fixed Catalog Price Rules - the rule is saved but not applied
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Cross Sell Sorting Not Working
Fixed Error when obtaining missed file over get.php
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Unable to save Poll for more than one Store.
Fixed Mage_Directory_Helper_Data::getRegionJson doesn't translate region names
Fixed Static block in the Main Content Area overlaps border of the catalog of products
Fixed 3D secure with Saved CC works incorrectly
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed Unable add Gift Options for Individual Items
Fixed Customer Reports
- avoid selections group by null customer id.
Fixed Mysql4 install error
Fixed "What's this?" link is absent, "Click for price" link doesn't work for shared Wishlist page.
Fixed Incorrect Row Total Calculation in Refund
- changed tax counting algorithm(now it counts tax for single item)
Fixed Incorrect recipient name of Shipping Label
Fixed Missing "Street Address Line 2" in Shipping Label (in case with DHL)
Fixed After upgrading Magento website left in the maintenance mode
Fixed Frontend: JavaScript error appears if user registered on Checkout Page.
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Information is not saved in DB after placing order during checkout
Fixed Reports data wrong even after refreshing lifetime statistics
Fixed Frontend can be broken by recursion
Fixed Sub items are not displayed for the order for bundles, if user use Return and Orders link
- added renderers for non-simple product types
Fixed Error message for the case when store information is incomplete should be changed
Fixed MAP behavior for RSS feed pages should be changed accordingly to SRS (only "Click for price" link should be present)
Fixed Exception after upgrade Magento via diff files
Fixed Frontend: The block "Compare Products" is empty after relogin
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- remove checking if customerGroupId exists because quote is loaded with existed customerGroupId as guest
Fixed Unable to delete product with tag in pending status
Fixed Images not imported using new Import/Export



==== 1.6.0.0-rc1 ====

=== Major Highlights ===
Minimum Advertised Price
Persistent Shopping Cart

=== Improvements ===
XmlConnect package release v21
Order Payment Action for Express Checkout (PayPal)
- Added settings Authorization Honor Period and Order Valid Period into EC tab in the backend
- Automatically new authorize transaction created after order transaction
- Automatically cancel order after the expiration of Order Valid Period
- Automatically authorize transaction void\create after the expiration of Authorization Honor Period
Implemented Authorize.Net 'hold for review' status shows up as 'declined' in Magento.
Add Dynamic sku option for configurable products
Moneybookers Multistore System Configuration
Moneybookers OBT Defaults
PrototypeJS upgraded to 1.7

=== Changes ===
Removed deprecation.js because its not compatible with prototype 1.7
Relations between models and resource models were revised for better support of multiple databases
* Varien_Db_Adapter_Pdo_Mysql revised
* Introduced Varien_Db_Adapter_Interface,  Varien_Db_Ddl_Table
* Introduced new classes named resource helpers
* Backwards comatibility and known issues
** Flat attribute definition is not backward compatible
** Old columns names are not fully mapped to new ones
** Error appears after Customer Group saving with name length more than 32
** Caching config in Database results in endless recursion
** There's no sql upgrade for media storage tables
Deprecated GoogleBase module (http://googlemerchantblog.blogspot.com/2010/12/new-shopping-apis-and-deprecation-of.html)

=== Fixes ===
Fixed Upgrade checking after cache flushed
Fixed Frontend: Tier price not always applied to Mini Shopping Cart
Fixed A message for the case when shipping label is created from the order should be modified
Fixed Spelling mistake in abbreviations unit of mass measurement (lbs, kgs)
Fixed FedEx Ground Shipping Method unavailable (if others FedEx Shipping Methods unavailable)
Fixed Incorrect Signature Confirmation options in the drop-down (in case with UPS)
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- add recollect total prices for quote on customer register
Fixed Fatal error when requesting non-existent file from Media directory
Fixed Button "Add to Cart" located in JS-popup (with Display Actual Price = On Gesture) doesn't work.
Fixed Headers sent twice or three times when file downloading
Fixed Shipping method is calculating based on default shipping address instead of 'Same as billing' setting in backend
Fixed No ability to create more that one online Partial Invoice with Google Checkout
- parent transaction will be closed on payment model level;
- fixed exception error in Mage_Tax_Model_Resource_Calculation
Fixed Cross Sell Sorting Not Working
Fixed No ability to create Shipping Label for USPS - First-Class Mail International Package
Fixed Notification remove link in admin redirects to homepage on frontend in IE8
Fixed Incorrect behavior of image gallery
Fixed 'On Gesture' option is not applied on products' level
Fixed The message that appears instead or totals in the shopping cart and mini shopping cart should be modified
Fixed Void button present when order is fully invoiced
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed PayflowLink doesn't work (error "Payment has been declined. Please try again." is shown, Order is canceled)
Fixed Incorrect Online Refund amount in Magento, when Adjustment Fee is specified (Google Checkout)
Fixed Brazil PayPal requirements upgrade
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Issue with add to cart action, possible to add to cart a quantity of N+1 for a product.
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
Fixed Wrong content in export file (all export types)
Fixed "Mysql" must be renamed to "MySQL" in installer
Fixed File overwriting during Import/Export.
Fixed Reuse of adapter utilities in helper
Fixed MAP behavior for RSS feed pages should be changed (only "Click for price" link should be present)
Fixed When changing locale that has Unicode characters, the countries are not sorting correctly
Fixed Importing customers via csv
Fixed Two void transactions created when using Payment Action = Order in PayPal Express
Fixed Issue with newsletter subscriptions and logged in customers
Fixed Frontend: Long-term cookie session is not over after click on "(Not..?)" link
Fixed Mismatch counts of products for different scope
Fixed Wrong config setting are implemented for MAP functionality in admin on product's level
Fixed Street Address and Street Address 2 are mixed up in request to shipping carrier (in case with USPS International)
Fixed No ability to create Shipping Label if "ship to" in Canada (in case with UPS)
- fixed MonetaryValue to be whole number
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Add verification into predispatch observers used in persistent shopping cart
Fixed Canceled orders should be excluded from Tax Reports
Fixed No ability to create Shipping Label with package type "Flat-Rate Box" (in case with USPS International)
Fixed Import/Export: Append Complex Data works incorrect with grouped products
- check behavior was added
Fixed Fatal error appears on get shipping rates for UPS if system base currency <> merchant country currency
Fixed Map in the frontend link has "Click to see price" name, but must be "Click for price"
Fixed Taxes are not displayed in the catalog from frontend for Bundle products
Fixed Available to delete dropdown attribute which used in configurable product
Fixed MySQL error with "max_allowed_packet" during check data step for a huge .csv file
- Changed value for constant DB_MAX_PACKET_COEFFICIENT in Mage_ImportExport_Model_Resource_Helper_Mysql4
Fixed Invalid requests to USPS API
Fixed No ability to input some value in dimensions field in case for package type with non-standard dimensions
Fixed Packages Pop-up looks incorrectly
Fixed Caching config in Database results in endless recursion
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed No Signature Confirmation in Packages pop-up
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed "NaN" instead of two dashes in Package pop-up (in case with disabled Length, Width and Height fields)
Fixed Prefix and suffix aren't visible in Register Form
- Modified persistent customer templates
Fixed Unable to Checkout with Multiple Addresses with Registration
Fixed Not work shipping methods Fedex & DHL
- Re-factored DHL, Fedex, Ups, Usps
- Fixed minor bugs for frontend(package.phtml, view.phtml) and backend(popup.phtml, shippingmethod.phtml)
Fixed When we do reindex from console, folder var/log changes permissions from 0777 to 0775
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Orders placed through PayPal marked as "Suspected Fraud"
- Added formatting amount  into comparing
Fixed Enable Log Cleaning option is not working properly
Fixed Impossible to do online refund for "CyberSource" payment method
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Value from Total Weight field is not passed to shipping carrier (in case with DHL and UPS)
Fixed After enabling dashboard chart admin user is unable to login to admin panel
Fixed Sorting on Please Select products to Add doesn't work
Fixed Catalog Price Rules - the rule is saved but not applied
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Cross Sell Sorting Not Working
Fixed Error when obtaining missed file over get.php
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Unable to save Poll for more than one Store.
Fixed Mage_Directory_Helper_Data::getRegionJson doesn't translate region names
Fixed Static block in the Main Content Area overlaps border of the catalog of products
Fixed 3D secure with Saved CC works incorrectly
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed Unable add Gift Options for Individual Items
Fixed Customer Reports
- avoid selections group by null customer id.
Fixed Mysql4 install error
Fixed "What's this?" link is absent, "Click for price" link doesn't work for shared Wishlist page.
Fixed Incorrect Row Total Calculation in Refund
- changed tax counting algorithm(now it counts tax for single item)
Fixed Incorrect recipient name of Shipping Label
Fixed Missing "Street Address Line 2" in Shipping Label (in case with DHL)
Fixed After upgrading Magento website left in the maintenance mode
Fixed Frontend: JavaScript error appears if user registered on Checkout Page.
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Information is not saved in DB after placing order during checkout
Fixed Reports data wrong even after refreshing lifetime statistics
Fixed Frontend can be broken by recursion
Fixed Sub items are not displayed for the order for bundles, if user use Return and Orders link
- added renderers for non-simple product types
Fixed Error message for the case when store information is incomplete should be changed
Fixed MAP behavior for RSS feed pages should be changed accordingly to SRS (only "Click for price" link should be present)
Fixed Exception after upgrade Magento via diff files
Fixed Frontend: The block "Compare Products" is empty after relogin
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- remove checking if customerGroupId exists because quote is loaded with existed customerGroupId as guest
Fixed Unable to delete product with tag in pending status
Fixed Images not imported using new Import/Export



==== 1.6.x-devel-112177 ====

=== Improvements ===
XmlConnect package release v21

=== Changes ===
Removed deprecation.js because its not compatible with prototype 1.7

=== Fixes ===
Fixed MySQL error with "max_allowed_packet" during check data step for a huge .csv file
- Changed value for constant DB_MAX_PACKET_COEFFICIENT in Mage_ImportExport_Model_Resource_Helper_Mysql4
Fixed Invalid requests to USPS API
Fixed No ability to input some value in dimensions field in case for package type with non-standard dimensions
Fixed Packages Pop-up looks incorrectly
Fixed Caching config in Database results in endless recursion
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed No Signature Confirmation in Packages pop-up
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed "NaN" instead of two dashes in Package pop-up (in case with disabled Length, Width and Height fields)
Fixed Prefix and suffix aren't visible in Register Form
- Modified persistent customer templates
Fixed Unable to Checkout with Multiple Addresses with Registration
Fixed Not work shipping methods Fedex & DHL
- Re-factored DHL, Fedex, Ups, Usps
- Fixed minor bugs for frontend(package.phtml, view.phtml) and backend(popup.phtml, shippingmethod.phtml)
Fixed When we do reindex from console, folder var/log changes permissions from 0777 to 0775
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Orders placed through PayPal marked as "Suspected Fraud"
- Added formatting amount  into comparing
Fixed Enable Log Cleaning option is not working properly
Fixed Impossible to do online refund for "CyberSource" payment method
Fixed Incorrect transparency of PNG image in indexed non-alpha mode
Fixed Value from Total Weight field is not passed to shipping carrier (in case with DHL and UPS)
Fixed After enabling dashboard chart admin user is unable to login to admin panel
Fixed Sorting on Please Select products to Add doesn't work
Fixed Catalog Price Rules - the rule is saved but not applied
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Cross Sell Sorting Not Working
Fixed Error when obtaining missed file over get.php
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Unable to save Poll for more than one Store.
Fixed Mage_Directory_Helper_Data::getRegionJson doesn't translate region names
Fixed Static block in the Main Content Area overlaps border of the catalog of products
Fixed 3D secure with Saved CC works incorrectly
Fixed Shipping origin address used instead of the one specified in the RMA setting for Use Store Address = No
Fixed Unable add Gift Options for Individual Items
Fixed Customer Reports
- avoid selections group by null customer id.
Fixed Mysql4 install error
Fixed "What's this?" link is absent, "Click for price" link doesn't work for shared Wishlist page.
Fixed Incorrect Row Total Calculation in Refund
- changed tax counting algorithm(now it counts tax for single item)
Fixed Incorrect recipient name of Shipping Label
Fixed Missing "Street Address Line 2" in Shipping Label (in case with DHL)
Fixed After upgrading Magento website left in the maintenance mode
Fixed Frontend: JavaScript error appears if user registered on Checkout Page.
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Information is not saved in DB after placing order during checkout
Fixed Reports data wrong even after refreshing lifetime statistics
Fixed Frontend can be broken by recursion
Fixed Sub items are not displayed for the order for bundles, if user use Return and Orders link
- added renderers for non-simple product types
Fixed Error message for the case when store information is incomplete should be changed
Fixed MAP behavior for RSS feed pages should be changed accordingly to SRS (only "Click for price" link should be present)
Fixed Exception after upgrade Magento via diff files
Fixed Frontend: The block "Compare Products" is empty after relogin
Fixed Frontend: Catalog Price Rule does not apply to Mini Shopping Cart after login current customer
- remove checking if customerGroupId exists because quote is loaded with existed customerGroupId as guest
Fixed Unable to delete product with tag in pending status
Fixed Images not imported using new Import/Export



==== 1.6.0.0-beta1 ====

=== Major Highlights ===
Minimum Advertised Price
Persistent Shopping Cart

=== Improvements ===
Order Payment Action for Express Checkout (PayPal)
- Added settings Authorization Honor Period and Order Valid Period into EC tab in the backend
- Automatically new authorize transaction created after order transaction
- Automatically cancel order after the expiration of Order Valid Period
- Automatically authorize transaction void\create after the expiration of Authorization Honor Period
Implemented Authorize.Net 'hold for review' status shows up as 'declined' in Magento.

=== Fixes ===
Fixed Reindex Data works with errors
Fixed Group product is exported incorrectly : associated product values are not included
- reorganized counting of an array elements. Passing array items by link, broke scripts logic below.
Fixed Sql install and upgrade issues
- updated customer address attributes
Fixed Apply dashboard reports fix
Fixed The Find Feed is not reporting the correct values
Fixed show free payment method is enabled
Fixed Tax is not applied for products that are currently in the Wishlist
Fixed Unable to import products
- an collection was replaced with method which use less memory
Fixed It is impossible apply for product any tax class for 'Storeview' scope
- Added field is_global into the setup field map
Fixed Increased import data field size for huge imports.
Fixed Store view value for attribute fixed not to override global scope
Fixed Sort-titles Visibility and Status in admin redirects to Dashboard on frontend and create exception.
Fixed Configurable product uses setting from associated products
Fixed Simple Product does not have a "PayPal Checkout" button when a Product is an item of Grouped Product
Fixed Unable to import large Qty (several hundreds and more) of products using new import (tested with over 10,000 SKUs)
Fixed Apply dashboard reports fix
- fixed Reports-Sales-Orders revenue formula
Fixed authorization number detection and order transaction voiding
Fixed Session Lifetime (seconds) with value 9999999999999999 brakes all backend with warning
Fixed Images not imported
- added import/export for product media gallery
Fixed Provide backwards compatibility for setting Foreign Keys on changed core columns
- implemented auto-modifying foreign keys for column definitions
Fixed "Number of Child Authorizations" does not working
Fixed Database session storage doesn't work
- receive session_data instead of session_id
Fixed No ability to create Shipping Label after unsuccessful attempt (in a create shipment page)
Fixed USPSs Domestic Shipping Methods unavailable
Fixed Order Row Subtotal is incorrect (Order with Tax and Discount)
- fixed row subtotal tax counting.
Fixed Unable to use capture online/offline when creating invoice of edited/reordered Authorize.net orders
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Table Rate Shipping Method value column needs to be sorted in ascending order
Fixed Incorrect titles in "Product Tax Classes" tab.
Fixed Sending invoice email don`t change the status.
Fixed Admin should be able to perform online invoice after void transaction
- Added possibility to reauthorize orders with "order" payment action after void
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed Wrong customer group in order creation process in Admin panel
- Set new customer group to all his quotes for all stores on customer save
Fixed dot and tilde in base url during installation.
Fixed: Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- on prepare for render js categories tree using extjs library, collecting allowed categories for product, if product selected and product id present at request params. Then disabling all categories that can't be selected.
Fixed Incorrect dependencies between modules and code usage.
Fixed Admin doesn't sees bundle products that was added to Wishlist in backend.
Fixed Admin user interface: mistake in the label name, Id instead ID.
Fixed Warning message in backend when trying to set condition for new Shopping cart price rule
Fixed Wrong customer group in order creation process in Admin panel
- Set new customer group to all his quotes for all stores on customer save
Fixed dot and tilde in base url during installation.
Implemented Order Payment Action for Express Checkout (PayPal) Upgrade
- Added system menu changes
Fixed Incorrect dependencies between modules and code usage.
Fixed Flat attribute definition is not backward compatible
- partly reverted previous changes;
- added compatible mode for Db adapters;
- small code style fixes
Fixed Table Rate Shipping Method value column needs to be sorted in ascending order
Fixed Column "Sales Total Amount" of Coupons Sales Reports calculates in wrong way
- Changed the mathematical formula of counting Sales Total Amount
- Changed the lines, that contains more than 120 characters
Fixed Admin doesn't sees bundle products that was added to Wishlist in backend.
Fixed Admin user interface: mistake in the label name, Id instead ID.
Fixed Sending invoice email don`t change the status.
Fixed Possibility of online invoice still exist when Order Valid Period = 0
- Fixed store detection on capture
Fixed Admin should be able to perform online invoice after void transaction
- Added possibility to reauthorize orders with "order" payment action after void
Fixed Grouped product imported without associated products
- added $linksRows definition
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Incorrect titles in "Product Tax Classes" tab.
Fixed Categories moving provides Fatal error
Fixed System - > Configuration - > inventory tab disappears when switching to Website/Store view scope
Fixed Default store group with empty default store view causes fatal error on System>Configuration>Catalog>Catalog
Fixed Limit of collection for Random Product Block
Fixed Notification remove link in admin redirects to homepage on frontend in IE8
Fixed translate function fixed to use translator (for editor labels and buttons)
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed There are no server-side validation for required options (attributes) of Configurable product.
Fixed Full checkout "blocking" when delete product that was already added to the shopping cart.
Fixed No ability to submit order in back-end(in case with selected "Same As Billing Address" check box).
Fixed On the product view page action panel disappears after user manipulation on IE7/8.
Fixed Product Flat Data is not reindexed in Mysql
- default value must be unset for new column format
Fixed Varien Image crop implementation fixed
Fixed translation of quoted strings, added ability to move parameters on next line
Fixed comment node in system.xml to be translated
Fixed Default email "emaildomain.com" is a real domain.
Fixed Non-active button "continue to review your order" in multiple address checkout.
Fixed Ability to view another customer's Wishlist contents via RSS URL.
Fixed Incorrect design of the Payment Method sub-menu with billing agreement information in default CE theme
Fixed 'Term and Conditions' are not visible with PayPal Express Checkout in 'Review Order' page.
Fixed Reports->Products does not work
- Removed "order by" from count
Fixed Fatal error during filtering products on frontend by Price (decimal) type attribute
Fixed Tax rounding and calculation
- $address->_store replaced with $address->getQuote()->getStore()
Fixed Old column names are not fully mapped to new ones
- Fixed wrong data, returned by helpers to init old fields map
- Fixed @return phpDoc comments
- Used array_merge() instead of "+" - for better readability
Fixed Magento is not able to install on several versions of MySQL (5.041, Windows)
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Export: Error during export products
- added checks for an empty array of $productIds
Fixed Invalid language on import error
Fixed No ability to print Shipping Label
Fixed Enabled "Custom Admin URL" makes impossible access to backend
Fixed Backordered Item Status on Orders
- fixed problem when same product is an option of different composite (bundle, etc.) products
Fixed Scheduled newsletter queues should be sent
Fixed Export doesn't work when we have a lot of products in
Fixed 'Term and Conditions' are not visible with PayPal Express Checkout in 'Review Order' page
- Added block checkout/agreements into PayPal EC UK checkout order review page
Fixed Wrong price calculation for bundle products during Customer's shopping cart managing (Just for new prototype version)
- addProductAdvanced was replaced by addProduct
Fixed Order Row Subtotal is incorrect (Order with Tax and Discount)
- Product qty was not included during counting Subtotal amount.
Fixed Enabled "Custom Admin URL" makes impossible access to backend
- labels in System Configuration were changed
Fixed Backordered Item Status on Orders
- fixed problem when same product is an option of different composite (bundle, etc.) products
Fixed Export doesn't work when we have a lot of products in
Fixed 'Term and Conditions' are not visible with PayPal Express Checkout in 'Review Order' page
- Added block checkout/agreements into PayPal EC UK checkout order review page
Fixed Wrong price calculation for bundle products during Customer's shopping cart managing (Just for new prototype version)
- addProductAdvanced was replaced by addProduct
Fixed Order Row Subtotal is incorrect (Order with Tax and Discount)
- Product qty was not included during counting Subtotal amount.
Fixed WYSIWYG Editor - Unable to Create a Folder when Inserting a File.
Fixed Mage_Adminhtml_Block_Widget_Grid_Container to translate default label strings
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Flat attribute definition is not backward compatible
- removed ability to setup compatibility mode in admin, because it is not supported in module init
Fixed Flat attribute definition is not backward compatible
Fixed Incorrect path format when Media Storage is set to Database, unable to upload file for import
Fixed Unneeded popup window is opened through adding new product
Fixed Sorting on Please Select products to Add does not work
Added Admin can view and change products price with No Read Permission
- Added dispatching event catalog_product_attribute_update_before
- Added deleting attribute data in attribute updating model if the admin has not permissions
- Added disabling attribute fields in the block if the admin has not permissions
Fixed Package Types that not available for current Shipping Method displayed in Create Packages pop-up
Fixed Sorting on Please Select products to Add does not work
Fixed There's no sql upgrade for media storage tables
- also fixed issue with creating media storage tables on mysql 4.1.x
Fixed Admin can change status of products with No Read Permission
- Added massaction item deleting in massaction block combobox if the admin has not permissions
Fixed Unable to place order with Authorize.net Direct Post payment method in IE 9
Fixed No ability to create Shipping Label(in case with UPS International)
- fixed Delivery confirmation for UPS using its API documentation
Fixed No ability to create Shipping Label if pop-up contain Girth field (in case with USPS Domestic)
- Fixed using girth field according to USPS API documentation
Fixed Requested Qty, Authorized Qty, Returned Qty and Approved Qty must validate data to allow only digits
Fixed Apply dashboard reports fix
Fixed Email notifications do no show items with other than Authorize/Pending status
- Fix itself plus some refactoring
Fixed Special price is not displayed on the category page if "Special Price From Date" & "Special Price To Date" fields are filled.
Fixed "Localhost" isn't a valid domain name for installation
Fixed No ability to cancel Partial Authorization checkout with Authorize.net on frontend
Fixed Persistent Shopping Cart should be disabled by default
Fixed Lightbox 2.5 with IE7 returns JS error on the page
Fixed Fatal error during filtering products on frontend by Price (decimal) type attribute
- There was a problem with catalog_product_index_eav_decimal(_tmp) tables, a field 'value' should not be present in PRIMARY_KEY constraints
Fixed Fatal error during filtering products on frontend by Price (decimal) type attribute
- Update was fixed.
Fixed Missing Capture transaction in backend when capture money from PayPal (PayPal UK Express)
Fixed PayPal Website Payments Pro Payflow Edition Direct Payment does not work
- Fixed COUNTRYCODE back to COUNTRY in outgoing request to PayPal Website Payments Pro Payflow
Edition Direct Payment, but preserved COUNTRYCODE in parsing incoming request.*
Fixed "NaN" instead of two dashes in Package pop-up (in case with disabled Length, Width and Height fields)
Fixed Reports: Products Ordered report does not work
- added function _construct for setting property useAnalyticFunction = true
Fixed During creating order no warning message appears for non-configured Composite product and
Authorize.net Direct Post payment method
- The redirect patch for processing exception is changed from */*/ to */sales_order_create/
Fixed Broken backwards compatibility in adapters addIndex/dropIndex, addKey/dropKey methods
- fixed returned values to be backwards compatible
Fixed Ability to input some value in dimensions field in case for package type with standard dimensions
Fixed USPS is available Shipping Method from EU to EU
Fixed Interface is blocked after user manipulation with Details link and Other reason link
Fixed Reorder and "Create Order" in admin without Read, Edit permissions does not work and create exception.
- Added a checking. removeColumn method will be called if a block is a grid only.
Fixed In case Allow Reorder=No, Reorder still available
- store dependency was added(patch was applied)
Fixed No ability to login or register new customer in frontend (IE8)
Fixed Enabled "Custom Admin URL" makes impossible access to backend
- fixed config cache issue


==== 1.6.x-devel-109807 ====

=== Major Highlights ===
Minimum Advertised Price
Persistent Shopping Cart

=== Improvements ===
Order Payment Action for Express Checkout (PayPal)
- Added settings Authorization Honor Period and Order Valid Period into EC tab in the backend
- Automatically new authorize transaction created after order transaction
- Automatically order cancel after the expiration of Order Valid Period
- Automatically authorize transaction void\creat after the expiration of Authorization Honor Period
Implemented Authorize.Net 'hold for review' status shows up as 'declined' in Magento.

=== Fixes ===
Fixed Reindex Data works with errors
Fixed Group product is exported incorrectly : associated product values are not included
- reorganized counting of an array elements. Passing array items by link, broke scripts logic below.
Fixed Sql install and upgrade issues
- updated customer address attributes
Fixed Apply dashboard reports fix
Fixed The Find Feed is not reporting the correct values
Fixed Fixed show free payment method is enabled
Fixed Tax is not applied for products that are currently in the Wishlist
Fixed Unable to import products
- an collection was replaced with method which use less memory
Fixed It is impossible apply for product any tax class for 'Storeview' scope
- Added field is_global into the setup field map
Fixed Increased import data field size for huge imports.
Fixed Store view value for attribute fixed not to override global scope
Fixed Sort-titles Visibility and Status in admin redirects to Dashboard on frontend and create exception.
Fixed Configurable product uses setting from associated products
Fixed Simple Product does not have a "PayPal Checkout" button when a Product is an item of Grouped Product
Fixed Unable to import large Qty (several hundreds and more) of products using new import
Fixed Apply dashboard reports fix
- fixed Reports-Sales-Orders revenue formula
Fixed Fixed authorization number detection and order transaction voiding
Fixed Session Lifetime (seconds) with value 9999999999999999 brakes all backend with warning
Fixed Images not imported
- added import/export for product media gallery
Fixed Provide backwards compatibility for setting Foreign Keys on changed core columns
- implemented auto-modifying foreign keys for column definitions
Fixed "Number of Child Authorizations" does not working
Fixed Database session storage doesn't work
- receive session_data instead of session_id
Fixed No ability to create Shipping Label after unsuccessful attempt (in a create shipment page)
Fixed USPSs Domestic Shipping Methods unavailable
Fixed Order Row Subtotal is incorrect (Order with Tax and Discount)
- fixed row subtotal tax counting.
Fixed Unable to use capture online/offline when creating invoice of edited/reordered Authorize.net orders



==== 1.6.x-devel-109807 ====

=== Fixes ===
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Table Rate Shipping Method value column needs to be sorted in ascending order
Fixed Incorrect titles in "Product Tax Classes" tab.
Fixed Sending invoice email don`t change the status.
Fixed Admin should be able to perform online invoice after void transaction
- Added possibility to reauthorize orders with "order" payment action after void
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed Wrong customer group in order creation process in Admin panel
- Set new customer group to all his quotes for all stores on customer save
Fixed Fixed dot and tilde in base url during installation.
Fixed: Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- on prepare for render js categories tree using extjs library, collecting allowed categories for product, if product selected and product id present at request params. Then disabling all categories that can't be selected.
Fixed Incorrect dependencies between modules and code usage.
Fixed Admin doesn't sees bundle products that was added to Wishlist in backend.
Fixed Admin user interface: mistake in the label name, Id instead ID.
Fixed Warning message in backend when trying to set condition for new Shopping cart price rule
Fixed Wrong customer group in order creation process in Admin panel
- Set new customer group to all his quotes for all stores on customer save
Fixed Fixed dot and tilde in base url during installation.
Implemented Order Payment Action for Express Checkout (PayPal) Upgrade
- Added system menu changes
Fixed Incorrect dependencies between modules and code usage.
Fixed Flat attribute definition is not backward compatible
- partly reverted previous changes;
- added compatible mode for Db adapters;
- small code style fixes
Fixed Table Rate Shipping Method value column needs to be sorted in ascending order
Fixed Column "Sales Total Amount" of Coupons Sales Reports calculates in wrong way
- Changed the mathematical formula of counting Sales Total Amount
- Changed the lines, that contains more then 120 characters
Fixed Admin doesn't sees bundle products that was added to Wishlist in backend.
Fixed Admin user interface: mistake in the label name, Id instead ID.
Fixed Sending invoice email don`t change the status.
Fixed Possibility of online invoice still exist when Order Valid Period = 0
- Fixed store detection on capture
Fixed Admin should be able to perform online invoice after void transaction
- Added possibility to reauthorize orders with "order" payment action after void
Fixed Grouped product imported without associated products
- added $linksRows definition
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Incorrect titles in "Product Tax Classes" tab.
Fixed Categories moving provides Fatal error
Fixed System - > Configuration - > inventory tab disappears when switching to Website/Store view scope
Fixed Default store group with empty default store view causes fatal error on System>Configuration>Catalog>Catalog
Fixed Limit of collection for Random Product Block
Fixed Notification remove link in admin redirects to homepage on frontend in IE8
Fixed translate function fixed to use translator (for editor labels and buttons)
Fixed Admin should be able to perform online invoice after void transaction
- Don't call for authorization if previous is alive
Fixed There are no server-side validation for required options (attributes) of Configurable product.
Fixed Full checkout "blocking" when delete product that was already added to the shopping cart.
Fixed No ability to submit order in back-end(in case with selected "Same As Billing Address" check box).
Fixed On the product view page action panel disappears after user manipulation on IE7/8.
Fixed Product Flat Data is not reindexed in Mysql
- default value must be unset for new column format
Fixed Varien Image crop implementation fixed
Fixed Fixed translation of quoted strings, added ability to move parameters on next line
Fixed Fixed comment node in system.xml to be translated
Fixed Default email "emaildomain.com" is a real domain.
Fixed Non-active button "continue to review your order" in multiple address checkout.
Fixed Ability to view another customer's Wishlist contents via RSS URL.
Fixed Incorrect design of the Payment Method sub-menu with billing agreement information in default CE theme
Fixed 'Term and Conditions' are not visible with PayPal Express Checkout in 'Review Order' page.
Fixed Reports->Products does not work
- Removed "order by" from count
Fixed Fatal error during filtering products on frontend by Price (decimal) type attribute
Fixed Tax rounding and calculation
- $address->_store replaced with $address->getQuote()->getStore()
Fixed Old column names are not fully mapped to new ones
- Fixed wrong data, returned by helpers to init old fields map
- Fixed @return phpDoc comments
- Used array_merge() instead of "+" - for better readability
Fixed Magento is not able to install on several versions of MySQL (5.041, Windows)
Fixed There are no special titles for 'Site Map', 'Search Terms', 'Contact Us', 'Forgot Your Password' pages.
Fixed Export: Error during export products
- added checks for an empty array of $productIds
Fixed Invalid language on import error



==== 1.6.0.0-alpha1 ====

=== Improvements ===
Add Dynamic sku option for configurable products
Moneybookers Multistore System Configuration
Moneybookers OBT Defaults
PrototypeJS upgraded to 1.7

=== Changes ===
Relations between models and resource models were revised for better support of multiple databases
* Varien_Db_Adapter_Pdo_Mysql revised
* Introduced Varien_Db_Adapter_Interface,  Varien_Db_Ddl_Table
* Introduced new classes named resource helpers
* Backwards comatibility and known issues
** Flat attribute definition is not backward compatible
** Old columns names are not fully mapped to new ones
** Error appears after Customer Group saving with name length more than 32
** Caching config in Database results in endless recursion
** There's no sql upgrade for media storage tables
Deprecated GoogleBase module (http://googlemerchantblog.blogspot.com/2010/12/new-shopping-apis-and-deprecation-of.html)

=== Fixes ===
Fixed Unable to change customer password when email confirmation is enabled
Fixed Can't choose Group at the creation new Order by admin
Fixed Subtotal for Bundle product with quantity 2 calculates as for one
Fixed Breadcrumbs and the ?Use categories path for product URLs setting
Fixed RSS feed redirected to 404 error page (from admin panel)
Fixed Cache Management incorrect ACL check
Fixed Media Sub-Folder Creation and View in Admin
Fixed Quantity of bundle item is not stored correctly, in case when it is decimal
Fixed Shipping creation for bundle product shows wrong q-ty
Fixed Issue creating content staging site
Fixed Unable to create attribute with numbers
Fixed Moving Grouped product from Order and Shopping cart to the Wishlist does not work
Fixed Product Attribute can't be saved if Attribute Code contain numbers
Fixed Incorrect titles in "Sales Emails" tab
Fixed Any backend user can access the MCM (Downloader)
Fixed Saving attribute value in store view scope only causes data loss
Fixed Resources names are not translated on Role Resources page at backend
Fixed Quote Lifetime don't work
Fixed WYSIWYG Editor - Unable to Create a Folder when Inserting a File
Fixed Out of stock products getting "This product has not been configured." error msg
Fixed Impossible save empty values for store view scope
Fixed Include in Navigation Menu
Fixed Date Field error in product
Fixed product.js not working well images that are taller than wider.
Fixed Modern theme search results page bug
Fixed Bundled product special pricing does not reflect in cart
Fixed In Configurable Products only Admin attribute label is retrieved
Fixed Anchored categories w/ subcategories and products in both
Fixed Minimum quantity in Grouped product
Fixed Minimum Quantities Warning not working properly
Fixed Unable to change configurable product name for store view
Fixed Dropdown attributes with no value should be hidden
Fixed CLONE -"Compare Products" block does not appear on the category page and product page
Fixed Category and product design settings inheritance
Fixed Not shown button for browsing file in "downloadable product" tab "Downloadable Information"(Just for new prototype version).
Fixed Some small and thumbnail images are corrupted for products
Fixed Zooming doesn't work for an image larger or taller than the container
Fixed Frontend->Necessary to add pagination to the bottom of category
Fixed Category Tree -> Changing category color
Fixed Changing Attribute Scopes
Fixed Typo: wrong helper used in ProductController to call initProductLayout()
Fixed Unable to continue checkout when "Street Address" use non English characters
Fixed Time payment processing extremely long
Fixed Cannot create or save after editing customer's Address, "Please enter the street" error appears on frontend
Fixed product not salable marking/language issue
Fixed Free shipping doesn't work in table rates shipping method
Fixed Wrong order status after "Credit Memo" for product's with FPT
Fixed Missing Capture transaction in backend when capture money from PayPal (PayPal UK Express)
Fixed Unable to made online refund from Magento using PayPal UK Express checkout
Fixed It's possible to click twice on order place button and receive "Cart is empty" page
Fixed Unable to place order for customer with Cyrillic street name.
Fixed Backend - Add new customer - ALL TRANSLATIONS MISSING
Fixed Customer Segment "Up to Date" Condition Logical Inversion
Fixed Errorhandling in saveAction / editAction broken
Fixed Reward points expiration date is shown incorrect
Fixed Incorrect "Date of Birth" validation
Fixed Error when searching Customer Wishlist by Qty at admin backend
Fixed Default values for customer attributes settings are not used in some cases
Fixed Category Treeview Broken (Manage Products/Manage Categories)
Fixed Categories' does not show full categories tree (Just for new prototype version).
Fixed It should be possible to create Simple associated product during Configurable product creation process (Just for new prototype version)
Fixed It should be possible to delete row with Samples for Downloadable product during creation (Just for new prototype version)
Fixed No display of Remaining Balance, if only one credit card used with Authorize.net Payment Method
Fixed Partial Authorization is not working at all, when Authorize and Capture setting is enabled for Authorize.net
Fixed Subtotal displays incorrect subtotal if gift wrapping was applied
Fixed Orders with not supported statuses moved to orders archive.
Fixed No compiled CSS and JavaScripts are present in native database
Fixed View Details" link is not present for simple product with custom options or Gift Cards added to the Wishlist
Fixed Full Page Cache and design themes exceptions
Fixed Setting "Backorders" > "No Backorders" do not apply in backend and order creation.
Fixed Not received the warning message "This product is available for purchase in increments of 2 only." in backend order creation.
Fixed Order is in google sandbox doesn't contain gift card
Fixed Broken JS validation on "Configuration" step
Fixed Broken mysql4-data-upgrade-1.4.0.0.13-1.4.0.0.14.php file
Fixed "Turkish Lira" missing on the "Localization" step during installation
Fixed Magento Connect -> MCM -> "Log in" page - Message or some information about required fields doesn't appeared
Fixed Magento Connect -> MCM -> "Settings" tab -> Changes don't saved
Fixed Magento Connect -> MCM -> "Settings" tab -> data doesn't saved
Fixed Magento Connect -> MCM -> If extension packages contains files with the same names, it installation shoul be conflicted.
Fixed Payment Applicable From = "Specific Countries" option does not work for Express Checkout (Payflow Edition)
Fixed Credit Card information is required for $0.00 total.
Fixed Image-Upload does not work in Safari 5
Fixed Paypal Direct send wrong billing address to API
Fixed Incorrect billing/shipping address transfer from Magento to PayPal ( WPP Payflow Edition, WPP Payflow Edition EC )
Fixed Gateway error: A valid amount is required' appears during create Credit Memo for order, which uses Authorize.net
Fixed Magento creates order even if response from PaypalUk is empty
Fixed Enabled payment actions are available for order with "Zero subtotal"
Fixed Incorrect format of the transferring shipping/billing addresses from Magento to PayPal (WPP EC, WPS, WPP )
Fixed When in backend ?new order? and using a custom price the subtotal is wrong
Fixed Buy One Get One Free not working
Fixed Table Rates & Free Shipping Cart Rules not working together
Fixed Catalog Prices include tax is not working.
Fixed buy 1 get 1 free doesn't work
Fixed Bundle Product using Fixed Price does not Display Tier Pricing Correctly
Fixed Cart Price Rule not working with Product Attributes
Fixed Tax from orders in status pending presents in Tax Report
Fixed Coupons Report Math Bug
Fixed Credit Memo refunding not working due to four decimal places for Shipping costs
Fixed Can not ad Product to order if it has custom options
Fixed Tier price does not applies correctly on the back-end if customer group is changed on the backoffice order
Fixed Wrong product with custom options price is displayed in the wishlist sidebar during order creation via back-end
Fixed Missing isset() in Mage_Sales_Model_Recurring_Profile::createOrder()
Fixed Shipping address is not saving during process order in backend with 'Save in Address book' option for existing customer.
Fixed Advanced search on boolean type attributes
Fixed UPS (UPSS,DHL,FedEx) options "Maximum Package Weight " works not correct.
Fixed Shipping method UPS_XML missing titles
Fixed Table rate shipping is not recalculate after applying a discount
Fixed PDF subtotal including tax is zero
Fixed Tax/VAT number not displayed
Fixed HTML typo in Transactional mail "account_new_confirmation.html"
Fixed Varien_Db_Adapter_Mysqli::raw_query() should throw an Exception after 10 tries

==== 1.5.1.0 ====                                                                     
                                             
=== Improvements ===
Alternative image storage feature enabled with fixed get.php file.
Magento Mobile updated to release v20
Implemented SOAP Faults for GiftMessage API
- added faults in functions
- added description in api.xml
Implemented The names of WPPHS depend on a merchant`s country in the backend. Create a functionality for dynamic changing.
- Added functionality for dynamic changing the names of WPPHS
- Added backend config into system.xml
Implemented WS-I for API
- added wsi.xml for all WebAPI modules
- added new wsi-soap handler
- added new wsi-soap adapter
- changed admin configuration, added parameter into "Magento Core API"->WSI Compliance
- changed api.xml
Implemented GiftMessage for Cart

=== Changes ===
Replaced usage of Varien_File_Uploader with Mage_Core_Model_File_Uploader

=== Fixes ===
Fixed PayPal Standard: order has two invoice and two refund
Fixed Adjustment Fee, Adjustment Refund and Refund Shipping fields must be disabled on credit memo for Payflow Pro and PayFlowLink payment methods
- Actualized API params mapping 
- Added parameter Amount into refund request
Fixed Broken mysql4-data-upgrade-1.4.0.0.13-1.4.0.0.14.php file
Fixed XMLConnect - edited parameter cannot be saved
Fixed Media storage - problem with image in the CMS pages
- Added functional to get files with disabled db media storage feature through the get.php script
Fixed Unable to place order using PayPal Billing agreement through Checkout with multiple addresses
- Added additional multi shipping checkout exceptions logging.
Fixed No AmericanExpress support in Website Payments Pro Payflow Edition
- Added to Direct payment 
Fixed Incorrect Subtotal(Incl. Tax) in Shopping Cart, when catalog prices entered by admin include tax
Fixed Function "Apply Tax On - Original price only" does not correct calculate product tax
Fixed No ability to save Product Attribute with type Media Image
Fixed Mage_CatalogSearch_Model_Query::getMaxQueryLenght() is not properly deprecated.
Fixed Two links in forgotpassword.phtml template lead to not existent files
Fixed Added compiled js and css to whitelist. Added removing of relative URL parts to get.php.
Fixed several probable vulnerabilities on front and backend
Fixed Incorrect error message when extension state is lower than preferred state
Fixed No rule applied when coupon code is no longer valid
- verify if rule uses coupon at all before coupon check
Fixed Argument passed to Mage_Catalog_Helper_Image::init() must be an instance of Mage_Catalog_Model_Product, instance of Mage_Wishlist_Model_Item given
Fixed Varien_Db_Adapter_Mysqli::raw_query() should throw an Exception after 10 tries
Fixed Import file downloaded from FTP in BINARY mode
- added option(ASCII || BINARY) for mode of file transferring;
- default mode of file transferring is BINARY;
- was changed property "type" of input field for password.
Fixed User interface: real mistake in the label name, Api instead API
Fixed issue with URL Rewrite Rule for new products with no category information
Fixed Invoice do not created when using "Automatically Invoice All Items" option of Zero Subtotal Checkout
Fixed Additional dot when checking out as Guest
Fixed Prefix and suffix aren't visible in Add New Address Form
Fixed Calculation order for Catalog Price Rule and Configurable Product option price
Fixed When put values in Customer Name and Address Options they do not reflect on the backend customer and customer address forms
Fixed Custom URL Rewrite creation broken
- skip filtering for store select if no product or category specified in case of custom rewrite
Fixed Shopping Cart Price Rule->Conditions->Shipping Country is not correctly controlled on multiple checkout.
- Added checking: if address object is a new object rules validation cache will not working because we can not save validation results for address without id
Fixed Resources names are not translated on Role Resources page at backend 
Fixed Multiselect and Dropdown Attribute values set to "0" are not exported correctly
Fixed WYSIWYG Editor - Unable to Create a Folder when Inserting a File
Fixed Wrong cache key for websites
- {{base_url}} not replaced with url on the saving in the cache. {{base_url}} replaced with  base url on the getting.
Fixed After second refund made from paypal user get wrong refund amounts
Fixed Multiselect and Dropdown Attribute values set to "0" are not exported correctly
- modified condition for option emptiness check to pass string and int zero values
Fixed Infinite loop is started, when backend user selects non-existing time period for a chart on Dashboard
Fixed Missing isset() in Mage_Sales_Model_Recurring_Profile::createOrder()
- Added the filtering "value" key on the setting in the conditions: Order Number, Purchased Quantity, Sales Amount
Fixed Discount is not applied to product in case when in conditions of Catalog Price Rule "contains" is chosen
Fixed Unable to open "View all wishlist items" link from email
Fixed Specifying incorrect timezone in configuration causes halt of backend work flow and inability to add products to a Cart on frontend
- Added timezone validation
Fixed Checkout with Configurable Product includes disabled simple
- removing parent from shopping cart if child becomes disabled or out of stock
Fixed Validate Each Address Separately in Multi-address Checkout do not working
Fixed Google Checkout - catalog price discount for Configurable product is calculated incorrectly
Fixed FPT with prices included tax problem
Fixed Incorrect Excl. Tax in product page, when catalog prices entered by admin include tax
- Fixed JS excluding tax price recalculation
Fixed Unable to configure Grouped product from the backend
Fixed Order, that related with Recurring Profile does not displayed
Fixed Discount is not applied to product in case when in conditions of Catalog Price Rule "contains" is chosen
Fixed After second refund made from paypal user get wrong refund amounts
Fixed WPPHS payment method has tags in the name
Fixed Symlinks do not work for back-end blocks
Fixed The names of WPPHS depend on a merchant`s country in the backend. Create a functionality for dynamic changing.
Fixed Disabled success redirect functionality in paypal express checkout
Fixed Added whitelist support to get.php script
Fixed Mage_Customer_Model_Address class name is hardcoded in certain models
Fixed Typo in Mage_ImportExport_Model_Import_Adapter_Abstract::_construct()
Fixed 'FOUND' and 'NOT FOUND' labels are not translated in Mage_SalesRule_Model_Rule_Condition_Product_Found::loadValueOptions()
Fixed 'Select' label is not translated in Mage_Adminhtml_Block_Sales_Order_Create_Search_Grid::_prepareColumns()
Fixed Invalid HTML from form multiline element renderer
Fixed Collection calling private _setOrder() method in CatalogEvent module
Fixed Tags on search results for Global Record Search (Adminhtml) are not translatable
Fixed JavaScript bug in IE8 with date advice set during js validation.
Fixed Missing translation for ZF error messages
- provided translation of ZF native validation error messages
Fixed Shopping Cart Price Rule->Conditions->Shipping Country is not correctly controlled on multiple checkout.
Fixed Moneybookers Multistore System Configuration
Fixed Moneybookers OBT Defaults
Fixed Product info API request
- a behavior of the function, was optimized;
- refactoring classes with calling function from helper without changing the inside logic;
- duplicated code were moved to catalog/product helper with creating the new one function for that.
Fixed typos in adminhtml widget form block
- Changed reserved word 'const' to lower case in tax config model
Fixed Google Base Synchronize
- Fixed fatal error on very first Publish and then Synchronizing if in GB products already were
- Fixed potential fatal when on mass Publish action we will not retrieve any item id: expected array, but null or empty string given
Fixed Rounding issues in shipping methods and in sales payment
Fixed Usage of non-mb-supported strlen() in custom option validation
- fixed length calculation routine to work with multi-byte characters
- changed order of evaluation, so that length is calculated only if length constraint is set for custom option
Fixed Unused class Mage_Reports_Model_Mysql4_Shopcart_Product_Collection did not marked like deprecated
- mark class as deprecated after 1.5.0.1
Fixed Products prepare function
- Change prepare products function
- Update resource with phpDoc
- Update wsdl
Improved SOAP Faults in Shopping Cart
- all faults for ShoppingCart are unique for each issue and have wide description
Fixed Shopping Cart create order should return order increment id
- updated wsdl, wsi
- changed return type for Mage_Checkout_Model_Cart_Api::createOrder
Fixed Grouped product has no configured price in Wishlist
Fixed Unable to continue checkout when "Street Address" use non english characters
Fixed Misprint in comment in Mage_Checkout_Model_Cart::init()
Fixed Controllers used protected properties
- removed protected property _hasDataChanges equals true in controllers
- added property _hasDataChanges equals true in method "addComment" for all objects
Fixed Page "404 Not Found" is showed by clicked Edit link in the Invoice page of placed order
Fixed Google Base Synchronize
Fixed Error on Authorize.net Direct Post payment method in Backend
Fixed API default/SOAP functionality switched
- removed unused variable loading
- changed loading default api handler in IndexController
- added loading default "soap" api handler in SoapController
Fixed Missed unique index on eav table
Fixed Order status visible_on_front flag in configuration file can't be overridden
Fixed Unexpected error message appears when quantity to refund more than quantity invoiced
Fixed PayPal payment methods are not shown on the checkout Payment Information step if Brazilian Real is set as base currency
- Added new supported currency codes into config
Fixed Trim value after explode
Fixed Unable to save customer date attribute with date more then 2010
Fixed No customer's information
Fixed PayPal Business Email address update
Fixed Hovering mouse cursor on "Configure" button for a composite product shows incorrect hint
Fixed Error in fulltext search indexation for values that contain 'à' character
- modified regular expression to correct process of unicode characters
Fixed Zooming don't work for an image larger or taller than the container
Fixed Variable  is used before its definition in Mage_CatalogRule_Helper_Data::calcPriceRule()
Fixed Typo in app\design\frontend\base\default\template\checkout\success.phtml
Fixed Fatal error during newsletters sending via cron
- Also added missed PHP-docs to Mage_Newsletter_Model_Problem class.
Fixed Quantity of bundle item is not stored correctly, in case when it is decimal
Fixed Unable to change configurable product name for store view
- the bug was in two HTML input tags with same names located on "General" and "Associated Products" tabs. One of them was been renamed to solve the problem.
Fixed Microsoft Excel 2007 fails to open Magento generated XML file
Fixed Admin page - incorrect displaying of pop-up message for gift options in Items Ordered block
Fixed One extra unnecessary product appears in Items Ordered list of placed Order, when payment is provided using Authorize.net Direct Post
Fixed If 3D Secure Card Validation is enabled then Gift Options section has wrong position during backend order creation
Fixed Reindex of Category Products for large catalogs is extremely slow
Fixed Product minimum quantity, add to cart
Fixed Created in Backend customer doubled after creation order for him and not save any addres information
Fixed Changes to helper text for the images for the application submission page
Fixed Redirect patch
Fixed product list images for iPad device to use base image
Fixed Sending invoice email don`t change the status
Fixed remove paypal country id hard coded
Fixed Mobile Controller issue
Fixed App locations (countries) do not match iTunes App Stores countries available
Fixed Disabled cookie message issue
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Web form with empty fields can be saved - also is_object() calls are replaced with instanceof checking inside of Adminhtml/MobileController
Fixed Bundle product with required option must have "Configure" button inactive if one of the option is out of stock.
Fixed Unable to retrieve product attributes, "Unsupported operand types"
Fixed Add to Wishlist is not work
Fixed A bug inside catalog/model/product/Api.php::create prevents this function from working
- Added $store parameter.
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- on frontend when "Use Secure URLs in Frontend" is set to "yes", https is used only for some selected pages. This fix takes into account what's the protocol in use
Fixed Improvement to block caching
Fixed Typo in Mage_Catalog_Model_Resource_Eav_Mysql4_Product_Type_Configurable_Attribute::savePrices()
Fixed Shipping creation for bundle product shows wrong q-ty
Fixed Check for controller instance in rating option resource model
Fixed Export Filters are not working correctly during export of customers
Fixed Function "Apply Tax On - Original price only" does not correct calculate product tax
Fixed Mage_Index.csv is not used at all
Fixed Incorrect tax count, when making new order through back-end and using discount coupon (price cart rule)
Fixed Error "Source file moving failed" on Import process, when PHP version is 5.2
Fixed "Store credit amount can not exceed order amount" error in Credit Memo applying to Store Credit for decimal quantities and decimal subtotals
Fixed Disabled cookie message issue
Fixed Edit Order without creating new one functionality doesn't save changes in non-default customer address attributes
Fixed Unable to buy Downloadable product with specified option "Links can be purchased separately" set to "No"
Fixed Incorrect message of soap fault
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Unable to open "View all wishlist items" link from email
- Added action to add shared wishlist item to shopping cart
Fixed iFrame must be centered for Website Payments Pro Hosted Solution payment method.
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Added support of UPS carrier methods with UPS XML type of rates calculation
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed PayPal Standart: order has two invoice and two refund
Fixed A product hasn't been added to whishlist from category with closed, upcoming events
Fixed Customer password is not imported from CSV file
Fixed CDN - necessary to replace information message
Fixed When put values in Customer Name and Address Options they do not reflect on the backend customer and customer address forms
Fixed Reports-> Products-> Products ordered - Trace appeared
Fixed Mage_Core_Helper_Url::getCurrentUrl() method ignores server PORT
Fixed No ability to change payment from Store Credits, when customer backs to a Cart from Order Review step, and then goes to checkout again (OnePageCheckout)
Fixed Customer attribute labels not translated in validation error messages
- added translation for attribute labels at classes Mage_Customer_Model_Attribute_Data_*
Fixed Typos in: Varien_Db_Adapter_Pdo_Mysql, Varien_File_Uploader
Fixed Mage_Core_Model_Design_Package::_prepareUrl() uses incorrect regular expression to check whether the url is relative
- modified preg_match for detecting absolute urls
Fixed Mage_Catalog_Block_Product_Gallery::getImageWidth() returns false for images with width smaller than 600px
- modified method Mage_Catalog_Block_Product_Gallery::getImageWidth(), if width <= 600 return width value, not false
Fixed Incorrect view of the shipping tax at the back end, unnecessary $0.01
Fixed Wrong visualisation of "Original Price" in placed order
- collecting totals for quote at multishipping checkout
Fixed Incorrect view of popup windows for composite product on backend (only IE)
Added Adding Composite Products in Admin Order Creation
- Fixed styles in ie7
Fixed "Items Ordered" tab is not refreshing while Admin order creation
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Re factored and optimized code
- Improved performance
- Added dependency for GoogleCheckout module from Usa module
- Added fedex and usps free methods supporting



==== 1.5.x-devel-104676 ====

=== Improvements ===
Magento Mobile updated to release v20

=== Fixes ===
Fixed PayPal Standard: order has two invoice and two refund
Fixed Adjustmen Fee, Adjustment Refund and Refund Shipping fields must be disabled on credit memo for Payflow Pro and PayFlowLink payment methods
- Actualized API params mapping 
- Added parameter Amount into refund request
Fixed Broken mysql4-data-upgrade-1.4.0.0.13-1.4.0.0.14.php file
Fixed XMLConnect - edited parameter cannot be saved
Fixed Media storage - problem with image in the CMS pages
- Added functional to get files with disabled db media storage feature through the get.php script
Fixed Unable to place order using PayPal Billing agreement through Checkout with multiple addresses
- Added additional multi shipping checkout exceptions logging.
Fixed No AmericanExpress support in Website Payments Pro Payflow Edition
- Added to Direct payment 
Fixed Incorrect Subtotal(Incl. Tax) in Shopping Cart, when catalog prices entered by admin include tax
Fixed Function "Apply Tax On - Original price only" does not correct calculate product tax
Fixed No ability to save Product Attribute with type Media Image


==== 1.5.1.0-rc1 ====

=== Improvements ===
Magento Mobile updated to release v19

=== Changes ===
Replaced usage of Varien_File_Uploader with Mage_Core_Model_File_Uploader

=== Fixes ===
Fixed Mage_CatalogSearch_Model_Query::getMaxQueryLenght() is not properly deprecated.
Fixed Two links in forgotpassword.phtml template lead to not existent files
Fixed Added compiled js and css to whitelist. Added removing of relative URL parts to get.php.
Fixed several probable vulnerabilities on front and backend
Fixed Incorrect error message when extension state is lower than preferred state
Fixed No rule applied when coupon code is no longer valid
- verify if rule uses coupon at all before coupon check
Fixed Argument passed to Mage_Catalog_Helper_Image::init() must be an instance of Mage_Catalog_Model_Product, instance of Mage_Wishlist_Model_Item given
Fixed Varien_Db_Adapter_Mysqli::raw_query() should throw an Exception after 10 tries
Fixed Import file downloaded from FTP in BINARY mode
- added option(ASCII || BINARY) for mode of file transferring;
- default mode of file transferring is BINARY;
- was changed property "type" of input field for password.
Fixed User interface: real mistake in the label name, Api instead API
Fixed issue with URL Rewrite Rule for new products with no category information
Fixed Invoice do not created when using "Automatically Invoice All Items" option of Zero Subtotal Checkout
Fixed Additional dot when checking out as Guest
Fixed Prefix and suffix aren't visible in Add New Address Form
Fixed Calculation order for Catalog Price Rule and Configurable Product option price
Fixed When put values in Customer Name and Address Options they do not reflect on the backend customer and customer address forms
Fixed Custom URL Rewrite creation broken
- skip filtering for store select if no product or category specified in case of custom rewrite
Fixed Shopping Cart Price Rule->Conditions->Shipping Country is not correctly controlled on multiple checkout.
- Added checking: if address object is a new object rules validation cache will not working because we can not save validation results for address without id
Fixed Resources names are not translated on Role Resources page at backend 
Fixed Multiselect and Dropdown Attribute values set to "0" are not exported correctly
Fixed WYSIWYG Editor - Unable to Create a Folder when Inserting a File
Fixed Wrong cache key for websites
- {{base_url}} not replaced with url on the saving in the cache. {{base_url}} replaced with  base url on the getting.
Fixed After second refund made from paypal user get wrong refund amounts
Fixed Multiselect and Dropdown Attribute values set to "0" are not exported correctly
- modified condition for option emptiness check to pass string and int zero values
Fixed Infinite loop is started, when backend user selects non-existing time period for a chart on Dashboard
Fixed Missing isset() in Mage_Sales_Model_Recurring_Profile::createOrder()
- Added the filtering "value" key on the setting in the conditions: Order Number, Purchased Quantity, Sales Amount
Fixed Discount is not applied to product in case when in conditions of Catalog Price Rule "contains" is chosen
Fixed Unable to open "View all wishlist items" link from email
Fixed Specifying incorrect timezone in configuration causes halt of backend work flow and inability to add products to a Cart on frontend
- Added timezone validation
Fixed Checkout with Configurable Product includes disabled simple
- removing parent from shopping cart if child becomes disabled or out of stock
Fixed Validate Each Address Separately in Multi-address Checkout do not working
Fixed Google Checkout - catalog price discount for Configurable product is calculated incorrectly
Fixed FPT with prices included tax problem
Fixed Incorrect Excl. Tax in product page, when catalog prices entered by admin include tax
- Fixed JS excluding tax price recalculation
Fixed Unable to configure Grouped product from the backend
Fixed Order, that related with Recurring Profile does not displayed
Fixed Discount is not applied to product in case when in conditions of Catalog Price Rule "contains" is chosen
Fixed After second refund made from paypal user get wrong refund amounts
Fixed WPPHS payment method has tags in the name

==== 1.5.x-devel-102426 ====

=== Improvements ===
Magento Mobile updated to release v19

=== Changes ===
Replaced usage of Varien_File_Uploader with Mage_Core_Model_File_Uploader

=== Fixes ===
Fixed Mage_CatalogSearch_Model_Query::getMaxQueryLenght() is not properly deprecated.
Fixed Two links in forgotpassword.phtml template lead to not existent files
Fixed Added compiled js and css to whitelist. Added removing of relative URL parts to get.php.
Fixed several probable vulnerabilities on front and backend
Fixed Incorrect error message when extension state is lower than preferred state
Fixed No rule applied when coupon code is no longer valid
- verify if rule uses coupon at all before coupon check
Fixed Argument passed to Mage_Catalog_Helper_Image::init() must be an instance of Mage_Catalog_Model_Product, instance of Mage_Wishlist_Model_Item given
Fixed Varien_Db_Adapter_Mysqli::raw_query() should throw an Exception after 10 tries
Fixed Import file downloaded from FTP in BINARY mode
- added option(ASCII || BINARY) for mode of file transferring;
- default mode of file transferring is BINARY;
- was changed property "type" of input field for password.
Fixed User interface: real mistake in the label name, Api instead API
Fixed issue with URL Rewrite Rule for new products with no category information
Fixed Invoice do not created when using "Automatically Invoice All Items" option of Zero Subtotal Checkout
Fixed Additional dot when checking out as Guest
Fixed Prefix and suffix aren't visible in Add New Address Form



==== 1.5.1.0-beta1 ====

=== Improvements ===
Implemented SOAP Faults for GiftMessage API
- added faults in functions
- added description in api.xml
Implemented The names of WPPHS depend on a merchant`s country in the backend. Create a functionality for dynamic changing.
- Added functionality for dynamic changing the names of WPPHS
- Added backend config into system.xml
Implemented WS-I for API
- added wsi.xml for all WebAPI modules
- added new wsi-soap handler
- added new wsi-soap adapter
- changed admin configuration, added parameter into "Magento Core API"->WSI Compliance
- changed api.xml
Implemented GiftMessage for Cart

=== Changes ===
Updated Magento Mobile package to ver. 18

=== Fixes ===
Fixed Symlinks do not work for back-end blocks
Fixed The names of WPPHS depend on a merchant`s country in the backend. Create a functionality for dynamic changing.
Fixed Disabled success redirect functionality in paypal express checkout
Fixed Added whitelist support to get.php script
Fixed Mage_Customer_Model_Address class name is hardcoded in certain models
Fixed Typo in Mage_ImportExport_Model_Import_Adapter_Abstract::_construct()
Fixed 'FOUND' and 'NOT FOUND' labels are not translated in Mage_SalesRule_Model_Rule_Condition_Product_Found::loadValueOptions()
Fixed 'Select' label is not translated in Mage_Adminhtml_Block_Sales_Order_Create_Search_Grid::_prepareColumns()
Fixed Invalid HTML from form multiline element renderer
Fixed Collection calling private _setOrder() method in CatalogEvent module
Fixed Tags on search results for Global Record Search (Adminhtml) are not translatable
Fixed JavaScript bug in IE8 with date advice set during js validation.
Fixed Missing translation for ZF error messages
- provided translation of ZF native validation error messages
Fixed Shopping Cart Price Rule->Conditions->Shipping Country is not correctly controlled on multiple checkout.
Fixed Moneybookers Multistore System Configuration
Fixed Moneybookers OBT Defaults
Fixed Product info API request
- a behavior of the function, was optimized;
- refactoring classes with calling function from helper without changing the inside logic;
- duplicated code were moved to catalog/product helper with creating the new one function for that.
Fixed Poor randomness of auto-generated passwords in Customer Model
- was used function from core helper;
- code style has been formatted.
Fixed several probable vulnerabilities on front and backend
Fixed typos in adminhtml widget form block
- Changed reserved word 'const' to lower case in tax config model
Fixed Google Base Synchronize
- Fixed fatal error on very first Publish and then Synchronizing if in GB products already were
- Fixed potential fatal when on mass Publish action we will not retrieve any item id: expected array, but null or empty string given
Fixed Rounding issues in shipping methods and in sales payment
Fixed Usage of non-mb-supported strlen() in custom option validation
- fixed length calculation routine to work with multi-byte characters
- changed order of evaluation, so that length is calculated only if length constraint is set for custom option
Fixed Unused class Mage_Reports_Model_Mysql4_Shopcart_Product_Collection did not marked like deprecated
- mark class as deprecated after 1.5.0.1
Fixed Products prepare function
- Change prepare products function
- Update resource with phpDoc
- Update wsdl
Improved SOAP Faults in Shopping Cart
- all faults for ShoppingCart are unique for each issue and have wide description
Fixed Shopping Cart create order should return order increment id
- updated wsdl, wsi
- changed return type for Mage_Checkout_Model_Cart_Api::createOrder
Fixed Grouped product has no configured price in Wishlist
Fixed Unable to continue checkout when "Street Address" use non english characters
Fixed Misprint in comment in Mage_Checkout_Model_Cart::init()
Fixed Controllers used protected properties
- removed protected property _hasDataChanges equals true in controllers
- added property _hasDataChanges equals true in method "addComment" for all objects
Fixed Page "404 Not Found" is showed by clicked Edit link in the Invoice page of placed order
Fixed Google Base Synchronize
Fixed probably SQL-injection in backend
Fixed Error on Authorize.net Direct Post payment method in Backend
Fixed API default/SOAP functionality switched
- removed unused variable loading
- changed loading default api handler in IndexController
- added loading default "soap" api handler in SoapController
Fixed Missed unique index on eav table
Fixed Its possible to add&proceed to checkout with any product from the catalog no matter website its assign to.
Fixed Order status visible_on_front flag in configuration file can't be overridden
Fixed Unexpected error message appears when quantity to refund more than quantity invoiced
Fixed PayPal payment methods are not shown on the checkout Payment Information step if Brazilian Real is set as base currency
- Added new supported currency codes into config
Fixed Trim value after explode
Fixed Unable to save customer date attribute with date more then 2010
Fixed No customer's information
Fixed PayPal Business Email address update
Fixed probable abuse with image re-size functionality on frontend
Fixed Hovering mouse cursor on "Configure" button for a composite product shows incorrect hint
Fixed Error in fulltext search indexation for values that contain 'à' character
- modified regular expression to correct process of unicode characters
Fixed Zooming don't work for an image larger or taller than the container
Fixed Variable  is used before its definition in Mage_CatalogRule_Helper_Data::calcPriceRule()
Fixed Typo in app\design\frontend\base\default\template\checkout\success.phtml
Fixed Fatal error during newsletters sending via cron
- Also added missed PHP-docs to Mage_Newsletter_Model_Problem class.
Fixed Quantity of bundle item is not stored correctly, in case when it is decimal
Fixed Unable to change configurable product name for store view
- the bug was in two HTML input tags with same names located on "General" and "Associated Products" tabs. One of them was been renamed to solve the problem.
Fixed Microsoft Excel 2007 fails to open Magento generated XML file
Fixed several probable XSS issues on front end and backend
Fixed Admin page - incorrect displaying of pop-up message for gift options in Items Ordered block
Fixed One extra unnecessary product appears in Items Ordered list of placed Order, when payment is provided using Authorize.net Direct Post
Fixed If 3D Secure Card Validation is enabled then Gift Options section has wrong position during backend order creation
Fixed Reindex of Category Products for large catalogs is extremely slow
Fixed Product minimum quantity, add to cart
Fixed Created in Backend customer doubled after creation order for him and not save any addres information
Fixed Changes to helper text for the images for the application submission page
Fixed Redirect patch
Fixed product list images for iPad device to use base image
Fixed Sending invoice email don`t change the status
Fixed remove paypal country id hard coded
Fixed Mobile Controller issue
Fixed App locations (countries) do not match iTunes App Stores countries available
Fixed Disabled cookie message issue
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Web form with empty fields can be saved - also is_object() calls are replaced with instanceof checking inside of Adminhtml/MobileController
Fixed Bundle product with required option must have "Configure" button inactive if one of the option is out of stock.
Fixed Unable to retrieve product attributes, "Unsupported operand types"
Fixed Add to Wishlist is not work
Fixed A bug inside catalog/model/product/Api.php::create prevents this function from working
- Added $store parameter.
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- on frontend when "Use Secure URLs in Frontend" is set to "yes", https is used only for some selected pages. This fix takes into account what's the protocol in use
Fixed Improvement to block caching
Fixed Typo in Mage_Catalog_Model_Resource_Eav_Mysql4_Product_Type_Configurable_Attribute::savePrices()
Fixed Shipping creation for bundle product shows wrong q-ty
Fixed Check for controller instance in rating option resource model
Fixed Export Filters are not working correctly during export of customers
Fixed Function "Apply Tax On - Original price only" does not correct calculate product tax
Fixed Mage_Index.csv is not used at all
Fixed Incorrect tax count, when making new order through back-end and using discount coupon (price cart rule)
Fixed Error "Source file moving failed" on Import process, when PHP version is 5.2
Fixed "Store credit amount can not exceed order amount" error in Credit Memo applying to Store Credit for decimal quantities and decimal subtotals
Fixed Disabled cookie message issue
Fixed Edit Order without creating new one functionality doesn't save changes in non-default customer address attributes
Fixed Unable to buy Downloadable product with specified option "Links can be purchased separately" set to "No"
Fixed Incorrect message of soap fault
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Unable to open "View all wishlist items" link from email
- Added action to add shared wishlist item to shopping cart
Fixed iFrame must be centered for Website Payments Pro Hosted Solution payment method.
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Added support of UPS carrier methods with UPS XML type of rates calculation
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed PayPal Standart: order has two invoice and two refund
Fixed A product hasn't been added to whishlist from category with closed, upcoming events
Fixed Customer password is not imported from CSV file
Fixed CDN - necessary to replace information message
Fixed When put values in Customer Name and Address Options they do not reflect on the backend customer and customer address forms
Fixed Reports-> Products-> Products ordered - Trace appeared
Fixed Mage_Core_Helper_Url::getCurrentUrl() method ignores server PORT
Fixed No ability to change payment from Store Credits, when customer backs to a Cart from Order Review step, and then goes to checkout again (OnePageCheckout)
Fixed Customer attribute labels not translated in validation error messages
- added translation for attribute labels at classes Mage_Customer_Model_Attribute_Data_*
Fixed Typos in: Varien_Db_Adapter_Pdo_Mysql, Varien_File_Uploader
Fixed Mage_Core_Model_Design_Package::_prepareUrl() uses incorrect regular expression to check whether the url is relative
- modified preg_match for detecting absolute urls
Fixed Mage_Catalog_Block_Product_Gallery::getImageWidth() returns false for images with width smaller than 600px
- modified method Mage_Catalog_Block_Product_Gallery::getImageWidth(), if width <= 600 return width value, not false
Fixed Incorrect view of the shipping tax at the back end, unnecessary $0.01
Fixed Wrong visualisation of "Original Price" in placed order
- collecting totals for quote at multishipping checkout
Fixed Incorrect view of popup windows for composite product on backend (only IE)
Added Adding Composite Products in Admin Order Creation
- Fixed styles in ie7
Fixed "Items Ordered" tab is not refreshing while Admin order creation
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Re factored and optimized code
- Improved performance
- Added dependency for GoogleCheckout module from Usa module
- Added fedex and usps free methods supporting


==== 1.5.x-devel-100810 ====

=== Fixes ===

Fixed Shopping Cart Price Rule->Conditions->Shipping Country is not correctly controlled on multiple checkout.
Fixed Moneybookers Multistore System Configuration
Fixed Moneybookers OBT Defaults
Fixed Product info API request
- a behavior of the function, was optimized;
- refactoring classes with calling function from helper without changing the inside logic;
- duplicated code were moved to catalog/product helper with creating the new one function for that.
Fixed Poor randomness of auto-generated passwords in Customer Model
- was used function from core helper;
- code style has been formatted.
Fixed several probable vulnerabilities on front and backend
Fixed typos in adminhtml widget form block
- Changed reserved word 'const' to lower case in tax config model
Fixed Google Base Synchronize
- Fixed fatal error on very first Publish and then Synchronizing if in GB products already were
- Fixed potential fatal when on mass Publish action we will not retrieve any item id: expected array, but null or empty string given
Fixed Rounding issues in shipping methods and in sales payment
Fixed Usage of non-mb-supported strlen() in custom option validation 
- fixed length calculation routine to work with multi-byte characters
- changed order of evaluation, so that length is calculated only if length constraint is set for custom option
Fixed Unused class Mage_Reports_Model_Mysql4_Shopcart_Product_Collection did not marked like deprecated 
- mark class as deprecated after 1.5.0.1


==== 1.5.x-devel-100247 ====

=== Improvements ===
Implemented GiftMessage API Faults
- added faults in functions
- added description in api.xml
Implemented The names of WPPHS depend on a merchant`s country in the backend. Create a functionality for dynamic changing.
- Added functionality for dynamic changing the names of WPPHS
- Added backend config into system.xml

=== Fixes ===
Fixed Products prepare function
- Change prepare products function
- Update resource with phpDoc
- Update wsdl
Improved Faults in Shopping Cart
- all faults for ShoppingCart are unique for each issue and have wide description
Fixed Shopping Cart create order should return order increment id
- updated wsdl, wsi
- changed return type for Mage_Checkout_Model_Cart_Api::createOrder
Fixed Grouped product has no configured price in Wishlist
Fixed Unable to continue checkout when "Street Address" use non english characters
Fixed Misprint in comment in Mage_Checkout_Model_Cart::init()
Fixed Controllers used protected properties
- removed protected property _hasDataChanges equals true in controllers
- added property _hasDataChanges equals true in method "addComment" for all objects
Fixed Page "404 Not Found" is showed by clicked Edit link in the Invoice page of placed order
Fixed probably XSS vulnerabilities in backend
Fixed Google Base Synchronize
Fixed probably SQL-injection in backend
Fixed Error on Authorize.net Direct Post payment method in Backend
Fixed API default/SOAP functionality switched
- removed unused variable loading
- changed loading default api handler in IndexController
- added loading default "soap" api handler in SoapController
Fixed Missed unique index on eav table
Fixed Its possible to add&proceed to checkout with any product from the catalog no matter website its assign to.
Fixed Order status visible_on_front flag in configuration file can't be overridden
Fixed Unexpected error message appears when quantity to refund more than quantity invoiced
Fixed PayPal payment methods are not shown on the checkout Payment Information step if Brazilian Real is set as base currency
- Added new supported currency codes into config
Fixed Trim value after explode
Fixed Unable to save customer date attribute with date more then 2010
Fixed No customer's information
Fixed PayPal Business Email address update


==== 1.5.x-devel-96719 ====

=== Improvements ===
Implemented WS-I for API
- added wsi.xml for all WebAPI modules
- added new wsi-soap handler
- added new wsi-soap adapter
- changed admin configuration, added parameter into "Magento Core API"->WSI Compliance
- changed api.xml
Implemented GiftMessage for Cart

== Fixes ===
Fixed probable abuse with image re-size functionality on frontend
Fixed Hovering mouse cursor on "Configure" button for a composite product shows incorrect hint
Fixed Error in fulltext search indexation for values that contain 'à' character
- modified regular expression to correct process of unicode characters
Fixed Zooming don't work for an image larger or taller than the container
Fixed Variable  is used before its definition in Mage_CatalogRule_Helper_Data::calcPriceRule()
Fixed Typo in app\design\frontend\base\default\template\checkout\success.phtml
Fixed Fatal error during newsletters sending via cron
- Also added missed PHP-docs to Mage_Newsletter_Model_Problem class.
Fixed Quantity of bundle item is not stored correctly, in case when it is decimal
Fixed Unable to change configurable product name for store view
- the bug was in two HTML input tags with same names located on "General" and "Associated Products" tabs. One of them was been renamed to solve the problem.
Fixed Microsoft Excel 2007 fails to open Magento generated XML file
Fixed several probable XSS issues on front end and backend
Fixed probable SQL injection on frontend
Fixed Admin page - incorrect displaying of pop-up message for gift options in Items Ordered block
Fixed One extra unnecessary product appears in Items Ordered list of placed Order, when payment is provided using Authorize.net Direct Post
Fixed If 3D Secure Card Validation is enabled then Gift Options section has wrong position during backend order creation
Fixed Reindex of Category Products for large catalogs is extremely slow
Fixed Product minimum quantity, add to cart
Fixed Created in Backend customer doubled after creation order for him and not save any addres information
Fixed Changes to helper text for the images for the application submission page
Fixed Redirect patch
Fixed product list images for iPad device to use base image
Fixed Sending invoice email don`t change the status
Fixed remove paypal country id hard coded
Fixed Mobile Controller issue
Fixed App locations (countries) do not match iTunes App Stores countries available
Fixed Disabled cookie message issue
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Web form with empty fields can be saved - also is_object() calls are replaced with instanceof checking inside of Adminhtml/MobileController
Fixed Bundle product with required option must have "Configure" button inactive if one of the option is out of stock.
Fixed Unable to retrieve product attributes, "Unsupported operand types"
Fixed Add to Wishlist is not work
Fixed A bug inside catalog/model/product/Api.php::create prevents this function from working
- Added $store parameter.
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- on frontend when "Use Secure URLs in Frontend" is set to "yes", https is used only for some selected pages. This fix takes into account what's the protocol in use
Fixed Improvement to block caching
Fixed Typo in Mage_Catalog_Model_Resource_Eav_Mysql4_Product_Type_Configurable_Attribute::savePrices()
Fixed Shipping creation for bundle product shows wrong q-ty
Fixed Check for controller instance in rating option resource model
Fixed Export Filters are not working correctly during export of customers
Fixed Function "Apply Tax On - Original price only" does not correct calculate product tax
Fixed Mage_Index.csv is not used at all
Fixed Incorrect tax count, when making new order through back-end and using discount coupon (price cart rule)
Fixed Error "Source file moving failed" on Import process, when PHP version is 5.2
Fixed "Store credit amount can not exceed order amount" error in Credit Memo applying to Store Credit for decimal quantities and decimal subtotals
Fixed Disabled cookie message issue
Fixed Edit Order without creating new one functionality doesn't save changes in non-default customer address attributes
Fixed Unable to buy Downloadable product with specified option "Links can be purchased separately" set to "No"
Fixed Incorrect message of soap fault
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Unable to open "View all wishlist items" link from email
- Added action to add shared wishlist item to shopping cart
Fixed iFrame must be centered for Website Payments Pro Hosted Solution payment method.
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Added support of UPS carrier methods with UPS XML type of rates calculation
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed PayPal Standart: order has two invoice and two refund
Fixed A product hasn't been added to whishlist from category with closed, upcoming events
Fixed Customer password is not imported from CSV file
Fixed CDN - necessary to replace information message
Fixed When put values in Customer Name and Address Options they do not reflect on the backend customer and customer address forms
Fixed Reports-> Products-> Products ordered - Trace appeared


==== 1.5.x-devel-96719 ====

=== Fixes ===
Fixed Mage_Core_Helper_Url::getCurrentUrl() method ignores server PORT
Fixed No ability to change payment from Store Credits, when customer backs to a Cart from Order Review step, and then goes to checkout again (OnePageCheckout)
Fixed Customer attribute labels not translated in validation error messages
- added translation for attribute labels at classes Mage_Customer_Model_Attribute_Data_*
Fixed Typos in: Varien_Db_Adapter_Pdo_Mysql, Varien_File_Uploader
Fixed Mage_Core_Model_Design_Package::_prepareUrl() uses incorrect regular expression to check whether the url is relative
- modified preg_match for detecting absolute urls
Fixed Mage_Catalog_Block_Product_Gallery::getImageWidth() returns false for images with width smaller than 600px
- modified method Mage_Catalog_Block_Product_Gallery::getImageWidth(), if width <= 600 return width value, not false
Fixed Incorrect view of the shipping tax at the back end, unnecessary $0.01
Fixed Wrong visualisation of "Original Price" in placed order
- collecting totals for quote at multishipping checkout
Fixed Incorrect view of popup windows for composite product on backend (only IE)
Added Adding Composite Products in Admin Order Creation
- Fixed styles in ie7
Fixed "Items Ordered" tab is not refreshing while Admin order creation
Fixed Free shipping does not transfer to Google Checkout when it is enabled in a shipping method
- Re factored and optimized code
- Improved performance
- Fixed typos
- Added dependency for GoogleCheckout module from Usa module 
- Added fedex and usps free methods supporting


==== 1.5.0.1 =====

=== Major Highlights ===
Due to a design flaw we are removing alternative image storage feature from this release. It will be redesigned and released in our upcoming releases

==== 1.5.0.0 =====

=== Major Highlights ===
Added Payflow Link using HSS (Hosted Sole Solution) 
Balance Response, Partial Authorization Transactions, Authorization Reversals Support for MasterCard and Discover with Authorize.net
3D Secure Authentication for Authorize.net payment method
Authorize.Net SIM payment method
Improved Import/Export functionality
Ability to order composite products from backend including:
- reconfigure already added products on front end
- adding preconfigured products in wish-list
Alternative media storage options
- Database
- CDN
Order status management
- ability to add new status and assign to some state
- statuses now stored in DB table instead of configuration file
Ability to edit order addresses for an existing order
- this functionality admin has link to edit address for order view page
Magento Mobile included in base packaging

=== Improvements ===
Implemented Environment emulation in core email class
- Added Emulation model.
- Added Email Info and Email Template Mailer models.
- Re-factored sendEmail() and sendUpdateEmail() methods of order, credit memo, invoice and shipment models.
Added App Previewer for Android and iPad in XmlConenect
Upgraded Zend Framework to 1.11.0
Implemented new process of hashing parameters in Ogone payment method
- implemented an advanced hashing method that invokes all transaction parameters for building security hash
- updated fields sort order in system configuration
- added the new parameter which designates whether to use the old or advanced hashing method
- made SHA-IN and SHA-OUT sys config parameter titles corresponding to parameter titles on merchant site in Ogone
- major refactoring of the Ogone helper: simplified public interface of hash validation, added support for SHA-1, SHA-256 and SHA-512 algorithms (not selectable in system config)
- optimized performance of debugging and building redirect form: removed 2 excessive calls (one from template, another from debugging - it invoked form building even if debugging was disabled)
- since the form is built from a block, prevented injecting SID parameter to URLs when building form
- added HTML escaping in the template hidden fields
- added new system configuration parameter - hashing algorithm
- verified/fixed all API hashing parameters in accordance to documentation v.5.0
Fixed several memory leaks in product model. Added tool method clear() to clean object data and references to this object
Implemented Order payment action for PayPal
Implemented SOAP Api calls for shopping cart
Upgraded Zend Framework to 1.11.1
Phoenix_Moneybookers improvements:
- updated payment logo images
- added "Maestro" and "Online Bank Transfer" payment methods into Moneybookers group
- wrapped Moneybookers payment logo title and alt text on payment selection text into translation calls


=== Changes ===
Paypal HSS payment method label, comment and default title

=== Fixes ===
Fixed User cannot place order using Paypal payment methods with 3d secure
Fixed iPhone product list preview
Fixed App locations (countries) do not match iTunes App Stores countries available
Fixed Added parent quote items to discount calculation to prevent skipping of configurable products.
Fixed Rounding issue on front end if discount with fixed amount is applied and no tax rules applies to the order.
- added rounding item discount before take away from total discount
Fixed Fatal error after deleting one of the shipping addresses during checkout with multiple addresses
Fixed Merged CSS files with selected native Database as media storage are not applied with Chrome and FF
- first trying to detect MIME type manually, and only after by native php function
Fixed The buttons "Accept Payment" and "Deny Payment" do not appear in orders with status 'Payment Review'
Fixed issue when Simple products not visible individually (part of grouped) are moved to Wishlist
Fixed Impossible to delete product from Items Ordered (backend Order creation) using "remove" in Action dropdown
Fixed Fatal error after deleting one of the shipping addresses during checkout with multiple addresses
Fixed Qty for simple products (part of grouped) is incorrect when moved from order to Wishlist
- additional fixture for other testcase
Fixed Grouped product is added to Items Ordered as grouped, when any of buttons in sideblocks is pressed after product configuration in a product grid (backend Order creation)
- prevent to add unconfigured grouped product on server side
- in sales.js, do productConfigure.clean('quote_items') only if "Items Ordered" block is going to update
- in sales.js, hide "Search" block only when product added to qoute from "Search" block
- in configure.js, added ability to cleaning by list type scope
Fixed Incorrect behavior of Partial Authorization process, when admin user cancels authorizations (Authorize.net)
- added reloading block 'totals' after canceling partial authorization
Fixed Google Checkout Issue - Transactions not appearing
- adding transaction (transaction id = google order id) for googlecheckout payment
- fixed usage of Mage_GoogleCheckout_Model_Api_Xml_Callback::_getTaxClassForShipping() method according to it's interface
- fixed usage of Mage_GoogleCheckout_Model_Api_Xml_Abstract::_getTaxClassForShipping() method according to it's interface
- creating transactions for refund and chargeback
Fixed Missed index on sales.order table
Fixed Price for composite products in a products grid on Order creation page
Fixed Status of Order is now doesn't ignore the setting in Config for AUTH_AND_CAPTURE orders.
Fixed Unable to install extension using MCM for CE
Fixed Rounding error
Fixed Preview iFrame of iPhone recieve error message
- wrap images manipulations with try-catch (in controller)
- alert the catched error message when preview is loaded
Fixed Most product attibutes not exporting
Fixed Removed error message on new orders payd by PayflowLink with "complete" status (like on virtual products)
Fixed Behavior when customer changes billing/shipping address and/or changes items in cart, etc having started Partial Authorization
- added chopping cart`s and address checksum checking for partial authorization process
Fixed Moving composite products from shopping cart to wishlist does not work
- fixed error handling - added catching and processing, so in case of errors only item with error will not be moved
- fixed wishlist items to get right storeId (by passing product, and not productId)
Fixed Rounding issue (1 cent) appears on Tax Calculation Method Based On = Row
Fixed category/product image resizing
- Image sizes for Ipad has been changed
- Re-Factored: Application model call has been changed to helper method for all old calls
Fixed Only check money payment at standard chechout process receive success
Fixed Edit fonts configuration for iPad
Added iPad preview should illustrate tabs' state.
- Made separate icons
- Active/inactive logic added
- Added custom fonts for rating color customization
- Fixed positions for the icons
- Removed icons labels
- "i"-icon should always be on screen (currently it becomes hidden after making "information"-tab inactive)
Fixed Review collection need to sort with the latest added review
Fixed XML Connect - Incorrect help link in Push Notification page
Fixed API Certificate Based Authentication Used default signature value instead of the Certificate value
Fixed XML Connect - Design page - Ipad backgrounds issue
Fixed "Ship to different address" is not applied with IE8 with any payment method
Fixed Added skipping delta in shipping calculation on free shipping
Fixed Incorrect behavior of Gift Options popup for bundle product on backend Order View page. No ability to close popup
Fixed Rounding issue (1 cent) appears on discount applied and Tax Calculation Method Based On = Row
Fixed Add landscape mode background for Android and update information for portrait mode background
- changed <backgroundImageAndroid> to <backgroundAndroidPortraitImage>,
- changed all <someimagetagImageDeviceOrientatin> to <someimagetagDeviceOrientatinImage> for correctly image resizings,
- same for Icon,
- added orientation divisions for Android devices,
- fixed wrong spelled word "Portret" onto "Portrait" for iPad's config tags
- Image resize method has been changed
- backround getter method fixed
Fixed Tax rates export doesn't work
Fixed Incorrect downloader version in footer
Changed default title for HSS payment method
Fixed Rounding issue on credit memos/invoices causing different totals in magento and 1 cent error on paypal
- added adjustment for invoice`s subtotal_incl_tax and base_subtotal_incl_tax if invoice is last invoice of order
Fixed Added setting of store id in payment method instance on Authorize.net partial authorization cancel from admin place.
Fixed Fix Android preview area
- Added custom fonts
- Fixed header icons borders
- Fixed button border on homepage
- Added custom color declaration
Fixed Tabs dont affect second preview screen for Android mobile application
Fixed Incorrect design for Android mobile application in IE8
Added update Preview Area for iPad
- Fixed incorrect design for Ipad mobile application in IE8
- added stars custom fonts for landscape mode
- Fixed wrong positioning of the icons in landscape mode
Fixed Double use Authorize.net Partial Authorization Multicard with 46225 zip in one order causes wrong checkout behavior
Fixed Using MCM 2.0 shell script produces warnings and doesn't work correctly
Fixed Labels for composite products (backend) are shown incorrect
Fixed Ability to Refund the already refunded item in Patial Invoice
- added qty`s limits into creating creditmemo functionality
Fixed Performance issue with big amount of tax rates
Fixed Notice error in system.xml after saving PayPal configuration
Fixed No Qty column in the Wishlist sideblock
Fixed Export functionality doesn't work
Fixed Maestro International CC number has no validation
- use "Switch/Maestro" instead of "Maestro (International)"
Fixed No transactions is created, no ability to perform Invoice, when Order, which contains Gift Options, is placed from backend with Authorize.net Direct Post payment method
Fixed Moving Grouped product from Order and Shopping cart to the Wishlist does not work
Fixed Added advice block hiding on synchronize process
Fixed Database as cache backend
- fix for MySQL 4. Shorten field lengthes
Fixed Improvemets for MCM and Magento Extension Packager after MCMUP
Fixed PayPal Standard with specific tax settings for shop cart item with qty >= 2
Fixed Wrong tax calculation for bundle products
Fixed Export Filters are not working correctly during export of customers
Fixed Unable to complete several partial online refunds with Authorize.net Direct Post
Fixed Disable Mage_Checkout did not remove My Cart & Checkout links in the Top Link
Fixed An error occurs with using Payflo Link payment method and IE8
- just small fixture of strange for user popup in IE - "Do you want to see only secure content?"
Fixed Price for composite products in a products grid on Order creation page
Fixed No error message appears if execute synchronization with non-existing DB
Fixed "Configure" link in Product grid (backend) does not work (only IE)
Fixed "Void" button must not be active on the invoice with amount captured on-line
- redefined methods canVoid for Express and Direct Paypal models - hiding button void for invoice and creditmemo
- redefined methods cancel for Express and Direct Paypal models - no checking for invoices for order to decide void it or not at cancel.
Fixed Dropdown for Amount is absent (only IE)
- create new JS method that preserves visibility states of selects in pop-up block
Fixed Status of Order is now doesn't ignore the setting in Config.
Fixed Incorrect behavior of AJAX-popup for Gift Options (Individual Item) in IE8
Fixed to show full review for the iPad device
- added checking the current app's device type is not iPad and in this case the text of the review is truncated;
- replaced TABs on spaces in helper's class
- Re-factored XmlConnect helperfor unknown device type
Fixed xmlconnect/catalog/product action returns invalid html for product's description
- added an "xml" tag before DOCTYPE definition
Fixed wrong using of translation in method getElementHtml()
Fixed update Preview Area for iPad
Fixed Missed active/Inactive tabs logic added for a preview
Fixed Selecting catalog as a price rule condition redirects you on dashboard
- check if post array values are integers > 0
Fixed "Go to notifications" link works improperly
Fixed Unable to complete several partial online refunds with Authorize.net Direct Post
Fixed "Set Products as New to Date" is not working in Catalog New Products List widget
Fixed Mage_Adminhtml_Block_Media_Uploader::getUploaderUrl() generates incorrect path if magento is installed in a sub-directory within the root one
Fixed Now in Admin in System->TransactionalEmails all filters are saved to session.
Fixed Tax discrepancy between Tax Report and Order Report
Fixed PayPal Standard with specific tax settings for shop cart item with qty >= 2
Fixed Incorrect hint for non-configured product in Order on backend
Fixed Flush Cache Storage alert text is now changed to: "Cache storage may contain additional data. Are you sure that you want flush it?"
Fixed "Read Details" link is present in the message about synchronization status
- removed read details link from rows which have not url
Fixed Mage_Catalog_Model_Product::setFinalPrice() doesn't return its class instance for chaining purposes.
- fixed interface erroneously changed in 1.4.1.0
- fixed erroneous phpDoc
Fixed First Checkout by registered Customer: First Name and Last name fields are empty
Fixed Error with addlisttype.phtml in system log
- Removed not deleted layout block that was forgotten after rev 90337 with fix for MAGE-1955
Fixed Changes in UI for Order Status Management
Fixed Catalog Price Rule is not applied
- Added Mage_CatalogRule_Model_Rule::applyAllRulesToProduct()
Fixed Admin order creation - Unable to delete product from the cart
- fixed showing giftmessage options template, when no grid items are present
- fixed updating quote items and giftmessage items when backend receives wrong item id - now it doesn't fail with exception, but process it gracefully
Fixed With IE6 impossible to configure a Composite product in Backend
Fixed Message for non-configured composite product is changed after pressing "Update Items and Qty's"
Fixed Option "Order" on Payment Action dropdown must be available only for Express Checkout method
- Removed extra spaces in system.xml.
Fixed With IE8 an error occurs after applying the second time Credit Card in Admin panel with 3D Secure and partial authorization (Authorize.net)
- moved embedded gift options FORM tag out of other main FORM tag (such invalid layout broke DOM in IE)
- refactored JS-scripts, moved static to static files
- removed not used old js-file
Fixed Products are erased from "Product Ordered" report after deleting them
Fixed Incorrect behavior of Reorder action applied to Order, that contains Gift Options
Fixed When adding several configurable products at one time to Items Ordered from product grid, only last remains specified configuration (admin Order creation)
- restored JS-initing for controls on each popup show (was erroneously removed at rev 86017)
- fixed Configurable javascript so it won't interfere with other products controls on page
Fixed Incorrect transaction and Partial Refunds behavior with WPP Hosted Solution, when Order is partially invoiced
Fixed Hint for "View Details" in the Wishlist is located incorrectly
Fixed Onepage checkout - Shipping address issues
Fixed Tax Rate = 0% displayed in Cart
- display (0%) in rate title
Fixed Magento Backend performance optimization
Fixed Creating Purchase orders from backend works incorrect (IE)
Fixed Moving simple products (part of grouped) from shopping cart to order does not work
Fixed Payment Applicable From = "Specific Countries" option does not work for Express Checkout (Payflow Edition)
Fixed Cannot place Order in backend with Authorize.net Direct Post, when settings for payment method is applied on a Website scope level
Fixed SOAP don't use store for select products collection
- Change setting the store into filter
Fixed "Synchronize" button is disabled if select native database twice
- modified storage full name generation and button state check
Fixed Wrong algorithm to determine whether product can be configured (Composite Products feature)
- removed used method isComposite() from canConfigure() method
Fixed Missing nobr around date in Customer Product Reviews table
Fixed Status of Order, which is paced with Authorize.net Direct Post (Payment Action = Authorization) is incorrect
Fixed Added base_total_refunded field to invoice table
Fixed "Flush External Page Cache" does not work
Fixed Database as cache backend
Fixed Selecting products in Wishlist (backend) redirects you on dashboard
- Fixed searching by product names and days in wishlist
- Removed 'Visible In' column, because it showed same values as 'Added from'
- Fixed 'Added from' column to show real values, not some erroneous 'All Visible Stores'
- Fixed sorting by product name and days in wishlist
Fixed Only "Library Mail" works for USPS
Fixed The "MY WISHLIST" link always shows quantity of line items in the Wishlist and never the real quantity of items
- fix for case when out of stock products are not shown on frontend
Fixed Wrong behavior of Varien_Data_Collection_Db::_getConditionSql
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
- Rounding of shipment taxes was added
Fixed Impossible save empty values for store view scope
- Remove store_id from EAV module and move all store functionality into catalog module.
Fixed Wrong tax calculation for bundle products
Fixed File configuration dialog is not closed when pressing 'Ok' button
- additional fix of backend Customer functionality for IE8 to eliminate JS errors
Fixed Product creation -> Necessary validation for SKU field
Fixed Link "Gift Options" is not shown in Items Ordered grid of create Order page, when "Allow Gift Messages for Order Items" is set to "No"
- considering design html at right place
- removed useless variable from observer
Fixed Price for composite products in a products grid on Order creation page
Fixed Tax from orders in status pending presents in Tax Report
Fixed Catalog Price Rule is not applied
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed Order success page is not displayed after placing Order using Website Payments Pro Hosted Solution method
- now, return and cancel urls can be secure (https)
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Link "configure" is inactive for downloadable products in product grid on Order creation page in backend
Fixed A system error message is missing for cases when media storage synchronization is complete or an error occurred
- output messages for notifications edited
Fixed Incorrect price calculation for bundle product during backend order creation(Tax is doubles in Total)
Fixed Gift Options tab is present on product page for virtual product types
Fixed Magento Backend performance optimization
Fixed Gift Message for Individual Item prompt is shown in AJAX-popup, although "Allow Gift Messages for Order Items" is disabled
Fixed Unable to change customer password when email confirmation is enabled
Fixed Incorrect tax calculation for Tax Calculation Method Based On = Unit Price and Catalog Prices = Including Tax
Fixed "Preferred State" for extensions is not working
Fixed Total amount is not recounted, when customer cancels the Gift Options during OnePageCheckout
Fixed In "Gift options" AJAX popup "OK" button written incorrectly
Fixed No address autocomplete while admin order create with single store
- fixes due to unnecessary AJAX calls
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Gift column should be removed from product grid
Fixed SKU validation error on creating products
Fixed Shipped order has status "Processing" if invoice has been posted with "Not Capture" and amount was later captured on paypal side.
- considering online and offline capture amout when checking if capture is final
- trailing white spaces removed
Fixed Link to file from downloadable product is not available after authorize and capture payment action via Authorize.net
- Link management observer call methods are moved to save_commit_after events (for order and its item respectively) instead of save_after events
Fixed Price for product with file custom options in Wishlist is calculated incorrect
- Added ability to use special price templates for displaying wishlist items (as they can be partially/fully configured and catalog price template doesn't support it)
- Added default template, that shows configured price in addition to default clean product price
Fixed Cross-sells products disappears after adding another products to shopping cart
Fixed Price for composite products in a products grid on Order creation page
Fixed No ability to delete item from Wishlist by specifying Qty = 0 and click on Update Wishlist
Fixed Do not hide ajax loader on 'Place order' step on onepage checkout when customer selected PayflowLink payment method until PayPal iframe will be loaded
Fixed Admin reorder with bundle item cause wrong qty of simple products
Fixed Incorrect bundle product price and bundle items Qty count during the process of Admin Order creation
Fixed When bundle item is configured in that way, when it cannot have User defined quantity, Qty field remains editable in AJAX-popup
Fixed "UPS XML" allowed methods bug
Fixed Mage_Page_Block_Template_Links_Block::$_afterText is never used
Fixed No configuration popup for Grouped products in admin backend new order creation
- the problem was in sales.js during parsing currency from price cell. In case when no price was present in cell the JS exception occurs. So it was needed to determine currency symbol in other way. And it way was in sets this.currencySymbol in AdminOrder class when order obj initialization or when current currency  is switched.
- small fix in grouped.phtml and giftcatd.phtml: set additioal attributes for price calculation
- small fix in configure.js: using parameter listType instead of this.current.listType in _requestItemConfiguration method
- small fix in sales.js: do overall popup cleaning by productConfigure.clean() for each loadArea calling
Fixed When bundle item is configured in that way, when it cannot have User defined quantity, Qty field remains editable in AJAX-popup
Fixed Customer data not saved when returning to cart and back to checkout
Fixed Bad sku value for non-configured bundle in Create New Order at admin backend
Fixed Integrity Constraint Violation in Mage_Catalog_Model_Resource_Eav_Mysql4_Product_Indexer_Price::_prepareWebsiteDateTable
Fixed URL Rewrite Exeption
Fixed Menu "Catalog-Manage Products-Gift Options" have incorrect design and wrong position in menu list:
Fixed Displaying Out of Stock Products on the front-end.
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
Fixed Cannot login to backend while notify "This is a required field." is present
- There was JS error, invisible due to try-catch construction. Fixed
Fixed Authorize.net invoice capture.
- Do not capture/refund/void transaction if transaction has been captured/voided in authorize.net panel
Fixed Inadequate URL in Moneybookers eWallet "More Info" Link
Fixed It is impossible to export products using the new Export module
Fixed Tax Rate = 0% displayed in Cart
Fixed Unable to specify quantites for bundle items in AJAX-popup, when selection of bundle items is provided using radiobuttons
Fixed Incorrect style tables in customer confirmation email. For orders with Authorize.net payment method
- fixed incorrect styling in customer confirmation email;
- simplified styling on admin order page
Fixed Cron job dispatcher incorrectly releases locks
Fixed Incorrect items number in "MY WISHLIST" after updated quantity in the Wishlist
- Added new configuration option "Display Wishlist Summary" in System -> Configuration -> Customers -> Wishlist section
- Removed quantity information from wishlist frontend page
Fixed Update compare list after delete one item
Fixed No hint for disabled "Configure" button  
Fixed In Bundle product's page "Availability" string is not placed well
Fixed Non-correct headers uses for email return-path.
Fixed Numerous issued with displaying tax on front-end for bundled items
Fixed Impossible save empty values for store view scope
Fixed Non-correct headers uses for email return-path.  
- Added "-f" parameter to transport instance at Mage_Core_Model_Email_Template::send() like PHP mail() needs
Fixed Do not hide ajax loader on 'Place order' step on onepage checkout when customer selected PayflowLink payment method until PayPal iframe will be loaded
Fixed Order can be placed with non-configured composite product in Ordered Items
Fixed Using "Update Wishlist" adds quantity to existing value even nothing wasn't changed
Fixed Cannot open menu configuration-general-design
Fixed Added backend design exception model
Fixed The options in the action dropdown for export are incorrectly labeled in the Sales section
Fixed Checking if address exists was added before save addresses attributes (to prevent foreign key error in case of two users were logged in under one account in the same time).
Fixed URL rewrite algorithm was changed: fix for permanent link for old URLs.
Fixed Incorrect number of used card is shown after you have returned to 'Shopping Cart' in partial authorization (Authorize.Net)
Fixed In one page checkout incorrect information for declined card is shown for partial authorization(Authorize.Net)
Fixed Bundle products shoved without options
Fixed Instructions on the Payflow Link Configuration Menu
Fixed rate model checks rate to existence in rule before delete action
Fixed store name 'Demo Store' was changes to variable with real store name var store.getFrontendName()
Fixed Place order does not work with free shipping
Fixed possibility to find product in advanced search with from-to price is 0 was fixed
Fixed FPT with prices included tax problem
Fixed Instable work of back-end notification
- For now pop-up window doesn't go to our side. Flash availability check is removed
- little refactoring
- method Mage_AdminNotification_Helper_Data::isReadablePopupObject() marked as deprecated
Fixed Onepage checkout - Shipping address issues
- added resetting property to save billing address in address book
- added saving of new shipping address
- simplified condition in order preparation routine
Fixed Backordered Item Status on Orders
- saving current ordered items number for stock item and calculating backorder qty according to it
Fixed The product category is empty after moving category with products to another one
Fixed Magento Connect -> If substitute channel for package extension, MCM will send authorization data to the fake URL
Fixed Image Label is not Uploading properly
Fixed Category Tree -> Changing category color
Fixed With enabled "Inline Translation" its impossible to finish purchase
- Added checking for escaped html end tag
Fixed #0024559: Special Price to Date can not set Use Default Value
Fixed CMS -> Manage Pages: It's possible to save New Page with capital letters in URL key
- corrected js validation;
- added server-side url key validation.
Fixed Makeup of subcategories dropdown menu at front-end glitter with category fields bar
- removed property "z-index: 1" for #nav li.level-top
Revert changes from rev #83486
Fixed Tier prices are not recalculated in bundle product configuration with different currency
Fixed On Multi store installation, 'specials' rss feed includes specials from other stores
Fixed Subscribe to Order Status - translation problem
Fixed There is a spelling error with the translation
Fixed Single Coupon applying for each shipping location rather than whole order
- applying cart fixed rules for first shipping address order only
- store which quote address cart fixed rule was applied for in SalesRule_Model_Validator
Added method getDefaultCountry and constant XML_PATH_DEFAULT_COUNTRY into Mage_Core_Helper_Data
Added more abstract system config backend model for uploading files:
- removed duplicated logic from system config backend image model.
Fixed Grand total doubles when processing multi-shipping checkout and ordinary checkout
- cleaning address information when checkout type changes from multi-shipping to onepage
Fixed Problem with admin roles
Checkout page IE6/7 CSS bug fixed.
Fixed Edit product->"Inventory" tab - "Qty Increments" error contain mistake
Fixed No field for "Search Query"
Fixed Character "b" is added to Review
Fixed Retain the selected tab on editing CMS page
Fixed Invoices Tax class not displayed
Fixed Full tax summary on invoice
Fixed working with partial authorizations on first card submit
Fixed CMS can't create Hierarchy Node Link widget in IE8
Fixed The Wrong / not exist Url should be redirect to 404 page
Fixed Interface Locale needs additional country
Fixed The product category is empty after moving category with products to another one
Fixed 'Gateway error: A valid amount is required' appears during create Credit Memo for order, which uses Authorize.net
Fixed #19807: Product with visibility- Nowhere display on the fron-end in 'Last ordered items' block, if order create on back-end
Fixed Displaying Out of Stock Products on the front-end
- added price data for consider item stock status for wish-list and compare products items collections, in reorder for product collection which sales order item collection based on.
Fixed active tabs in store view scope while disabled PayPal methods
- Added functionality that disables corresponding methods in store view scope.
- Fixed related bug: in website view scope Express Checkout PE checkbox appears improperly checked after page load.
Fixed Active tabs in store view scope while disabled PayPal methods
Fixed Bundle price wrong when static qty above 1
Fixed No "Suspected Fraud" status for hacked orders
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
Fixed Don't show (-) in totals when shipping title and shiping method empty in a configuration
Fixed Product with price 0.00 possibility purchase through Shortcut PayPal button
Fixed Archived orders not displayed in customer's orders list
Fixed Fatal error on magento compilation
Fixed Mage::app() call is not overriding cache/var directories
Fixed After switching "Manage Stock" option, product prices index does not invalidate
Fixed Transfer Cart Line: dropdown with shipping Rates is absent on PayPal side
Fixed Can't choose Group at the creation new Order by admin
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
- added forgotten file from rev 84979
Fixed Bug in Error Message display for Send to Friend (Mage_Sendfriend_ProductController)
Fixed Admin order creation JS error message
Fixed Problems with category sort order
Fixed Button "Credit Memo" after refund partial per invoice is enabled
Fixed Report don't show order with status "Canceled"
Fixed Wrong quantity checks architecture in inventory observer
Fixed On page 404, link "go back" does not work
Fixed Category editing "Use Parent Category Settings" inconsistent behavior (Google Chrome)
Fixed Set products per Page
Fixed product review filter by customer does not work
- type is administrator when customer_id is NULL and store_id is admin store id
Fixed Product review filter by customer does not work
Fixed WYSIWYG Editor disabling issue
Fixed Quantity increment for Group Product Issue
Fixed #15780: Add configuration option to ignore SID on frontend
- Changed fieldset scope from global to website, because the field has website scope.
Fixed Message "The product has required options" appears twice in the back-end order for items with mandatory custom options
Fixed Meta description can be more than 255 chars
Fixed When creating a new customer from the backend in "Manage Customers", the welcome email is empty
Fixed  Image Label is not Uploading properly
- Slightly changed logic in adding image algorithms due to possible existence of added pictures
Fixed  JavaScript Calendar Date Range
- Also little fix to maintain corporate standards
Fixed Gift message displaying conditions not properly work on frontend and backend:
Fixed flat catalog tables do not contain varchar values for store view level
Fixed Add check "Use Default" for dependent form elements (in the admin), because if field "Use Default" it should be always disabled.
Fixed #21084: "can not" -> "cannot" text changes (found only one occurrence of "can not" and changed it)
Fixed New added required attribute should be filled in by customer before checkout
Fixed PayPal Billing Agreement presents in payment methods when no BA are created during admin order creation
Fixed Free Shipping Banner appears to be hard coded into the template file - replaced hardcoded callouts with CNS blocks. Two CMS blocks should be added to RR install.
Fixed Empty order status field
- Configuration mistake
Fixed Cart Rule discount with Fixed amount for a whole Cart is not applied for OnePageCheckout
Fixed Coupon with "Apply fixed amount discount for whole cart" does not apply to bundle products with dynamic price
Fixed Frontend additional attributes issue with price attributes.
Fixed Unable to translate "Submit Invoice" button
Fixed Undefined index after clicking on Print Shipment
Fixed Customer cannot be confirmed from the admin
Fixed Inline Translations don't work if you have more than one store
Fixed Invitation link has a session ID parameter
Fixed Magento creates order even if response from PaypalUk is empty
- response validation has been added
Fixed Displaying Out of Stock Products on the front-end
Fixed Incorrect billing/shipping address transfer from magento to PayPal (WPP Payflow Edition, WPP Payflow Edition EC )
Fixed User cannot be associated with webservice role if he was selected in the Role Users of Role inforamation Page
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- removed "beta" mark on CSS merger feature in system configuration, because known issue with different host names for different store views is solved
- split merged CSS storage into 2 parts: "css" and "css_secure"
- included "port" and "base host name" parameters into merger hash generation algorithm as parameters
Fixed: Default country setting not affect country select field default value on frontend 
Fixed Credit card data Iframe for PayflowLink is displayed on Order Review step for all payment methods
Fixed The Wrong / not exist  Url should be redirect to 404 page
- Added section availability in preDispatch
Fixed Report > Products Ordered ignores Store view switcher
- reforming $storeIds checks
Fixed Report > Products Ordered ignores Store view switcher
Fixed Cannot create or save after editing customer's Address, "Please enter the street" error appears on frontend
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Showing websites that only associated to current category or product.
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Fixed coding standards
Fixed Not all session data destroyed on logout
Fixed Inline Translation - Pages View Issue
- move cache types list in config
Fixed Shop By index range is build based on Excl. Tax value, but filter products in catalog based on Incl tax value. filter works incorrect
- it was problem with facets calculation, when we use Solr
Fixed Security issue - processing of disallowed actions with orders through direct URL
- wrong Credit Memo ACL resource name
Mage_Catalog_Model_Resource_Eav_Mysql4_Category_Flat
Fixed Different order amount in Google checkout and Magento orders
Fixed Bundle Product w/o required option calculates wrong fixed minimal price
Fixed Admin unable to uninstall payment method without editing config
- getMethodInstance method was rewrited
- Added instance check in some payment models according to this
Fixed lastInsertId invokes when no insert where proceed
Fixed Changing the root category for a store doesn't work correctly
Fixed Unable to translate notice messages, errors and success messages
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Tax of shipping method Flat Rate is not passed to the order while Google Checkout
Fixed Product Flat Data reindex
- disable flat data usage during reindex process
Fixed Catalog Rule does not work properly when condition uses Contains
Fixed Wrong prices (currency) for shipping price via UPS XML rates
Fixed Unable to translate product edit/create page
Fixed During product save operation, Magento disables keys for catalog_product_index_* tables.
Fixed FPT with prices included tax problem
- Added 'Catalog Prices' option check
Fixed Google Analytics e-commerce tracking not working
Fixed Empty bundle selections are shown as item options
Fixed Subtotal for Bundle product with quantity 2 calculates as for one
Fixed Remove initSessionLayoutMessages() from ProductController
Fixed Incorrect value of field "Custom Layout Update" causes fatal error
Fixed Duplicate of a product creates it with no SKU value and is saved
Fixed Field "Meta Description" should be has limit of 255 characters
Fixed Row subtotal is not displayed for Downloadable product in Backend
Fixed Bad styling of product options displayed in wishlist
Fixed Need to show item options of customer shopping cart at backend
Fixed Wishlist item configuration is not saved at backend
Fixed "OK" button instead of "Ok" must be on product configuration popups in backend
Fixed Products wishlist items are not sorted by added_at
Fixed Mage_Core_Model_Template doesn't properly restore old design context
Fixed StoreView value not in FlatCatalog for multiple-select type attribute
Fixed Rule condition "is one of" disappeared for category_ids attribute
- Added "is one of" and "is not one of" to multiselect type conditions
Fixed Security issue - the way to get URL-path of Admin side through Front-end URL
Fixed Pictures does not appears on the additional information tab on front end for product attribute with Catalog Input Type for Store Owner= Text Area
Fixed Add method which was accidentally removed
- Deprecated methods Mage_Catalog_Model_Product::loadParentProductIds, Mage_Catalog_Model_Resource_Eav_Mysql4_Product::getParentProductIds
Fixed Can't create refund online for Google Chekout
Fixed After pressing 'Cancel Payment' link nothing happens in Payflow Link payment method
Fixed class Mage_Core_Model_Store has problem with _processConfigValue and processSubst
- Added "@deprecated after 1.4.2.0" mark for processSubst() in Mage_Core_Model_Store
Fixed Category tree is missing for product, assigned to root category
Fixed Unable to translate "Delete Image" checkbox
Fixed wrong XML paths in isAllowed() method for system->Admin roles controllers.
Fixed Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
- Changed exception message
Fixed Different shipping amount for creditmemo from order page and invoice page
Fixed Tax rates with zip ranges doesn't match to addresses with asterisk ( * ) as zip code value
Fixed Fedex doesn't react to overrided in website scope BaseCurrency value.
Fixed Export Customers. Map billing or shipping street in the mapping interface. They won't be exported
Fixed Advanced Import Profiles doesn't work
Fixed Add New Customer Form: checkbox "Send Welcome Email" is not disabled if "Associate to Website"="Admin"
Fixed JS validation prevent submit form
Fixed Payment action: Ogone Default Operation is not working at all
Fixed There are no ability to create several Refunds to Order completed using Partial Authorization
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
Fixed URL key wasn't used while product save
Fixed Inline Translations don't work if you have more than one store
Fixed Tax Report Shows Wrong Tax Percent After Changing Tax Rate
- added grouping by tax percent in report collections
- modified unique key in the tax report aggregation table to allow generating report with grouping by tax percents
- data in the tax report aggregation table is truncated and lifetime statistics must be re-generated after upgrade
Fixed make increment_id fields unique in sales tables
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Orders: More than one filter to the same field is not possible
- Function items was changed.
Fixed Invoices: More than one filter to the same field is not possible
- Function items was changed.
Fixed Report counts configurable products twice
Fixed Tax rate with ZIP XXXXX* doesn't match to customer zip XXXXX
Fixed Method Mage_Wishlist_Block_Links::addWishlistLink removed
- Added "@deprecated after 1.4.2.0"
Fixed "Subscribed to Newsletter" success e-mail couldn't be sent if you changed customer's subscription in admin.
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Dashboard reports bug
- Added discount to Mage_Reports_Model_Mysql4_Order_Collection:::addSumAvgTotals()
Fixed Google base timeout
- Timeout is 60 seconds now.
Fixed Bundle product is not shipped correctly
Fixed Unable to translate product edit/create page
Fixed Dataflow customers export optimization
- customer groups are storing in memory instead of DB queries
Fixed Price layer navigation does not count product with zero price
Fixed Import Product doesn't work
- added empty file checking
Fixed Price Indexer does not apply configurable options surcharges for customer groups different to "NOT LOGGED IN"
Fixed Category Update Not Reflected in Left Nav
Fixed Notify Stock RSS Includes Products without stock
Fixed FPT is not shown in the order review page (for website)
Fixed SQL Upgrades have wrong implementation
Fixed Email to a friend error, existing Order Send Email error
- Added ability to access to /admin/sales_order/email/ action
Fixed Total Refunded Report shows Offline Refunded orders like Online Refunded
Fixed UPS XML Shipping method doesn't work, if country of shipping origin is not USA
- Added Mage::log() for errors @ Mage_Usa_Model_Shipping_Carrier_Ups::_parseXmlResponse()

==== 1.5.0.0-rc2 =====

== Changes ==
Paypal HSS payment method label, comment and default title

== Fixes ==
Fixed User cannot place order using Paypal payment methods with 3d secure
Fixed iPhone product list preview
Fixed App locations (countries) do not match iTunes App Stores countries available
Fixed Added parent quote items to discount calculation to prevent skipping of configurable products.
Fixed Rounding issue on front end if discount with fixed amount is applied and no tax rules applies to the order.
- added rounding item discount before take away from total discount
Fixed Fatal error after deleting one of the shipping addresses during checkout with multiple addresses
Fixed Merged CSS files with selected native Database as media storage are not applied with Chrome and FF
- first trying to detect MIME type manually, and only after by native php function
Fixed The buttons "Accept Payment" and "Deny Payment" do not appear in orders with status 'Payment Review'
Fixed issue when Simple products not visible individually (part of grouped) are moved to Wishlist
Fixed Impossible to delete product from Items Ordered (backend Order creation) using "remove" in Action dropdown
Fixed Fatal error after deleting one of the shipping addresses during checkout with multiple addresses
Fixed Qty for simple products (part of grouped) is incorrect when moved from order to Wishlist
- additional fixture for other testcase
Fixed Grouped product is added to Items Ordered as grouped, when any of buttons in sideblocks is pressed after product configuration in a product grid (backend Order creation)
- prevent to add unconfigured grouped product on server side
- in sales.js, do productConfigure.clean('quote_items') only if "Items Ordered" block is going to update
- in sales.js, hide "Search" block only when product added to qoute from "Search" block
- in configure.js, added ability to cleaning by list type scope
Fixed Incorrect behavior of Partial Authorization process, when admin user cancels authorizations (Authorize.net)
- added reloading block 'totals' after canceling partial authorization
Fixed Google Checkout Issue - Transactions not appearing
- adding transaction (transaction id = google order id) for googlecheckout payment
- fixed usage of Mage_GoogleCheckout_Model_Api_Xml_Callback::_getTaxClassForShipping() method according to it's interface
- fixed usage of Mage_GoogleCheckout_Model_Api_Xml_Abstract::_getTaxClassForShipping() method according to it's interface
- creating transactions for refund and chargeback

==== 1.5.0.0-rc1 =====

=== Fixes ===
Fixed Missed index on sales.order table
Fixed Price for composite products in a products grid on Order creation page
Fixed Status of Order is now doesn't ignore the setting in Config for AUTH_AND_CAPTURE orders.
Fixed Unable to install extension using MCM for CE
Fixed Rounding error
Fixed Preview iFrame of iPhone recieve error message
- wrap images manipulations with try-catch (in controller)
- alert the catched error message when preview is loaded
Fixed Most product attibutes not exporting
Fixed Removed error message on new orders payd by PayflowLink with "complete" status (like on virtual products)
Fixed Behavior when customer changes billing/shipping address and/or changes items in cart, etc having started Partial Authorization
- added chopping cart`s and address checksum checking for partial authorization process
Fixed Moving composite products from shopping cart to wishlist does not work
- fixed error handling - added catching and processing, so in case of errors only item with error will not be moved
- fixed wishlist items to get right storeId (by passing product, and not productId)
Fixed Rounding issue (1 cent) appears on Tax Calculation Method Based On = Row
Fixed category/product image resizing
- Image sizes for Ipad has been changed
- Re-Factored: Application model call has been changed to helper method for all old calls
Fixed Only check money payment at standard chechout process receive success
Fixed Edit fonts configuration for iPad
Added iPad preview should illustrate tabs' state.
- Made separate icons
- Active/inactive logic added
- Added custom fonts for rating color customization
- Fixed positions for the icons
- Removed icons labels
- "i"-icon should always be on screen (currently it becomes hidden after making "information"-tab inactive)
Fixed Review collection need to sort with the latest added review
Fixed XML Connect - Incorrect help link in Push Notification page
Fixed API Certificate Based Authentication Used default signature value insted of the Certificate value
Fixed XML Connect - Design page - Ipad backgrounds issue
Fixed "Ship to different address" is not applied with IE8 with any payment method
Fixed Added skipping delta in shipping calculation on free shipping
Fixed Incorrect behavior of Gift Options popup for bundle product on backend Order View page. No ability to close popup
Fixed Rounding issue (1 cent) appears on discount applied and Tax Calculation Method Based On = Row
Fixed Add landscape mode background for Android and update information for portrait mode background
- changed <backgroundImageAndroid> to <backgroundAndroidPortraitImage>,
- changed all <someimagetagImageDeviceOrientatin> to <someimagetagDeviceOrientatinImage> for correctly image resizings,
- same for Icon,
- added orientation divisions for Android devices,
- fixed wrong spelled word "Portret" onto "Portrait" for iPad's config tags
- Image resize method has been changed
- backround getter method fixed
Fixed Tax rates export doesn't work
Fixed Incorrect downloader version in footer
Changed default title for HSS payment method
Fixed Rounding issue on credit memos/invoices cousing different totals in magento and 1 cent error on paypal
- added adjustment for invoice`s subtotal_incl_tax and base_subtotal_incl_tax if invoice is last invoice of order
Fixed Added setting of store id in payment method instance on Authorize.net partial authorization cancel from admin place.
Fixed Fix Android preview area
- Added custom fonts
- Fixed header icons borders
- Fixed button border on homepage
- Added custom color declaration
Fixed Tabs dont affect second preview screen for Android mobile application
Fixed Incorrect design for Android mobile application in IE8
Added update Preview Area for iPad
- Fixed incorrect design for Ipad mobile application in IE8
- added stars custom fonts for landscape mode
- Fixed wrong positioning of the icons in landscape mode
Fixed Double use Authorize.net Partial Authorization Multicard with 46225 zip in one order causes wrong checkout behavior
Fixed Using MCM 2.0 shell script produces warnings and doesn't work correctly

==== 1.5.0.0-beta2 =====

=== Improvements ===
Implemented Environment emulation in core email class
- Added Emulation model.
- Added Email Info and Email Template Mailer models.
- Re-factored sendEmail() and sendUpdateEmail() methods of order, credit memo, invoice and shipment models.
Added App Previewer for Android and iPad in XmlConenect

=== Fixes ===
Fixed Labels for composite products (backend) are shown incorrect
Fixed Ability to Refund the already refunded item in Patial Invoice
- added qty`s limits into creating creditmemo functionality
Fixed Performance issue with big amount of tax rates
Fixed Notice error in system.xml after saving PayPal configuration
Fixed No Qty column in the Wishlist sideblock
Fixed Export functionality doesn't work
Fixed Maestro International CC number has no validation
- use "Switch/Maestro" instead of "Maestro (International)"
Fixed No transactions is created, no ability to perform Invoice, when Order, which contains Gift Options, is placed from backend with Authorize.net Direct Post payment method
Fixed Moving Grouped product from Order and Shopping cart to the Wishlist does not work
Fixed Added advice block hiding on synchronize process
Fixed Database as cache backend
- fix for MySQL 4. Shorten field lengthes
Fixed Improvemets for MCM and Magento Extension Packager after MCMUP
Fixed PayPal Standard with specific tax settings for shop cart item with qty >= 2
Fixed Wrong tax calculation for bundle products
Fixed Export Filters are not working correctly during export of customers
Fixed Unable to complete several partial online refunds with Authorize.net Direct Post
Fixed Disable Mage_Checkout did not remove My Cart & Checkout links in the Top Link
Fixed An error occurs with using Payflo Link payment method and IE8
- just small fixture of strange for user popup in IE - "Do you want to see only secure content?"
Fixed Price for composite products in a products grid on Order creation page
Fixed No error message appears if execute synchronization with non-existing DB
Fixed "Configure" link in Product grid (backend) does not work (only IE)
Fixed "Void" button must not be active on the invoice with amount captured on-line
- redefined methods canVoid for Express and Direct Paypal models - hiding button void for invoice and creditmemo
- redefined methods cancel for Express and Direct Paypal models - no checking for invoices for order to decide void it or not at cancel.
Fixed Dropdown for Amount is absent (only IE)
- create new JS method that preserves visibility states of selects in pop-up block
Fixed Status of Order is now doesn't ignore the setting in Config.
Fixed Incorrect behavior of AJAX-popup for Gift Options (Individual Item) in IE8
Fixed to show full review for the iPad device
- added checking the current app's device type is not iPad and in this case the text of the review is truncated;
- replaced TABs on spaces in helper's class
- Re-factored XmlConnect helperfor unknown device type
Fixed xmlconnect/catalog/product action returns invalid html for product's description
- added an "xml" tag before DOCTYPE definition
Fixed wrong using of translation in method getElementHtml()
Fixed update Preview Area for iPad
Fixed Missed active/Inactive tabs logic added for a preview
Fixed Selecting catalog as a price rule condition redirects you on dashboard
- check if post array values are integers > 0
Fixed "Go to notifications" link works improperly
Fixed Unable to complete several partial online refunds with Authorize.net Direct Post
Fixed "Set Products as New to Date" is not working in Catalog New Products List widget
Fixed Mage_Adminhtml_Block_Media_Uploader::getUploaderUrl() generates incorrect path if magento is installed in a sub-directory within the root one
Fixed Now in Admin in System->TransactionalEmails all filters are saved to session.
Fixed Tax discrepancy between Tax Report and Order Report
Fixed PayPal Standard with specific tax settings for shop cart item with qty >= 2
Fixed Incorrect hint for non-configured product in Order on backend
Fixed Flush Cache Storage alert text is now changed to: "Cache storage may contain additional data. Are you sure that you want flush it?"
Fixed "Read Details" link is present in the message about synchronization status
- removed read details link from rows which have not url
Fixed Mage_Catalog_Model_Product::setFinalPrice() doesn't return its class instance for chaining purposes.
- fixed interface erroneously changed in 1.4.1.0
- fixed erroneous phpDoc
Fixed First Checkout by registered Customer: First Name and Last name fields are empty
Fixed Error with addlisttype.phtml in system log
- Removed not deleted layout block that was forgotten after rev 90337 with fix for MAGE-1955
Fixed Changes in UI for Order Status Management
Fixed Catalog Price Rule is not applied
- Added Mage_CatalogRule_Model_Rule::applyAllRulesToProduct()
Fixed Admin order creation - Unable to delete product from the cart
- fixed showing giftmessage options template, when no grid items are present
- fixed updating quote items and giftmessage items when backend receives wrong item id - now it doesn't fail with exception, but process it gracefully
Fixed With IE6 impossible to configure a Composite product in Backend
Fixed Message for non-configured composite product is changed after pressing "Update Items and Qty's"
Fixed Option "Order" on Payment Action dropdown must be available only for Express Checkout method
- Removed extra spaces in system.xml.
Fixed With IE8 an error occurs after applying the second time Credit Card in Admin panel with 3D Secure and patrial authorization (Authorize.net)
- moved embedded gift options FORM tag out of other main FORM tag (such invalid layout broke DOM in IE)
- refactored JS-scripts, moved static to static files
- removed not used old js-file
Fixed Products are erased from "Product Ordered" report after deleting them
Fixed Incorrect behavior of ReOrder action applied to Order, that contains Gift Options
Fixed When adding several configurable products at one time to Items Ordered from product grid, only last remains specified configuration (admin Order creation)
- restored JS-initing for controls on each popup show (was erroneously removed at rev 86017)
- fixed Configurable javascript so it won't interfere with other products controls on page
Fixed Incorrect transaction and Partial Refunds behavior with WPP Hosted Solution, when Order is partially invoiced
Fixed Hint for "View Details" in the Wishlist is located incorrectly
Fixed Onepage checkout - Shipping address issues
Fixed Tax Rate = 0% displayed in Cart
- display (0%) in rate title
Fixed Magento Backend performance optimization
Fixed Creating Purchase orders from backend works incorrect (IE)
Fixed Moving simple products (part of grouped) from shopping cart to order does not work
Fixed Payment Applicable From = "Specific Countries" option does not work for Express Checkout (Payflow Edition)
Fixed Cannot place Order in backend with Authorize.net Direct Post, when settings for payment method is applied on a Website scope level
Fixed SOAP don't use store for select products collection
- Change setting the store into filter
Fixed "Synchronize" button is disabled if select native database twice
- modified storage full name generation and button state check
Fixed Wrong algorithm to determine whether product can be configured (Composite Products feature)
- removed used method isComposite() from canConfigure() method
Fixed Missing nobr around date in Customer Product Reviews table
Fixed Status of Order, which is paced with Authorize.net Direct Post (Payment Action = Authorization) is incorrect
Fixed Added base_total_refunded field to invoice table
Fixed "Flush External Page Cache" does not work
Fixed Database as cache backend
Fixed Selecting products in Wishlist (backend) redirects you on dashboard
- Fixed searching by product names and days in wishlist
- Removed 'Visible In' column, because it showed same values as 'Added from'
- Fixed 'Added from' column to show real values, not some erroneous 'All Visible Stores'
- Fixed sorting by product name and days in wishlist


==== 1.5.x-devel-92027 ====

=== Fixes ===
Fixed Selecting catalog as a price rule condition redirects you on dashboard
- check if post array values are integers > 0
Fixed "Go to notifications" link works improperly
Fixed Unable to complete several partial online refunds with Authorize.net Direct Post
Fixed "Set Products as New to Date" is not working in Catalog New Products List widget
Fixed Mage_Adminhtml_Block_Media_Uploader::getUploaderUrl() generates incorrect path if magento is installed in a sub-directory within the root one
Fixed Now in Admin in System->TransactionalEmails all filters are saved to session.
Fixed Tax discrepancy between Tax Report and Order Report
Fixed PayPal Standard with specific tax settings for shop cart item with qty >= 2
Fixed Incorrect hint for non-configured product in Order on backend
Fixed Flush Cache Storage alert text is now changed to: "Cache storage may contain additional data. Are you sure that you want flush it?"
Fixed "Read Details" link is present in the message about synchronization status
- removed read details link from rows which have not url
Fixed Mage_Catalog_Model_Product::setFinalPrice() doesn't return its class instance for chaining purposes.
- fixed interface erroneously changed in 1.4.1.0
- fixed erroneous phpDoc
Fixed First Checkout by registered Customer: First Name and Last name fields are empty
CR Change First Checkout by registered Customer: First Name and Last name fields are empty
- reverted Billing.php to the its previous state
- copied logic of determine customer name from customer address template  base/default/template/customer/address/edit.phtml
Fixed CRIT error with addlisttype.phtml in system log
- Removed not deleted layout block that was forgotten after rev 90337 with fix for MAGE-1955
Fixed Changes in UI for Order Status Management
Fixed Catalog Price Rule is not applied
- Added Mage_CatalogRule_Model_Rule::applyAllRulesToProduct()
Fixed Admin order creation - Unable to delete product from the cart
- fixed showing giftmessage options template, when no grid items are present
- fixed updating quote items and giftmessage items when backend receives wrong item id - now it doesn't fail with exception, but process it gracefully
Fixed With IE6 impossible to configure a Composite product in Backend
Fixed Message for non-configured composite product is changed after pressing "Update Items and Qty's"
Fixed Option "Order" on Payment Action dropdown must be available only for Express Checkout method
- Removed extra spaces in system.xml.
Fixed With IE8 an error occurs after applying the second time Credit Card in Admin panel with 3D Secure and patrial authorization (Authorize.net)
- moved embedded gift options FORM tag out of other main FORM tag (such invalid layout broke DOM in IE)
- refactored JS-scripts, moved static to static files
- removed not used old js-file
Fixed Products are erased from "Product Ordered" report after deleting them
Fixed Incorrect behavior of ReOrder action applied to Order, that contains Gift Options
Fixed When adding several configurable products at one time to Items Ordered from product grid, only last remains specified configuration (admin Order creation)
- restored JS-initing for controls on each popup show (was erroneously removed at rev 86017)
- fixed Configurable javascript so it won't interfere with other products controls on page
Fixed Incorrect transaction and Partial Refunds behavior with WPP Hosted Solution, when Order is partially invoiced
Fixed Hint for "View Details" in the Wishlist is located incorrectly
Fixed Onepage checkout - Shipping address issues
Fixed Tax Rate = 0% displayed in Cart
- display (0%) in rate title
Fixed Magento Backend performance optimization
Fixed Creating Purchase orders from backend works incorrect (IE)
Fixed Moving simple products (part of grouped) from shopping cart to order does not work
Fixed Payment Applicable From = "Specific Countries" option does not work for Express Checkout (Payflow Edition)
Fixed Cannot place Order in backend with Authorize.net Direct Post, when settings for payment method is applied on a Website scope level
Fixed SOAP don't use store for select products collection
- Change setting the store into filter
Fixed "Synchronize" button is disabled if select native database twice
- modified storage full name generation and button state check
Fixed Wrong algorithm to determine whether product can be configured (Composite Products feature)
- removed used method isComposite() from canConfigure() method
Fixed Missing nobr around date in Customer Product Reviews table
Fixed Status of Order, which is paced with Authorize.net Direct Post (Payment Action = Authorization) is incorrect
Fixed Added base_total_refunded field to invoice table
Fixed "Flush External Page Cache" does not work
Fixed Database as cache backend
Fixed Selecting products in Wishlist (backend) redirects you on dashboard
- Fixed searching by product names and days in wishlist
- Removed 'Visible In' column, because it showed same values as 'Added from'
- Fixed 'Added from' column to show real values, not some erroneous 'All Visible Stores'
- Fixed sorting by product name and days in wishlist


==== 1.5.0.0-beta1 =====

=== Improvements ===
Fixed several memory leaks in product model. Added tool method clear() to clean object data and references to this object
Implemented Order payment action for PayPal
Implemented SOAP Api calls for shopping cart

=== Fixes ===
Fixed Only "Library Mail" works for USPS
Fixed The "MY WISHLIST" link always shows quantity of line items in the Wishlist and never the real quantity of items
- fix for case when out of stock products are not shown on frontend
Fixed Wrong behavior of Varien_Data_Collection_Db::_getConditionSql
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
- Rounding of shipment taxes was added
Fixed Impossible save empty values for store view scope
- Remove store_id from EAV module and move all store functionality into catalog module.
Fixed Wrong tax calculation for bundle products
Fixed File configuration dialog is not closed when pressing 'Ok' button
- additional fix of backend Customer functionality for IE8 to eliminate JS errors
Fixed Product creation -> Necessary validation for SKU field
Fixed Link "Gift Options" is not shown in Items Ordered grid of create Order page, when "Allow Gift Messages for Order Items" is set to "No"
- considering design html at right place
- removed useless variable from observer
Fixed Price for composite products in a products grid on Order creation page
Fixed Tax from orders in status pending presents in Tax Report
Fixed Catalog Price Rule is not applied
Fixed Incorrect tax summary for partial credit memos/invoices
Fixed Order success page is not displayed after placing Order using Website Payments Pro Hosted Solution method
- now, return and cancel urls can be secure (https)
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Link "configure" is inactive for downloadable products in product grid on Order creation page in backend
- also fixed "Manage Customer" grids + Manage Shopping Cart (Enterprise Checkout) grids
Fixed A system error message is missing for cases when media storage synchronization is complete or an error occurred
- output messages for notifications edited
Fixed Incorrect price calculation for bundle product during backend order creation(Tax is doubles in Total)
Fixed Gift Options tab is present on product page for virtual product types
Fixed Magento Backend performance optimization
Fixed Gift Message for Individual Item prompt is shown in AJAX-popup, although "Allow Gift Messages for Order Items" is disabled
Fixed Unable to change customer password when email confirmation is enabled
Fixed Incorrect tax calculation for Tax Calculation Method Based On = Unit Price and Catalog Prices = Including Tax
Fixed "Preferred State" for extensions is not working
Fixed Total amount is not recounted, when customer cancels the Gift Options during OnePageCheckout
Fixed In "Gift options" AJAX popup "OK" button written incorrectly
Fixed No address autocomplete while admin order create with single store
- fixes due to unnecessary AJAX calls
Fixed Information about Gift Options is not stored, when admin user performs Edit Order action in backend
Fixed Gift column should be removed from product grid
Fixed SKU validation error on creating products
Fixed Shipped order has status "Processing" if invoice has been posted with "Not Capture" and amount was later captured on paypal side.
- considering online and offline capture amout when checking if capture is final
- trailing white spaces removed
Fixed Link to file from downloadable product is not available after authorize and capture payment action via Authorize.net
- Link management observer call methods are moved to save_commit_after events (for order and its item respectively) instead of save_after events
Fixed Price for product with file custom options in Wishlist is calculated incorrect
- Added ability to use special price templates for displaying wishlist items (as they can be partially/fully configured and catalog price template doesn't support it)
- Added default template, that shows configured price in addition to default clean product price
Fixed Cross-sells products disappears after adding another products to shopping cart


==== 1.5.x-devel-90295 ====

=== Fixes ===
Fixed Configurable Product:Associated Product tab - Rounding issue
Fixed Wrong usage of @see tag in phpdocs
- replaced @see into @link phpdocs in cases where the value is a link
Fixed A system error message is missing for cases when media storage synchronization is complete or an error occurred
Fixed Order success page is not displayed after placing Order using Website Payments Pro Hosted Solution method
Fixed Order contains information about used card type with Payflow Link (for USA and Canada) payment using
Fixed Product export have no Entity Attributes
Fixed Authorize.net Directpost payment method doesn't work when secure urls in frontend are being used
Fixed The options in the action dropdown for export are incorrectly labeled in the Sales section
- Rename XML and MSXML to Excel XML
Fixed Round up to 0.01 of amount with tax in cart
Fixed Shipped order has status "Processing" if invoice has been posted with "Not Capture" and amount was later captured on paypal side.
- Return invoice model for transaction, if it didn't return by transaction_id
Fixed File configuration dialog is not closed when pressing 'Ok' button
- also made better logic to disable/enable file controls, so that file is not uploaded (and just thrown away by server) when there's no need in it
Fixed Deleting attached files do not work
Fixed Price for composite products in a products grid on Order creation page
- it was also fixed converting to current currency rates
Fixed Firefox iframe issue
Fixed Can not add product to order from backend (IE8)
Fixed Moving product with file custom options to Wishlist works incorrect
Fixed Displaying Out of Stock Products on the front-end
Fixed Price for composite products in a products grid on Order creation page
- forgot to add parent::_afterLoad(); in Mage_Bundle_Model_Mysql4_Selection_Collection::_afterLoad() method witch leads to exception
Fixed Fix for HSS amount is sent to PayPal. But need to test includeTax/excludeTax settings.
Fixed A system error message is missing for cases when media storage synchronization is complete or an error occurred
- fixed ability to save storage witch last sync was made on
- removed link "read details" for local messages at notice bar
- messages correction
Fixed Authorize.net Directpost payment method. Can't create capture and refund transaction


=== 1.5.0.0-alpha2 ====

=== Major Highlights ===
Added Payflow Link using HSS (Hosted Sole Solution)

=== Improvements ===
Upgraded Zend Framework to 1.11.1
Phoenix_Moneybookers improvements:
- updated payment logo images
- added "Maestro" and "Online Bank Transfer" payment methods into Moneybookers group
- wrapped Moneybookers payment logo title and alt text on payment selection text into translation calls

=== Fixes ===
Fixed Price for composite products in a products grid on Order creation page
Fixed No ability to delete item from Wishlist by specifying Qty = 0 and click on Update Wishlist
Fixed Do not hide ajax loader on 'Place order' step on onepage checkout when customer selected PayflowLink payment method until PayPal iframe will be loaded
Fixed Admin reorder with bundle item cause wrong qty of simple products
Fixed Incorrect bundle product price and bundle items Qty count during the process of Admin Order creation
Fixed When bundle item is configured in that way, when it cannot have User defined quantity, Qty field remains editable in AJAX-popup
Fixed "UPS XML" allowed methods bug
Fixed Mage_Page_Block_Template_Links_Block::$_afterText is never used
Fixed No configuration popup for Grouped products in admin backend new order creation
- the problem was in sales.js during parsing currency from price cell. In case when no price was present in cell the JS exeption occurs. So it was needed to determine currency symbol in other way. And it way was in sets this.currencySymbol in AdminOrder class when order obj initialization or when current currency  is switched.
- small fix in grouped.phtml and giftcatd.phtml: set additioal attributes for price calculation
- small fix in configure.js: using parameter listType instead of this.current.listType in _requestItemConfiguration method
- small fix in sales.js: do overall popup cleaning by productConfigure.clean() for each loadArea calling
Fixed When bundle item is configured in that way, when it cannot have User defined quantity, Qty field remains editable in AJAX-popup
Fixed Customer data not saved when returning to cart and back to checkout
Fixed Bad sku value for non-configured bundle in Create New Order at admin backend
Fixed Integrity Constraint Violation in Mage_Catalog_Model_Resource_Eav_Mysql4_Product_Indexer_Price::_prepareWebsiteDateTable
Fixed URL Rewrite Exeption
Fixed Menu "Catalog-Manage Products-Gift Options" have incorrect design and wrong position in menu list:
Fixed Displaying Out of Stock Products on the front-end.
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
Fixed Cannot login to backend while notify "This is a required field." is present
- There was JS error, invisible due to try-catch construction. Fixed
Fixed Authorize.net invoice capture.
- Do not capture/refund/void transaction if transaction has been captured/voided in authorize.net panel
Fixed Inadequate URL in Moneybookers eWallet "More Info" Link
Fixed It is impossible to export products using the new Export module
Fixed Tax Rate = 0% displayed in Cart
Fixed Unable to specify quantites for bundle items in AJAX-popup, when selection of bundle items is provided using radiobuttons
Fixed Incorrect style tables in customer confirmation email. For orders with Authorize.net payment method
- fixed incorrect styling in customer confirmation email;
- simplified styling on admin order page
Fixed Cron job dispatcher incorrectly releases locks
Fixed Incorrect items number in "MY WISHLIST" after updated quantity in the Wishlist
- Added new configuration option "Display Wishlist Summary" in System -> Configuration -> Customers -> Wishlist section
- Removed quantity information from wishlist frontend page
Fixed Update compare list after delete one item
Fixed No hint for disabled "Configure" button  
Fixed In Bundle product's page "Availability" string is not placed well
Fixed Non-correct headers uses for email return-path.
Fixed Numerous issued with displaying tax on front-end for bundled items
Fixed Impossible save empty values for store view scope
Fixed Non-correct headers uses for email return-path.  
- Added "-f" parameter to transport instance at Mage_Core_Model_Email_Template::send() like PHP mail() needs
Fixed Do not hide ajax loader on 'Place order' step on onepage checkout when customer selected PayflowLink payment method until PayPal iframe will be loaded
Fixed Order can be placed with non-configured composite product in Ordered Items
Fixed Using "Update Wishlist" adds quantity to existing value even nothing wasn't changed


==== 1.5.x-devel-89318 ====

=== Fixes ===
Fixed Tax Rate = 0% displayed in Cart
Fixed Unable to specify quantites for bundle items in AJAX-popup, when selection of bundle items is provided using radiobuttons
Fixed Incorrect style tables in customer confirmation email. For orders with Authorize.net payment method
- fixed incorrect styling in customer confirmation email;
- simplified styling on admin order page
Fixed Cron job dispatcher incorrectly releases locks
Fixed Incorrect items number in "MY WISHLIST" after updated quantity in the Wishlist
- Added new configuration option "Display Wishlist Summary" in System -> Configuration -> Customers -> Wishlist section
- Removed quantity information from wishlist frontend page
Fixed Update compare list after delete one item
Fixed No hint for disabled "Configure" button  
Fixed In Bundle product's page "Availability" string is not placed well
Fixed Non-correct headers uses for email return-path.
Fixed Numerous issued with displaying tax on front-end for bundled items
Fixed Impossible save empty values for store view scope
Fixed Non-correct headers uses for email return-path.  
- Added "-f" parameter to transport instance at Mage_Core_Model_Email_Template::send() like PHP mail() needs
Fixed Do not hide ajax loader on 'Place order' step on onepage checkout when customer selected PayflowLink payment method until PayPal iframe will be loaded
Fixed Order can be placed with non-configured composite product in Ordered Items
Fixed Using "Update Wishlist" adds quantity to existing value even nothing wasn't changed

==== 1.5.0.0-alpha1 ====

=== Major Highlights ===
Balance Response, Partial Authorization Transactions, Authorization Reversals Support for MasterCard and Discover
3D Secure authentication for Authorize.net payment method
PayflowLink payment method
Authorize.Net SIM payment method
Improved Import/Export functionality
Ability to order composite products from backend and some extra functionality
- reconfigure already added products on front end
- adding preconfigured products in wish-list
Alternative media storage
- Database
- CDN
Order status management
- ability to add new status and assign to some state
- from now on statuses stored in appropriate DB table instead of configuration file
Ability to edit order addresses
- this functionality admin has link to edit address for order view page
Magento Mobile included in base packaging

=== Improvements ===
Upgraded Zend Framework to 1.11.0
Implemented new process of hashing parameters in Ogone payment method
- implemented an advanced hashing method that invokes all transaction parameters for building security hash
- updated fields sort order in system configuration
- added the new parameter which designates whether to use the old or advanced hashing method
- made SHA-IN and SHA-OUT sys config parameter titles corresponding to parameter titles on merchant site in Ogone
- major refactoring of the Ogone helper: simplified public interface of hash validation, added support for SHA-1, SHA-256 and SHA-512 algorithms (not selectable in system config)
- optimized performance of debugging and building redirect form: removed 2 excessive calls (one from template, another from debugging - it invoked form building even if debugging was disabled)
- since the form is built from a block, prevented injecting SID parameter to URLs when building form
- added HTML escaping in the template hidden fields
- added new system configuration parameter - hashing algorithm
- verified/fixed all API hashing parameters in accordance to documentation v.5.0

=== Fixes ===
Fixed Cannot open menu configuration-general-design
Fixed Added backend design exception model
Fixed The options in the action dropdown for export are incorrectly labeled in the Sales section
Fixed Checking if address exists was added before save address'es attributes (to prevent foreign key error in case of two users were logged in under one account in the same time).
Fixed URL rewrite algorithm was changed: fix for permanent link for old URLs.
Fixed Incorrect number of used card is shown after you have returned to 'Shopping Cart' in partial authorization (Authorize.Net)
Fixed In one page checkout incorrect information for declined card is shown for partial authorization(Authorize.Net)
Fixed Bundle products shoved without options
Fixed Instructions on the Payflow Link Configuration Menu
Fixed rate model checks rate to existens in rule before delete action
Fixed store name 'Demo Store' was changes to variable with real store name var store.getFrontendName()
Fixed Place order does not work with free shipping
Fixed possibility to find product in advanced search with from-to price is 0 was fixed
Fixed FPT with prices included tax problem
Fixed Instable work of back-end notification
- For now pop-up window doesn't go to our side. Flash availability check is removed
- little refactoring
- method Mage_AdminNotification_Helper_Data::isReadablePopupObject() marked as deprecated
Fixed Onepage checkout - Shipping address issues
- added resetting property to save billing address in address book
- added saving of new shipping address
- simplified condition in order preparation routine
Fixed Backordered Item Status on Orders
- saving current ordered items number for stock item and calculating backorder qty according to it
Fixed The product category is empty after moving category with products to another one
Fixed Magento Connect -> If substitute channel for package extension, MCM will send authorization data to the fake URL
Fixed Image Label is not Uploading properly
Fixed Category Tree -> Changing category color
Fixed With enabled "Inline Translation" its impossible to finish purchase
- Added checking for escaped html end tag
Fixed #0024559: Special Price to Date can not set Use Default Value
Fixed CMS -> Manage Pages: It's possible to save New Page with capital letters in URL key
- corrected js validation;
- added server-side url key validation.
Fixed Makeup of subcategories dropdown menu at front-end glitter with category fields bar
- removed property "z-index: 1" for #nav li.level-top
Revert changes from rev #83486
Fixed Tier prices are not recalculated in bundle product configuration with different currency
Fixed On Multi store installation, 'specials' rss feed includes specials from other stores
Fixed Subscribe to Order Status - translation problem
Fixed There is a spelling error with the translation
Fixed Single Coupon applying for each shipping location rather than whole order
- applying cart fixed rules for first shipping address order only
- store which quote address cart fixed rule was applied for in SalesRule_Model_Validator
Added method getDefaultCountry and constant XML_PATH_DEFAULT_COUNTRY into Mage_Core_Helper_Data
Added more abstract system config backend model for uploading files:
- removed duplicated logic from system config backend image model.
Fixed Grand total doubles when processing multi-shipping checkout and ordinary checkout
- cleaning address information when checkout type changes from multi-shipping to onepage
Fixed Problem with admin roles
Checkout page IE6/7 CSS bug fixed.
Fixed Edit product->"Inventory" tab - "Qty Increments" error contain mistake
Fixed No field for "Search Query"
Fixed Character "b" is added to Review
Fixed Retain the selected tab on editing CMS page
Fixed Invoices Tax class not displayed
Fixed Full tax summary on invoice
Fixed working with partial authorizations on first card submit
Fixed CMS can't create Hierarchy Node Link widget in IE8
Fixed The Wrong / not exist Url should be redirect to 404 page
Fixed Interface Locale needs additional country
Fixed The product category is empty after moving category with products to another one
Fixed 'Gateway error: A valid amount is required' appears during create Credit Memo for order, which uses Authorize.net
Fixed #19807: Product with visibility- Nowhere display on the fron-end in 'Last ordered items' block, if order create on back-end
Fixed Displaying Out of Stock Products on the front-end
- added price data for consider item stock status for wish-list and compare products items collections, in reorder for product collection which sales order item collection based on.
Fixed active tabs in store view scope while disabled PayPal methods
- Added functionality that disables corresponding methods in store view scope.
- Fixed related bug: in website view scope Express Checkout PE checkbox appears improperly checked after page load.
Fixed Active tabs in store view scope while disabled PayPal methods
Fixed Bundle price wrong when static qty above 1
Fixed No "Suspected Fraud" status for hacked orders
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
Fixed Don't show (-) in totals when shipping title and shiping method empty in a configuration
Fixed Product with price 0.00 possibility purchase through Shortcut PayPal button
Fixed Archived orders not displayed in customer's orders list
Fixed Fatal error on magento compilation
Fixed Mage::app() call is not overriding cache/var directories
Fixed After switching "Manage Stock" option, product prices index does not invalidate
Fixed Transfer Cart Line: dropdown with shipping Rates is absent on PayPal side
Fixed Can't choose Group at the creation new Order by admin
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
- added forgotten file from rev 84979
Fixed Bug in Error Message display for Send to Friend (Mage_Sendfriend_ProductController)
Fixed Admin order creation JS error message
Fixed Problems with category sort order
Fixed Button "Credit Memo" after refund partial per invoice is enabled
Fixed Report don't show order with status "Canceled"
Fixed Wrong quantity checks architecture in inventory observer
Fixed On page 404, link "go back" does not work
Fixed Category editing "Use Parent Category Settings" inconsistent behavior (Google Chrome)
Fixed Set products per Page
Fixed product review filter by customer does not work
- type is administrator when customer_id is NULL and store_id is admin store id
Fixed Product review filter by customer does not work
Fixed WYSIWYG Editor disabling issue
Fixed Quantity increment for Group Product Issue
Fixed #15780: Add configuration option to ignore SID on frontend
- Changed fieldset scope from global to website, because the field has website scope.
Fixed Message "The product has required options" appears twice in the back-end order for items with mandatory custom options
Fixed Meta description can be more than 255 chars
Fixed When creating a new customer from the backend in "Manage Customers", the welcome email is empty
Fixed  Image Label is not Uploading properly
- Slightly changed logic in adding image algorithms due to possible existence of added pictures
Fixed  JavaScript Calendar Date Range
- Also little fix to maintain corporate standards
Fixed Gift message displaying conditions not properly work on frontend and backend:
Fixed flat catalog tables do not contain varchar values for store view level
Fixed Add check "Use Default" for dependent form elements (in the admin), because if field "Use Default" it should be always disabled.
Fixed #21084: "can not" -> "cannot" text changes (found only one occurrence of "can not" and changed it)
Fixed New added required attribute should be filled in by customer before checkout
Fixed PayPal Billing Agreement presents in payment methods when no BA are created during admin order creation
Fixed Free Shipping Banner appears to be hard coded into the template file - replaced hardcoded callouts with CNS blocks. Two CMS blocks should be added to RR install.
Fixed Empty order status field
- Configuration mistake
Fixed Cart Rule discount with Fixed amount for a whole Cart is not applied for OnePageCheckout
Fixed Coupon with "Apply fixed amount discount for whole cart" does not apply to bundle products with dynamic price
Fixed Frontend additional attributes issue with price attributes.
Fixed Unable to translate "Submit Invoice" button
Fixed Undefined index after clicking on Print Shipment
Fixed Customer cannot be confirmed from the admin
Fixed Inline Translations don't work if you have more than one store
Fixed Invitation link has a session ID parameter
Fixed Magento creates order even if response from PaypalUk is empty
- response validation has been added
Fixed Displaying Out of Stock Products on the front-end
Fixed Incorrect billing/shipping address transfer from magento to PayPal (WPP Payflow Edition, WPP Payflow Edition EC )
Fixed User cannot be associated with webservice role if he was selected in the Role Users of Role inforamation Page
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- removed "beta" mark on CSS merger feature in system configuration, because known issue with different host names for different store views is solved
- split merged CSS storage into 2 parts: "css" and "css_secure"
- included "port" and "base host name" parameters into merger hash generation algorithm as parameters
Fixed: Default country setting not affect country select field default value on frontend 
Fixed Credit card data Iframe for PayflowLink is displayed on Order Review step for all payment methods
Fixed The Wrong / not exist  Url should be redirect to 404 page
- Added section availability in preDispatch
Fixed Report > Products Ordered ignores Store view switcher
- reforming $storeIds checks
Fixed Report > Products Ordered ignores Store view switcher
Fixed Cannot create or save after editing customer's Address, "Please enter the street" error appears on frontend
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Showing websites that only associated to current category or product.
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Fixed coding standards
Fixed Not all session data destroyed on logout
Fixed Inline Translation - Pages View Issue
- move cache types list in config
Fixed Shop By index range is build based on Excl. Tax value, but filter products in catalog based on Incl tax value. filter works incorrect
- it was problem with facets calculation, when we use Solr
Fixed Security issue - processing of disallowed actions with orders through direct URL
- wrong Credit Memo ACL resource name
Mage_Catalog_Model_Resource_Eav_Mysql4_Category_Flat
Fixed Different order amount in Google checkout and Magento orders
Fixed Bundle Product w/o required option calculates wrong fixed minimal price
Fixed Admin unable to uninstall payment method without editing config
- getMethodInstance method was rewrited
- Added instance check in some payment models according to this
Fixed lastInsertId invokes when no insert where proceed
Fixed Changing the root category for a store doesn't work correctly
Fixed Unable to translate notice messages, errors and success messages
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Tax of shipping method Flat Rate is not passed to the order while Google Checkout
Fixed Product Flat Data reindex
- disable flat data usage during reindex process
Fixed Catalog Rule does not work properly when condition uses Contains
Fixed Wrong prices (currency) for shipping price via UPS XML rates
Fixed Unable to translate product edit/create page
Fixed During product save operation, Magento disables keys for catalog_product_index_* tables.
Fixed FPT with prices included tax problem
- Added 'Catalog Prices' option check
Fixed Google Analytics e-commerce tracking not working
Fixed Empty bundle selections are shown as item options
Fixed Subtotal for Bundle product with quantity 2 calculates as for one
Fixed Remove initSessionLayoutMessages() from ProductController
Fixed Incorrect value of field "Custom Layout Update" causes fatal error
Fixed Duplicate of a product creates it with no SKU value and is saved
Fixed Field "Meta Description" should be has limit of 255 characters
Fixed Row subtotal is not displayed for Downloadable product in Backend
Fixed Bad styling of product options displayed in wishlist
Fixed Need to show item options of customer shopping cart at backend
Fixed Wishlist item configuration is not saved at backend
Fixed "OK" button instead of "Ok" must be on product configuration popups in backend
Fixed Products wishlist items are not sorted by added_at
Fixed Mage_Core_Model_Template doesn't properly restore old design context
Fixed StoreView value not in FlatCatalog for multiple-select type attribute
Fixed Rule condition "is one of" disappeared for category_ids attribute
- Added "is one of" and "is not one of" to multiselect type conditions
Fixed Security issue - the way to get URL-path of Admin side through Front-end URL
Fixed Pictures does not appears on the additional information tab on front end for product attribute with Catalog Input Type for Store Owner= Text Area
Fixed Add method which was accidentally removed
- Deprecated methods Mage_Catalog_Model_Product::loadParentProductIds, Mage_Catalog_Model_Resource_Eav_Mysql4_Product::getParentProductIds
Fixed Can't create refund online for Google Chekout
Fixed After pressing 'Cancel Payment' link nothing happens in Payflow Link payment method
Fixed class Mage_Core_Model_Store has problem with _processConfigValue and processSubst
- Added "@deprecated after 1.4.2.0" mark for processSubst() in Mage_Core_Model_Store
Fixed Category tree is missing for product, assigned to root category
Fixed Unable to translate "Delete Image" checkbox
Fixed wrong XML paths in isAllowed() method for system->Admin roles controllers.
Fixed Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
- Changed exception message
Fixed Different shipping amount for creditmemo from order page and invoice page
Fixed Tax rates with zip ranges doesn't match to addresses with asterisk ( * ) as zip code value
Fixed Fedex doesn't react to overrided in website scope BaseCurrency value.
Fixed Export Customers. Map billing or shipping street in the mapping interface. They won't be exported
Fixed Advanced Import Profiles doesn't work
Fixed Add New Customer Form: checkbox "Send Welcome Email" is not disabled if "Associate to Website"="Admin"
Fixed JS validation prevent submit form
Fixed Payment action: Ogone Default Operation is not working at all
Fixed There are no ability to create several Refunds to Order completed using Partial Authorization
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
Fixed URL key wasn't used while product save
Fixed Inline Translations don't work if you have more than one store
Fixed Tax Report Shows Wrong Tax Percent After Changing Tax Rate
- added grouping by tax percent in report collections
- modified unique key in the tax report aggregation table to allow generating report with grouping by tax percents
- data in the tax report aggregation table is truncated and lifetime statistics must be re-generated after upgrade
Fixed make increment_id fields unique in sales tables
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Orders: More than one filter to the same field is not possible
- Function items was changed.
Fixed Invoices: More than one filter to the same field is not possible
- Function items was changed.
Fixed Report counts configurable products twice
Fixed Tax rate with ZIP XXXXX* doesn't match to customer zip XXXXX
Fixed Method Mage_Wishlist_Block_Links::addWishlistLink removed
- Added "@deprecated after 1.4.2.0"
Fixed "Subscribed to Newsletter" success e-mail couldn't be sent if you changed customer's subscription in admin.
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Dashboard reports bug
- Added discount to Mage_Reports_Model_Mysql4_Order_Collection:::addSumAvgTotals()
Fixed Google base timeout
- Timeout is 60 seconds now.
Fixed Bundle product is not shipped correctly
Fixed Unable to translate product edit/create page
Fixed Dataflow customers export optimization
- customer groups are storing in memory instead of DB queries
Fixed Price layer navigation does not count product with zero price
Fixed Import Product doesn't work
- added empty file checking
Fixed Price Indexer does not apply configurable options surcharges for customer groups different to "NOT LOGGED IN"
Fixed Category Update Not Reflected in Left Nav
Fixed Notify Stock RSS Includes Products without stock
Fixed FPT is not shown in the order review page (for website)
Fixed SQL Upgrades have wrong implementation
Fixed Email to a friend error, existing Order Send Email error
- Added ability to access to /admin/sales_order/email/ action
Fixed Total Refunded Report shows Offline Refunded orders like Online Refunded
Fixed UPS XML Shipping method doesn't work, if country of shipping origin is not USA
- Added Mage::log() for errors @ Mage_Usa_Model_Shipping_Carrier_Ups::_parseXmlResponse()


==== 1.5.x-devel-88903 ====

=== Major Highlights ===
Balance Response, Partial Authorization Transactions, Authorization Reversals Support for MasterCard and Discover
3D Secure authentication for Authorize.net payment method
PayflowLink payment method
Improved Import/Export functionality
Ability to order composite products from backend and some extra functionality
- reconfigure already added products on front end
- adding preconfigured products in wish-list
Alternative media storage
- Database
- CDN
Order status management
- ability to add new status and assign to some state
- from now on statuses stored in appropriate DB table instead of configuration file
Ability to edit order addresses
- this functionality admin has link to edit address for order view page

=== Improvements ===
Upgraded Zend Framework to 1.11.0
Implemented new process of hashing parameters in Ogone payment method
- implemented an advanced hashing method that invokes all transaction parameters for building security hash
- updated fields sort order in system configuration
- added the new parameter which designates whether to use the old or advanced hashing method
- made SHA-IN and SHA-OUT sys config parameter titles corresponding to parameter titles on merchant site in Ogone
- major refactoring of the Ogone helper: simplified public interface of hash validation, added support for SHA-1, SHA-256 and SHA-512 algorithms (not selectable in system config)
- optimized performance of debugging and building redirect form: removed 2 excessive calls (one from template, another from debugging - it invoked form building even if debugging was disabled)
- since the form is built from a block, prevented injecting SID parameter to URLs when building form
- added HTML escaping in the template hidden fields
- added new system configuration parameter - hashing algorithm
- verified/fixed all API hashing parameters in accordance to documentation v.5.0

=== Fixes ===
Fixed Onepage checkout - Shipping address issues
- added resetting property to save billing address in address book
- added saving of new shipping address
- simplified condition in order preparation routine
Fixed Backordered Item Status on Orders
- saving current ordered items number for stock item and calculating backorder qty according to it
Fixed The product category is empty after moving category with products to another one
Fixed Magento Connect -> If substitute channel for package extension, MCM will send authorization data to the fake URL
Fixed Image Label is not Uploading properly
Fixed Category Tree -> Changing category color
Fixed With enabled "Inline Translation" its impossible to finish purchase
- Added checking for escaped html end tag
Fixed #0024559: Special Price to Date can not set Use Default Value
Fixed CMS -> Manage Pages: It's possible to save New Page with capital letters in URL key
- corrected js validation;
- added server-side url key validation.
Fixed Makeup of subcategories dropdown menu at front-end glitter with category fields bar
- removed property "z-index: 1" for #nav li.level-top
Revert changes from rev #83486
Fixed Tier prices are not recalculated in bundle product configuration with different currency
Fixed On Multi store installation, 'specials' rss feed includes specials from other stores
Fixed Subscribe to Order Status - translation problem
Fixed There is a spelling error with the translation
Fixed Single Coupon applying for each shipping location rather than whole order
- applying cart fixed rules for first shipping address order only
- store which quote address cart fixed rule was applied for in SalesRule_Model_Validator
Added method getDefaultCountry and constant XML_PATH_DEFAULT_COUNTRY into Mage_Core_Helper_Data
Added more abstract system config backend model for uploading files:
- removed duplicated logic from system config backend image model.
Fixed Grand total doubles when processing multi-shipping checkout and ordinary checkout
- cleaning address information when checkout type changes from multi-shipping to onepage
Fixed Problem with admin roles
Checkout page IE6/7 CSS bug fixed.
Fixed Edit product->"Inventory" tab - "Qty Increments" error contain mistake
Fixed No field for "Search Query"
Fixed Character "b" is added to Review
Fixed Retain the selected tab on editing CMS page
Fixed Invoices Tax class not displayed
Fixed Full tax summary on invoice
Fixed working with partial authorizations on first card submit
Fixed CMS can't create Hierarchy Node Link widget in IE8
Fixed The Wrong / not exist Url should be redirect to 404 page
Fixed Interface Locale needs additional country
Fixed The product category is empty after moving category with products to another one
Fixed 'Gateway error: A valid amount is required' appears during create Credit Memo for order, which uses Authorize.net
Fixed #19807: Product with visibility- Nowhere display on the fron-end in 'Last ordered items' block, if order create on back-end
Fixed Displaying Out of Stock Products on the front-end
- added price data for consider item stock status for wish-list and compare products items collections, in reorder for product collection which sales order item collection based on.
Fixed active tabs in store view scope while disabled PayPal methods
- Added functionality that disables corresponding methods in store view scope.
- Fixed related bug: in website view scope Express Checkout PE checkbox appears improperly checked after page load.
Fixed Active tabs in store view scope while disabled PayPal methods
Fixed Bundle price wrong when static qty above 1
Fixed No "Suspected Fraud" status for hacked orders
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
Fixed Don't show (-) in totals when shipping title and shiping method empty in a configuration
Fixed Product with price 0.00 possibility purchase through Shortcut PayPal button
Fixed Archived orders not displayed in customer's orders list
Fixed Fatal error on magento compilation
Fixed Mage::app() call is not overriding cache/var directories
Fixed After switching "Manage Stock" option, product prices index does not invalidate
Fixed Transfer Cart Line: dropdown with shipping Rates is absent on PayPal side
Fixed Can't choose Group at the creation new Order by admin
Fixed PayPal API Certificate uses settings from the default configuration, instead of the website
- added forgotten file from rev 84979
Fixed Bug in Error Message display for Send to Friend (Mage_Sendfriend_ProductController)
Fixed Admin order creation JS error message
Fixed Problems with category sort order
Fixed Button "Credit Memo" after refund partial per invoice is enabled
Fixed Report don't show order with status "Canceled"
Fixed Wrong quantity checks architecture in inventory observer
Fixed On page 404, link "go back" does not work
Fixed Category editing "Use Parent Category Settings" inconsistent behavior (Google Chrome)
Fixed Set products per Page
Fixed product review filter by customer does not work
- type is administrator when customer_id is NULL and store_id is admin store id
Fixed Product review filter by customer does not work
Fixed WYSIWYG Editor disabling issue
Fixed Quantity increment for Group Product Issue
Fixed #15780: Add configuration option to ignore SID on frontend
- Changed fieldset scope from global to website, because the field has website scope.
Fixed Message "The product has required options" appears twice in the back-end order for items with mandatory custom options
Fixed Meta description can be more than 255 chars
Fixed When creating a new customer from the backend in "Manage Customers", the welcome email is empty
Fixed  Image Label is not Uploading properly
- Slightly changed logic in adding image algorithms due to possible existence of added pictures
Fixed  JavaScript Calendar Date Range
- Also little fix to maintain corporate standards
Fixed Gift message displaying conditions not properly work on frontend and backend:
Fixed flat catalog tables do not contain varchar values for store view level
Fixed Add check "Use Default" for dependent form elements (in the admin), because if field "Use Default" it should be always disabled.
Fixed #21084: "can not" -> "cannot" text changes (found only one occurrence of "can not" and changed it)
Fixed New added required attribute should be filled in by customer before checkout
Fixed PayPal Billing Agreement presents in payment methods when no BA are created during admin order creation
Fixed Free Shipping Banner appears to be hard coded into the template file - replaced hardcoded callouts with CNS blocks. Two CMS blocks should be added to RR install.
Fixed Empty order status field
- Configuration mistake
Fixed Cart Rule discount with Fixed amount for a whole Cart is not applied for OnePageCheckout
Fixed Coupon with "Apply fixed amount discount for whole cart" does not apply to bundle products with dynamic price
Fixed Frontend additional attributes issue with price attributes.
Fixed Unable to translate "Submit Invoice" button
Fixed Undefined index after clicking on Print Shipment
Fixed Customer cannot be confirmed from the admin
Fixed Inline Translations don't work if you have more than one store
Fixed Invitation link has a session ID parameter
Fixed Magento creates order even if response from PaypalUk is empty
- response validation has been added
Fixed Displaying Out of Stock Products on the front-end
Fixed Incorrect billing/shipping address transfer from magento to PayPal (WPP Payflow Edition, WPP Payflow Edition EC )
Fixed User cannot be associated with webservice role if he was selected in the Role Users of Role inforamation Page
Fixed CSS Merger Cache Ignores Hostname and HTTPS
- removed "beta" mark on CSS merger feature in system configuration, because known issue with different host names for different store views is solved
- split merged CSS storage into 2 parts: "css" and "css_secure"
- included "port" and "base host name" parameters into merger hash generation algorithm as parameters
Fixed: Default country setting not affect country select field default value on frontend 
Fixed Credit card data Iframe for PayflowLink is displayed on Order Review step for all payment methods
Fixed The Wrong / not exist  Url should be redirect to 404 page
- Added section availability in preDispatch
Fixed Report > Products Ordered ignores Store view switcher
- reforming $storeIds checks
Fixed Report > Products Ordered ignores Store view switcher
Fixed Cannot create or save after editing customer's Address, "Please enter the street" error appears on frontend
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Showing websites that only associated to current category or product.
Fixed Magento allows admin to create category/product url rewrite for a store that doesn't have this category/product
- Fixed coding standards
Fixed Not all session data destroyed on logout
Fixed Inline Translation - Pages View Issue
- move cache types list in config
Fixed Shop By index range is build based on Excl. Tax value, but filter products in catalog based on Incl tax value. filter works incorrect
- it was problem with facets calculation, when we use Solr
Fixed Security issue - processing of disallowed actions with orders through direct URL
- wrong Credit Memo ACL resource name
Mage_Catalog_Model_Resource_Eav_Mysql4_Category_Flat
Fixed Different order amount in Google checkout and Magento orders
Fixed Bundle Product w/o required option calculates wrong fixed minimal price
Fixed Admin unable to uninstall payment method without editing config
- getMethodInstance method was rewrited
- Added instance check in some payment models according to this
Fixed lastInsertId invokes when no insert where proceed
Fixed Changing the root category for a store doesn't work correctly
Fixed Unable to translate notice messages, errors and success messages
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Tax of shipping method Flat Rate is not passed to the order while Google Checkout
Fixed Product Flat Data reindex
- disable flat data usage during reindex process
Fixed Catalog Rule does not work properly when condition uses Contains
Fixed Wrong prices (currency) for shipping price via UPS XML rates
Fixed Unable to translate product edit/create page
Fixed During product save operation, Magento disables keys for catalog_product_index_* tables.
Fixed FPT with prices included tax problem
- Added 'Catalog Prices' option check
Fixed Google Analytics e-commerce tracking not working
Fixed Empty bundle selections are shown as item options
Fixed Subtotal for Bundle product with quantity 2 calculates as for one
Fixed Remove initSessionLayoutMessages() from ProductController
Fixed Incorrect value of field "Custom Layout Update" causes fatal error
Fixed Duplicate of a product creates it with no SKU value and is saved
Fixed Field "Meta Description" should be has limit of 255 characters
Fixed Row subtotal is not displayed for Downloadable product in Backend
Fixed Bad styling of product options displayed in wishlist
Fixed Need to show item options of customer shopping cart at backend
Fixed Wishlist item configuration is not saved at backend
Fixed "OK" button instead of "Ok" must be on product configuration popups in backend
Fixed Products wishlist items are not sorted by added_at
Fixed Mage_Core_Model_Template doesn't properly restore old design context
Fixed StoreView value not in FlatCatalog for multiple-select type attribute
Fixed Rule condition "is one of" disappeared for category_ids attribute
- Added "is one of" and "is not one of" to multiselect type conditions
Fixed Security issue - the way to get URL-path of Admin side through Front-end URL
Fixed Pictures does not appears on the additional information tab on front end for product attribute with Catalog Input Type for Store Owner= Text Area
Fixed Add method which was accidentally removed
- Deprecated methods Mage_Catalog_Model_Product::loadParentProductIds, Mage_Catalog_Model_Resource_Eav_Mysql4_Product::getParentProductIds
Fixed Can't create refund online for Google Chekout
Fixed After pressing 'Cancel Payment' link nothing happens in Payflow Link payment method
Fixed class Mage_Core_Model_Store has problem with _processConfigValue and processSubst
- Added "@deprecated after 1.4.2.0" mark for processSubst() in Mage_Core_Model_Store
Fixed Category tree is missing for product, assigned to root category
Fixed Unable to translate "Delete Image" checkbox
Fixed wrong XML paths in isAllowed() method for system->Admin roles controllers.
Fixed Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
- Changed exception message
Fixed Different shipping amount for creditmemo from order page and invoice page
Fixed Tax rates with zip ranges doesn't match to addresses with asterisk ( * ) as zip code value
Fixed Fedex doesn't react to overrided in website scope BaseCurrency value.
Fixed Export Customers. Map billing or shipping street in the mapping interface. They won't be exported
Fixed Advanced Import Profiles doesn't work
Fixed Add New Customer Form: checkbox "Send Welcome Email" is not disabled if "Associate to Website"="Admin"
Fixed JS validation prevent submit form
Fixed Payment action: Ogone Default Operation is not working at all
Fixed There are no ability to create several Refunds to Order completed using Partial Authorization
Fixed Incorrect shipping tax calculation on invoice creditmemos with included tax
Fixed URL key wasn't used while product save
Fixed Inline Translations don't work if you have more than one store
Fixed Tax Report Shows Wrong Tax Percent After Changing Tax Rate
- added grouping by tax percent in report collections
- modified unique key in the tax report aggregation table to allow generating report with grouping by tax percents
- data in the tax report aggregation table is truncated and lifetime statistics must be re-generated after upgrade
Fixed make increment_id fields unique in sales tables
Fixed Added items to the Wishlist in the "Manage Shopping Cart" are not shown
Fixed Orders: More than one filter to the same field is not possible
- Function items was changed.
Fixed Invoices: More than one filter to the same field is not possible
- Function items was changed.
Fixed Report counts configurable products twice
Fixed Tax rate with ZIP XXXXX* doesn't match to customer zip XXXXX
Fixed Method Mage_Wishlist_Block_Links::addWishlistLink removed
- Added "@deprecated after 1.4.2.0"
Fixed "Subscribed to Newsletter" success e-mail couldn't be sent if you changed customer's subscription in admin.
Fixed Problems with newsletter template preview on newsletter queue edit page
Fixed Dashboard reports bug
- Added discount to Mage_Reports_Model_Mysql4_Order_Collection:::addSumAvgTotals()
Fixed Google base timeout
- Timeout is 60 seconds now.
Fixed Bundle product is not shipped correctly
Fixed Unable to translate product edit/create page
Fixed Dataflow customers export optimization
- customer groups are storing in memory instead of DB queries
Fixed Price layer navigation does not count product with zero price
Fixed Import Product doesn't work
- added empty file checking
Fixed Price Indexer does not apply configurable options surcharges for customer groups different to "NOT LOGGED IN"
Fixed Category Update Not Reflected in Left Nav
Fixed Notify Stock RSS Includes Products without stock
Fixed FPT is not shown in the order review page (for website)
Fixed SQL Upgrades have wrong implementation
Fixed Email to a friend error, existing Order Send Email error
- Added ability to access to /admin/sales_order/email/ action
Fixed Total Refunded Report shows Offline Refunded orders like Online Refunded
Fixed UPS XML Shipping method doesn't work, if country of shipping origin is not USA
- Added Mage::log() for errors @ Mage_Usa_Model_Shipping_Carrier_Ups::_parseXmlResponse()


==== 1.4.2.0 ====

=== Major Highlights ===
* Starting from this release we are including TheFind extension.

== Upgrade Notes ==
* Those who installed Magento version 1.4.2.0-beta1 or 1.4.2.0-rc1 through Magento Connect should reinstall it manually, because its version number is the same as of the current release and no automatic update will be available for it.

== Improvements ==
* Added "Switch/Maestro" card type support to centinel 3DS validator. Added comment about maestro and 3d-secure to paypal system config
* Added more flexible filters implementation in collections:
** Varien_Data_Collection::addFilter() registers filters as objects and implements getFilter() method to be able to detect/modify already existing filters
** Varien_Data_Collection_Db::_renderFilters():
*** Added a hook _renderFiltersBefore()
*** Implemented 'public' filter type, which maps the provided filter field from public into internal view and passes the "value" as a condition through _getConditionSql()
** Added $this->_renderFilters() call to abstract EAV collection to accommodate the filters that may be set by addFilter() method
* Added ability to pass multiple recipient emails and names to Mage_Core_Model_Email_Template::send()
* Backordered Item Status for subitems in Orders
** Added correct message at order for all backordered items. At back-end all items shows as backordered if their quantity is below or equal to zero
** Fix of duplication backorder messages for composite product options with same backordered item - saving backorder messages per product id
* Magento Connect Manager
** checking cyclic dependency references and conflicts with local files
**  implemented adding to MCM manually installed extension
** changed upgrade logic, previous version of package should be deleted before install new
** Implemented new download process and dependencies rules
** Added correct behavior during extension reinstall, so dependencies will not reinstall automatically
* Optimized rewrite selection from DB, added url rewrite and suffix validation at admin backend
* Added verification of access level for app/etc/local.xml. 
** Now if server configuration has issue and this file accessible from browser admin user gets notification in backend.
* Upgraded Zend Framework to version 1.10.8
* Added the Recurring Profiles tab in customer management
* Implemented cache for shipping rates and fixing issues with rounding
* Design packages and themes optimization/refactoring/improvements:
** minor improvements and fixes
** improved upgrade-ability of CE themes
* iPhone Theme Refactoring
* Added Widget settings sharing between widget types
* For Invoices, Shipment, Credit Memos added possibility to show admin comments at user frontend (checkboxes "Visible on Frontend" in admin interface)
** Added JS to enables/disable checkbox 'Append Comments' depending on checkbox 'Email Order Confirmation'
** Refactored invoice/shipment/refund comments collections models to one abstract Comment Collection Model
** Refactored Block Order Invoice/Shipment/Creditmemo comments to usage of common block and design - Block Order Comments
* A little more accurate profiler - important for very quick measurements
* Add Shopping Cart API
* Implementing payment refund notifications
* Added website price scope for bundle items
* Added support of pending transaction to payflow pro. Also fixed "denied payment review" message in payment
* Upgraded TinyMCE to v.3.3.7
* Added to prototype validation by length min-length validation
* Added Varien.DateElement for front-end date form fields and re-implemented Varien.DOB
* Added functionality to disable dashboard charts in backend (System > Configuration > Admin > Dashboard)
* Added functionality to disable dashboard charts during installation
* Adminhtml W3C Validation improvements
* Added ability to use session save method from configuration
* Rendering customer attributes
* Added favicon manager under System > Configuration > Design > HTML Head

== Changes ==
* Refactored shipping rates calculation to keep process solid and do not try to recreate internal process of calculation, as it was
* Added caching of requests to shipping carriers, because otherwise we get too much duplicate requests during calculation of every shipping method
* Refactored "Special products" RSS feeed
* Shortened the names of all foreign keys longer than 49 characters
* Compilation scope for some EAV models which was causing blank page after enabling compilation
* Deleted Mage_Sales_Model_Recurring_Profile_Info, which was not on its place and added accidentally
* Category and product design settings inheritance logic
* Refactored one routine in Inventory Observer to remove code duplication
* Disabling product attribute usage in promo rules not affect existing promo rules
* Refactoring validation states for Centinel
** Added template method Mage_Centinel_Model_StateAbstract::isLookupSuccessful
* Add boolean type for catalog price rules and condition for category_ids
* Removed Maestro/Switch/Solo card from system. Added Maestro/Switch and Solo cards to Chronopay and Cybersource methods
* Mage_Adminhtml_Block_Sales_Order_Creditmemo block had dependence from 'canCapture' 'canCapturePartial'. It was changed to 'canRefund' 'canRefundPartialPerInvoice'. For set result of Mage_Adminhtml_Block_Sales_Items_Abstract::CanEditQty`s we can use setCanEditQty
* Added Maestro/Switch and Solo Dollars card types for paypal_direct payment method. Also removed Maestro/Solo/Switch card type for this method
* Removed "Shipping address" block on recurring profile view page if product is virtual. Also fixed virtual order detection
* Refactored PayPal cart line items and cart totals calculation to accommodate various discounts and tax settings
** added hidden discount and hidden shipping taxes to the calculation
** eliminated cart line items logic from the helper, moved it to the paypal/cart model
** simplified transferring of the totals and line items to PayPal API objects
* Refactored sales rule discount detection on "buy_x_get_y" rule type
* Added catalog_product table definition to product review collection
* Changed type of obscure input field to 'password', so this field is hidden even when user enters data in it
* Removed dependence to payment method on getting billing agreement method title. For now payment method title stored in billing agreement
* Removed invoice creation thought zero subtotal checkout with new order status "pending"
* Removed SID from url generation when Use SID on Frontend option is disabled
* Added customer session validation for loadCustomerQuote method
* Iphone clears.css has been deleted

== Fixes ==
* Fixed Default shipping address is passed to PayPal instead of the selected shipping address
 * reverted cloning of shipping address and it's setting to quote.
 * implemented method assignCustomerWithAddressChange() with setting billing and shipping addresses
* Fixed Added transferring of last four digits of credit card number to give possibility refund authorize transactions.
* Fixed Returning from paypal cancel existing order
 * Canceling order in cancelAction() only if it was placed from current quote
* Fixed Taxes->Incorrect product price and tax value on the last chechout step
* Fixed Opening bestseller product (admin/dashboards) results in adding new product
** fixed case when dashboard shows report for non-existing product (i.e. deleted one)
* Fixed Bestsellers statistic bug
** removed NULL values from statistic tables and changed foreign keys to cascade deleting stats for deleted products
* Fixed Gift message displaying conditions not properly work on frontend and backend
* Fixed QTY of product is incorrectly showed in Customer's Current Activities - Shopping Cart and Customer's Shopping Cart.
* Fixed Gift message displaying conditions not properly work on frontend and backend - fixed missed bracked
* Fixed Magento Connect Manager -> No warning message
* Fixed Unable to upload community extention in Magento Connect Manager without Community Channel installed
* Fixed Bundle product price calculated not correctly
* Fixed Customer's email doesn't escalate to billing/shipping addresses
** added copying email field from quote address to order address
** added sending email to PayPal, when user's address doesn't contain email info
* Fixed Catalog-specific attribute options do not load when using through catalog/output helper
** method _getLoadDataFields at product attribute resource collection modified to select additional needed fields;
* Fixed saving attribute value in store view scope only
* Fixed Not searchable attributes are searched by Quick search.
* Fixed Customers won't appear in the search results on the customer grid in the admin
* Fixed Huge memory consumption on flat shipping rates import
** decrease to 5000 count of data wich inserts into DB in one iterate, to avoid exceed of 128M memory_limit
* Fixed Config fields "Disable output" doesn't implement inherited value
* Fixed Category created for some store view not displayed on frontend
** include_in_menu attribute was made as required to set default value when category created in specified store
* Fixed creating of  "Shopping Cart Price Rule'
** setActualProductAttributes method was called with 'attribute_set_id' value in $attributes param. But it does not exist in 'eav/attribute' table. So we need to check it
* Fixed PayPal PE transaction_id detection: Overrided getPaypalTransactionId method in PE API -  changed transaction id getting to process payflow accounts not assigned to paypal side
* Fixed Configurable Product Catalog Price Rule Issue: the main idea is to calculate price rule on configurable price separately from base price
* Fixed fatal error during import large file
* Fixed Shipping information is not displayed in backend after Google Checkout operations
* Fixed Field Mapping Issue during customer import
* Fixed CMS blocks grid inoperable with store filter in GWS-limited mode
* Fixed incorrect qty increment behaviour
** qty increment not decimal validate
** when adding product with qty increment to cart - redirect to product's page
** generate message about mismatch of qty increment when editing item qty at cart
* Fixed ups/usps and Guam
* Fidex issues with attaching product to multiple stores: refresh product index query update
* Fixed displaying of bundle product weight
* Fixed "Select a PayPal Solution" checkbox bug: Website Payments Pro and  Website Payments Pro Payflow Edition consider each other status in their checkboxes control logic
* Fixed Invoice Comments Stripped When Quantities Updated
* Fixed XSS security issue on frontend
* Fixed Google Chekout: Discount for shipping amount doesn't apply
* Fixed XSS issue in address form
* Fixed Address in the customers address book cannot be deleted
* Fixed CatalogSearch_Fulltext not being renewed for configurable products when editing attached simple products
* Fixed Google Checkout: shipping method info is empty at order page in admin backend
* Fixed Google Checkout: with discounted shipping - discount is applied again
* Fixed Wrong timezone/DST in reports
* Fixed coupon_code attribute inconsistency in some upgrade paths (from 1.4.0.0 to 1.4.1.0)
* Fixed  Created extension archive through Magento Connect include ".svn" directories
* Fixed version of downloader
* Fixed Magento Connect: User should has a possibility to choose version for extension upgrade
* Fixed Magento Connect: User shouldn't be able to download Magento into "0000 permissions" folders
* Fixed Magento Connect: JS validation is absent for "Authors" tab on  package extensions page
* Fixed Magento Connect: Saving information on settings page
* Fixed Magento Connect: "Configuration" step - server validation is absent during installation
* Fixed Magento Connect: "Log in" page - Message or some information about required fields doesn't appeared
* Fixed Magento Connect: "Configuration" step - incorrect message appeared during installation
* Fixed wrong shipping price in case of sales rule with fixed cart discount and 1 item in cart
* Fixed the label for the configurable product attribute does not reflect correctly on the frontend
* Fixed sales rule with fixed discount for whole cart doesn't work
* Fixed "Slash for category or product urls causes error 404" 
* Fixed Shared shopping cart on the stores with different domains
** check origin url in all store urls
** prevent to getting SID param from current query
* Fixed #18454: Import profiles do not reset websites values
* Fixed Issue with zero grand total express checkout for recurring products.
* Fixed "Allow Gift message" setting on the product page doesn't work in Front.
* Fixed "Duplicate" of bundle product leads to an error
* Fixed Catalog sitemap for categories shows inactive sub categories if flat catalog enabled
* Fixed Added support of all product attributes in conditions/actions of salesRules.
* Fixed Disabling product attribute usage in promo rules not affect existing promo rules
* Fixed "Cart Price Rule not working with Product Attributes" (boolean values not properly shown in rule conditions)
* Fixed Wrong amounts invoiced with FPT
* Fixed Wrong order status after refund and additional related issue on frontend during checkout
* Fixed Unable to delete uploaded sample for downloadable product
* Fixed Paypal Direct send wrong billing address to API
* Fixed Incorrect viewing of category settings after refreshing page
* Fixed Catalog price rule discount not working during backend order creation
* Fixed Double headers for session cookie set
* Fixed Custom design is not reset properly after shipment comment emails
* Fixed Tax report displays incorrect figures
* Fixed Removed invoice creation on "completed" IPN message with payment_entity = "auth" to prevent double capture creation on single transaction with IPR.
* Fixed Image browser in WYSIWYG editor doesn't fill mouse over/out fields
* Fixed Added rounding to "Refund Shipping" field on credit memo creation page.
* Fixed Added additional error messages to customer address validation on PHP side while creating.
* Fixed "No server side check for password length when customer edits his account information" 
** Also added proper processing for password == '0', earlier it was considered as non-set password
* Fixed WYSIWYG editor breaks directives that are not in src attribute
* fixed directives decoding for a case when the secret key is present in URLs
* Fixed Duplicate of a product creates it with no SKU value and is saved
* Fixed Redundant catalog product attribute "category_ids" remains during upgrade from 1.3 to 1.4
* Fixed Reports/Shopping cart/Products in carts optimization
* Fixed "If all Storeviews value set up - disabled --> Front end shows default storeview instead of 404 page"
* Fixed Added error on zero subtotal checkout with paypal express. Removed paypal express button on shopping cart with zero grand total.
* Fixed Field labels and field values are not aligned vertically on Sales Orders in Admin
* Fixed Spacing between field labels and field values is inappropriate on the Recurring Profiles tab in My Account section
* Fixed Not searchable attributes are searched by Quick search.
** Checking if attribute used in quick search before adding to fulltext field
* Fixed Mage_Customer_Model_Customer::getGroupId can't return zero value
* Fixed #23184: Huge memory consumption on flat shipping rates import
* Optimized and refactored Table Rate import
* Fixed Scrolling during category load results in some js-errors
* Fixed "Javascript alert on "manage category" page"
* Fixed Security Vulnerability on Mage_Core_Block_Template level
* Fixed Merged CSS breaks Secure Pages (https)
* Fixed SOAP webservices do not work when enabling "Add Store Code to URLs"
* Fixed Incorrect displaying of the Start Date entered by customer while adding to the cart recurring product
* Fixed Downloadable Product "lable" typo
* Fixed While creating gift message from backend it disappears in case of refreshing page
* Fixed Product export fails when the quantity of exported products is 25 000 or more (memory leak in products)
* Fixed While creating gift message from backend it disappears in case of refreshing page
* Fixed Google Chekout: Discount for shipping amount doesn't apply
** onepage checkout recalculates shipping charges after setting the payment method (not solved yet in multishipping)
** added warning about Carrier Calculated Shipping in Google Checkout system configuration
** GC API callback now sets the payment method to quote on requests
** the free shipping calculator now marks the entire address as "free shipping" if all its items have free shipping
* Fixed On wide monitors checkbox "Create Permanent redirect" in admin backend wraps up to the end of input box
* Fixed Tag isn't showed in Product Page and My account->My Tags, if tag are deleted by customer, approved by administrator, added by customer
* Fixed Non standard images make troubles with "Next"/"Previous" buttons
* Fixed There is no validation of the Tracking number field during first time creation of the shipment
* Fixed Missed dollar sign in variable name
* Fixed Incorrect escaping of Mage_Catalog_Model_Abstract::loadByAttribute method
** Zend_DB_Select::where must get null values to skip quoting into $cond empty strings if value is null
* Fixed "URL rewrites duplicating when assigning to root category"
* Fixed Shipping method UPS_XML missing titles
* Fixed The pager is missing for tagged product list
* Fixed Report > Products Ordered ignores Store view switcher
* Fixed Flat catalog index problem after upgrade with customizations present
* Fixed Incorrect bundle items inventory decrements
* Fixed Category and product design settings inheritance
* Fixed Removed fatal error on removing non existent quote item from quote
* Fixed Credit Card Maestro/Solo: The field "Start Date" is not displayed on order information page
** deleted unused Maestro/Solo from Payment module config
** moved Maestro/Switch and Solo card definition from Chronopay to Payment module config
** deleted Meastro/Switch definition with incorrect code MS from Cybersource module config
** fixed logic of showing "Issue number" and "Start Date" of Switch/Solo card on frontend
* Added warning about offline refund
* Fixed Mage_Checkout_Block_Cart_Item_Renderer::getIsInStock bug
* Fixed Fatal on edit configurable product page, if custom required price attribute is used
* Fixed #0011135: View invoice error with changed query string
* Fixed Trailing semi-colon displayed on Profile Export page
* Fixed New Orders & Other Authenticated RSS feeds should use HTTPS
* Fixed Dataflow export products sku filter works as not "starts with", but "like"
* Fixed Removed default shipping address assign on paypal express checkout
* Fixed The customers from Puerto Rico can't pay with PayPal (Express Checkout in PaypalUk)
* Fixed Shared shopping cart on the stores with different domains
* Fixed Discount amount for the whole cart divide proportionally between all affected items according to their base price and then applied.
* Fixed Removed store selector in single store mode on url rewrite edit page
* Fixed Javascript validator's translation strings missing
* Fixed Quick Search Autocomplete does not work via ajax http protocol for https page
* Fixed Inventory->Qty Increments - unable to add
* Fixed Loading search query performance issue
* Fixed Changed labels in checkout and payment information blocs for credit cards Solo Maestro Switch 
* Fixed Product q-ty doesnt decrease after google checkout
** added same 'checkout_submit_all_after' event to  AmazonPayments
** removed 'TODO' notice from Multishipping Checkout, because current scheme is better and will not be influenced by any Multishipping refactoring
** fixed Observer reaction on 'checkout_submit_all_after' to include needed reindexing
* Added checkout_multishipping_controller_success_action and checkout_onepage_controller_success_action events that pass the created order ids on frontend checkout success actions
* Fixed Google Analytics tracking pages with wrong URI:
** Completely reimplemented googleanalytics/ga block:
*** it doesn't depend on session/quote, but just uses order_ids, if passed
*** the page_name parameter is reimplemented as it was intended to be: an optional parameter that can be customized via layout for certain actions
*** moved out the integration part with google checkout to observer
*** eCommerce tracking passes shipping address instead of the billing address, if available
*** replaced the "affiliation" into store frontend name in eCommerce tracking (as it is intended to be)
*** eliminated passing order item "category" in eCommerce tracking (that never existed)
*** optimized javascript code of GA with Google Checkout integration
** Eliminated mutual code coupling between Google Analytics and Google Checkout modules
** Improved integration of Google Analytics and Google Checkout:
*** the GA integration should appear only when GC buttons are available
*** there will be no integration when there is no GA tracking code configured
*** the GA/GC integration seems like wasn't working because there was no pageTracker js variable accessible to the GC scripts
* Fixed Wrong links in backend to "New Products/Low Stock/Customer reviews" RSS feeds
* Fixed "Send auto-generated password" generates e-mail with incorrect template
* Fixed Unable to refund Credit Memo because of Shipping Rounding
* Fixed Added custom option info to recurring profile info page on frontend and backend.
* Fixed Product Visibility and Status disappear when in search
* Fixed Removed validation of new customer shipping address on backend for orders with virtual products only 
* Fixed ability to buy Product which have status "Out of Stock" through a direct link on button "Checkout with PayPal"
* Fixed All free shipping methods in absent in Transfer Shipping Options menu on PayPal side
* Fixed Payment methods titles for the PDF prints through admin gets from default config instead of the storeview config
* Fixed PayPal and Puerto Rico shipping address
* Fixed "Transfer Shipping Options" pass on PayPal side not correct value for Flat Rate method
* Fixed Centinel JCB validation test cases 8-9
* Fixed Saving caterory in store view scope
* Fixed Attribute upgrades moved from 1.4.0.0.15 to 1.4.0.0.33
* Fixed that product tagged by administrator has wrong URL at front-end
* Fixed refusal from Card Verification (through link Exit), does not allow to place order repeatedly
** If lookup was filed and customer tries again we will do new lookup.
** If lookup was success and customer tries again without some changes we will not do new lookup
** If authentication was filed and customer tries again we will do new lookup and authentication
** If authentication was success and customer tries again without some changes we will not do new lookup and authentication
* Fixed #22536: Light-weight email templates. Wishlist share email fix
* Fixed declaration of Mage_Cybersource_Model_Api_ExtendedSoapClient::__doRequest() compatibility with SoapClient::__doRequest()
* Fixed Two registration emails from a wrong store and without a logo are sent when a customer is created in Admin panel
* Fixed Reindex for bundle products with date fields
* Fixed Status is "Ready" instead to be "Reindex required" then creating new subcategory in mode "Manual Update"
** index status changed to STATUS_REQUIRE_REINDEX when search engine changes
* Fixed #23321: Wrong type casting in method
* Fixed Print-All Includes Tracking # from All Shipments on Every Shipment
* Fixed Ignored 'Include in Navigation Menu' category option with enabled flat catalog.
* Fixed Admin unable to add Image through WYSIWYG to description and Short description without intermediate product saving
* Fixed QTY decrement after multishipping
* Double clicking adds product to cart twice
* Fixed Catalog Price Rule(for NOT LOGGEN IN customers) is not applied for shopping cart and while checkout as guest or while first registration.
* Fixed Payment methods titles for the PDF prints through admin gets from default config instead of the storeview config
* Fixed Mage_Adminhtml_Model_System_Config_Backend_Serialized::_afterLoad() does not check input for unserialize()
* Fixed Sending letters through "Contact Us" form, leads to error
* Fixed PayPal Express with Flat Rate: incorrect counting Shipping amounts per order
* Fixed Saving attribute value in store view scope only causes data loss.
* Fixed #22607: Dispose of Mage_GiftRegistry module
* Fixed Related products are not saved when you attach them to a product
* Fixed Added qty to bundle unit price calculation to quote totals recalculating.
* Fixed Saving category cause: 'Exception' with message 'File was not uploaded.' in /home/vadim.kusakin/dev/qa/2759/lib/Varien/File/Uploader.php:139
* Fixed Fixed Magento Connect -> MCM -> If agreement checkbox is unchecked, "Continue" button should be disabled
* Fixed Set the same column font size as in cells in PDF documents printing
* Fixed Home page appears instead of predefined 404 page
* Fixed Removed converting of "is one of" and "is not one of" values in decimal.
* Fixed Wrong column type for order_increment_id on Invoice, Shipments, Creditmemo grids
** order_increment_id was setted as "text" instead of "number" type
* Fixed Inconsistency with credit memos showing buttons online vs offline
* Fixed PayPal Express shortcut is missed on product page
* Fixed An email is sent to a customer after its profile is edited in the Admin panel
* Fixed that Payflow Pro includes only the first line of billing/shipping addresses into request
* Fixed Incorrect showing of product page when inputing a product description with table which have attribute align = left
* Fixed Wrong link for bestsellers in admin dashboard. Grids.php fixture doesn't do anything for this bug - just to beautify code.
* Fixed Added fixes to reports - base_discount_amount is actually kept negative in DB.
* Fixed Empty dropdown 'status' at the creation New Review Grid.
* Fixed Incorrect work of "Recently Compared Products" functional on category's page
* Fixed behavior when having single store, javascript raises exception and all followed code is not executed
* Fixed that Special price for dynamic bundle applies twice
* Fixed #21960: Labels in page/html_wrapper and core/text_list in layout 
* Fixed GUI bugs on Recurrent Profile frontend part
* Fixed Magento Connect -> Message about invalid URL is duplicated
* Fixed that suspend Recurring Profile from front side leads to error
* Fixed Missing pager for tagged product list
* Fixed Wrong profiler output for getUrl in Category
* Fixed Saving of billing agreement relation with order - added force billing agreement re-saving and fixed isValid method in agreement detection.  
* Fixed Incorrect sort order reliable on mysql internal order during eav attribute load
** move prepare select to separate method
* Fixed passing additional totals to PayPal when cart line items are disabled:
** simplified paypal/abstract api to just set the paypal/cart instance and the needed configuration settings
** moved workarounds of setting shipping and discount totals as line items into the appropriate APIs: WPS and NVP
* Fixed In My product Review short description HTML tags are shown
* Fixed that Refund from google chekout don't display on the order in Magento
* Fixed that "Compare Products" block does not appear on the category page and product page
* Fixed Non-existing attribute's source model causes fatal error
* Fixed Varien_Db_Select memory leak
* Fixed #18569: Gift Messages not in OrderInfo returned array
* Fixed PayPal API credentials wizard popup size
* Fixed #11449: customer_id is mismatch with entity_id in customer.create
* Fixed merging CSS-files with different skin domain to pick a proper base URL
* Fixed Bad UI style on checkout success page
* Fixed buying more than 1 virtual product in multishipping checkout
* Fixed #22518: Wrong amount for second refund
* Fixed #22776: Bug Causing Recursion Error
* Fixed #22668: Incorrect reports for coupons
* Fixed Products -> Product with "Out of stock" status displayed on frontend, but shouldn't
* Fixed Password miss match for newly created in Back end customer
* Fixed "There has been an error processing your request" page is displayed when specified order status is selected on Reports->Sales->Tax page
* Fixed bug with 'Use Flat Catalog Category'
* Fixed #13770, #16300, #21040 : Product Media Api Broken, product_media.create API overwrites image itself each upload, product_media.update API does not upgrade the image itself
* Fixed #16306: Webservice with htaccess (changes in code style)
* Fixed #22536: Light-weight email templates 
* Fixed #18935: Soap api v2 multiple complexFilters with the same key
* Fixed incorrect Window titles on frontend
* Fixed Eliminated display currency usage (instead of the base website currency) in shopping cart price rule conditions
* Fixed #21146: Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
** corrected syntax mistakes
* Fixed batch of issues related to google checkout:
** Invoice don't create automatically with Google Checkout
** Google checkout invoice duplication
** Automatically authorize the buyer's credit card for the full amount of the order
** Refund from google checkout don't display on the order in Magento
** Google Chekout: Discount for shipping amount doesn't apply
** Different order amount in Google checkout and Magento orders
** Applying of discount for shipping, when using google checkout
** Order is in google sandbox doesn't contain gift card
* Fixed #23461: Wrong attribute value in catalog link widget XML
* Fixed getting complete state for orders with zero grand total when processed
* Added Store id param to billing agreement entity.  Also fixed store setting in billing agreement payment method.
* Fixed fatal error in payment method list fetching
* Fixed #22575: Trace error during using filter "Products" on Tags page
* Fixed Grids with settings remain active while disabled PayPal methods
* Fixed configuration merger fatal error when store/website resource structure is inconsistent
* Fixed PayPal admin setup: checkbox problem
* Fixed Adding shipping address transferring on non guest checkout in Paypal Standard
* Fixed "Save in address book" checkbox in the Shipping address area doesn't work while admin order creation
* Fixed pre-selecting default address during checkout
* Fixed Email with empty password is sent to a customer after an order is created in the Admin panel
* Fixed Necessary to add data validation for filed "Trial Billing Frequency" in Recurring Profile
* Fixed "Out of Stock" product is possible to purchase successfully through Shortcut button
* Fixed phpdocs in lib/Varien and removed junk file
* Fixed #21146: Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
* Fixed #21643: Fixed "wsdl" parameter validation for Soap V2
** Changed class SoapServer with class Zend_Soap_server
** Added ability to set response charset from admin panel: System->Configuration->Magento Core API
* Fixed #21499: Default billing and shipping address
* Fixed #21565: missing "comment" for salesOrderStatusHistoryEntity
* Fixed #20481: Access Control List not retrieved for API user for resources() and resourceFaults() operations
* Fixed #18367: FCGI Error on WSDL Url with Apache and mod_fastcgi
* Fixed #22053: use HTTP 301 code instead of 302 in case of web/url/redirect_to_base
* Fixed #20654: Admin order creation->Move mouse cursor isn't changed into hand while move it on some product for adding 
* Fixed #21590: Attribute 'Date': testing for uniqueness fields not working
* Fixed #21566: Type of attribute 'Price': Possible to add text value for field 'default value'
* Fixed #22053: added optional behavior (301 or 302)
* Fixed #21570: Review from not logged in user is saved in list of All Reviews when "Allow guests to write reviews = No"
* Fixed #22090: Different values of Qty Increments during create and after duplicate products
* Fixed #22489: Eliminate difference between bundle.js in different skins 
* Fixed #22419: Set default stock_data if not exist in create/update product
* Fixed #20227: "Review(x)" link should be added to the compare page.
* Fixed #21570: Review from not logged in user is saved in list of All Reviews when "Allow guests to write reviews = No"
* Fixed #20959: Locale problem in shipping tracking popup raises exception 
* Fixed #21955: Layout cache ignores product column count update
* Fixed #20011: After using filter "Color" or "Manufacture" in Configurable Product meaning from column is disappear
* Fixed #21908: Incorrect attribute ordering in "Compare products" page.
* Fixed #22222: Edit review-> if browse stores in the "Visible In " drop-down, rating values reseted 
* Fixed #22075: Product Attribute title specified for StoreView isn't showing on the configurable product's page
* Fixed #22605: catalog_category.level return root categories when website or store are null
* Fixed #21806: Different values display on the shopping cart in front-end and back-end 
* Fixed #20113: Shipping address display as default on the front-end and as not default on admin for one customer 
* Fixed #22575: Trace error during using filter "Products" on Tags page
** added 'filter_index' to array parameter in addColumn() method call
* Fixed #14591: Incorrect SKU for Configurable Product with Custom Options 
* Fixed #22476: Blank Column in Related Products Grid
** deleted duplicate <col> output for editable columns
* Fixed #22575: Trace error during using filter "Products" on Tags page
** apply filter_index field values to index
* Fixed #22644: A discrepancy between GT(Base) and GT(Purchased) 
* Fixed #22645: Incorrect original price when using custom price in order. 
* Fixed #22653: Missed checking for file existence in JS/CSS merger
** checking in source file exists. If not - do not check last modification and force to merge target file again
* Fixed #22594: Unable to place orders through checkout with multiple addresses with PayPal direct + zero subtotal for one order 
* Fixed #21185: Newsletter confirmed automatically BEFORE account email is confirmed. 
* Fixed #22167: "Add new row" button in downloadable product 
* Fixed #21952: BUG - Category / Url Model (UYN-886991) 
* Fixed #15334, #17794
** API category did not pass validation process due to available_sort_by must be ArrayOfString
** Added category validation for backend (missed)
** Creating separate validation for available_sort_by and default_sort_by attributes
* Fixed #22599 Upgrade from 1.1.8 to 1.8.0.0 database compatibility issues (PARTIAL)
* Fixed #22661: 1 cent bug 
* Fixed #22434: 100% discount of products -> the amounts of Tax and Grand Totals are or negative or not corectly 
* Fixed #10073: Unnecessary option for downloadable products
* Fixed #20014: Qty use decimals for downloadable
* Fixed #22164: Incorrect message for maximum shipping amount
* Fixed #22174: Custom 'Qty to Refund' isn't remembered after message about incorrect amount
* Fixed #22182: The value of 'Customer Since' field to duplicate clients at different sites.
* Fixed #22243: Add new review by admin->type of this review is 'guest', but should be 'administrator'
* Fixed #22313: Time of order creation if not displayed by the "Order Created At (datetime)" template variable.
* Fixed #22348: "Add to card" button is absent for giftcard product in the catalog
* Fixed #22640: Creating customer unable after adress tab manipulations
* Fixed #22670: Credit memo - incorrect shipping price displaying
* Fixed #22798: Excl and Inc. Tax don't display on the Estimate Shipping and Tax block
* Fixed #20088: Admin able to push on-line refund button for the capture off-line invoice
* Fixed #16306: Webservice with htaccess. Added server authorization (.htaccess)
* Fixed #22266: HEADERS ALREADY SENT Error during dataflow import
** Additionally: moveing layout update in separate layout file of dataflow module.
* Fixed #21412: The "Save Attribute" and "Save and Continue Edit" buttons become disabled after saving attribute with attribute code that exists
* Fixed #22844: After login to admin got 404 instead Startup Page 
* Fixed #22852: shopping cart price rule - search by ID - error page 
* Fixed #15897: Unsubscription Email Sender in the Newsletters Subscription Options is not working correctly
* Fixed #15899: Newsletters subscription confirmation in not working
* Fixed #22908: Grid Serializer doesn't handle dropdowns as edit columns
* Fixed #22946: 'Products Tagged by Administrators' grid contains information about product that is assigned by the customer
* Fixed #22935: Issue with Google AdWords and DSMM Code 
* Fixed #22910: view of system/design table with no records under IE 8 
* Fixed #22914: view of URL rewrite table with no records under IE 8
* Fixed #22935: Issue with Google AdWords and DSMM Code 
* Fixed #22536: Light-weight email templates 
* Fixed #23017: Memcache session fallback does not work
* Fixed #22992: Trace appears during create reorder from front-end 
* Fixed #22991: Cannot add items to shopping cart after active 'Use Flat Catalog Product' 
* Fixed #22813: Google base Undefined Offset when Managing attribute mapping
* Fixed #23138: URL rewrite error on product creation
* Added Regions for baltic states and Finland
* Fixed #23092: Memcached and compiler
* Fixed #19804: sorting/searching by "inventory" field
* Fixed #23241: Catalog price rule not correctly appy for customer group
* Fixed #16294: WSDL missing attributes for customerCustomerEntity
* Fixed #22851: Used wrong resource model for api/user
* Fixed #18207: SOAP-ERROR: Parsing Schema: can't import schema from 'http://schemas.xmlsoap.org/soap/encoding/'
* Fixed Fatal error: Call to undefined function eaccelerator_fetch()


==== 1.4.x-devel-83018 ====

== Fixes ==
* Fixed Opening bestseller product (admin/dashboards) results in adding new product
** fixed case when dashboard shows report for non-existing product (i.e. deleted one)
* Fixed Bestsellers statistic bug
** removed NULL values from statistic tables and changed foreign keys to cascade deleting stats for deleted products
* Fixed Gift message displaying conditions not properly work on frontend and backend
* Fixed QTY of product is incorrectly showed in Customer's Current Activities - Shopping Cart and Customer's Shopping Cart.
* Fixed Gift message displaying conditions not properly work on frontend and backend - fixed missed bracked
* Fixed Magento Connect Manager -> No warning message
* Fixed Unable to upload community extention in Magento Connect Manager without Community Channel installed
* Fixed Bundle product price calculated not correctly
* Fixed Customer's email doesn't escalate to billing/shipping addresses
** added copying email field from quote address to order address
** added sending email to PayPal, when user's address doesn't contain email info

==== 1.4.x-devel-82478 ====

== Improvements ==
* Added "Switch/Maestro" card type support to centinel 3DS validator. Added comment about maestro and 3d-secure to paypal system config
* Added more flexible filters implementation in collections:
** Varien_Data_Collection::addFilter() registers filters as objects and implements getFilter() method to be able to detect/modify already existing filters
** Varien_Data_Collection_Db::_renderFilters():
*** Added a hook _renderFiltersBefore()
*** Implemented 'public' filter type, which maps the provided filter field from public into internal view and passes the "value" as a condition through _getConditionSql()
** Added $this->_renderFilters() call to abstract EAV collection to accommodate the filters that may be set by addFilter() method
* Added ability to pass multiple recipient emails and names to Mage_Core_Model_Email_Template::send()

== Changes ==
* Refactored shipping rates calculation to keep process solid and do not try to recreate internal process of calculation, as it was
* Added caching of requests to shipping carriers, because otherwise we get too much duplicate requests during calculation of every shipping method
* Refactored "Special products" RSS feeed

== Fixes ==
* Fixed Catalog-specific attribute options do not load when using through catalog/output helper
** method _getLoadDataFields at product attribute resource collection modified to select additional needed fields;
* Fixed saving attribute value in store view scope only
* Fixed Not searchable attributes are searched by Quick search.
* Fixed Customers won't appear in the search results on the customer grid in the admin
* Fixed Huge memory consumption on flat shipping rates import
** decrease to 5000 count of data wich inserts into DB in one iterate, to avoid exceed of 128M memory_limit
* Fixed Config fields "Disable output" doesn't implement inherited value
* Fixed Category created for some store view not displayed on frontend
** include_in_menu attribute was made as required to set default value when category created in specified store
* Fixed creating of  "Shopping Cart Price Rule'
** setActualProductAttributes method was called with 'attribute_set_id' value in $attributes param. But it does not exist in 'eav/attribute' table. So we need to check it
* Fixed PayPal PE transaction_id detection: Overrided getPaypalTransactionId method in PE API -  changed transaction id getting to process payflow accounts not assigned to paypal side
* Fixed Configurable Product Catalog Price Rule Issue: the main idea is to calculate price rule on configurable price separately from base price
* Fixed fatal error during import large file
* Fixed Shipping information is not displayed in backend after Google Checkout operations
* Fixed Field Mapping Issue during customer import
* Fixed CMS blocks grid inoperable with store filter in GWS-limited mode
* Fixed incorrect qty increment behaviour
** qty increment not decimal validate
** when adding product with qty increment to cart - redirect to product's page
** generate message about mismatch of qty increment when editing item qty at cart
* Fixed ups/usps and Guam
* Fidex issues with attaching product to multiple stores: refresh product index query update
* Fixed displaying of bundle product weight
* Fixed "Select a PayPal Solution" checkbox bug: Website Payments Pro and  Website Payments Pro Payflow Edition consider each other status in their checkboxes control logic
* Fixed Invoice Comments Stripped When Quantities Updated
* Fixed XSS security issue on frontend

==== 1.4.x-devel-81496 ====

== Improvements ==
* Backordered Item Status for subitems in Orders
** Added correct message at order for all backordered items. At back-end all items shows as backordered if their quantity is below or equal to zero
** Fix of duplication backorder messages for composite product options with same backordered item - saving backorder messages per product id
* Magento Connect Manager
** checking cyclic dependency references and conflicts with local files
**  implemented adding to MCM manually installed extension
** changed upgrade logic, previous version of package should be deleted before install new
** Implemented new download process and dependencies rules
** Added correct behavior during extension reinstall, so dependencies will not reinstall automatically

== Changes ==
* Shortened the names of all foreign keys longer than 49 characters

== Fixes ==
* Fixed Google Chekout: Discount for shipping amount doesn't apply
* Fixed XSS issue in address form
* Fixed Address in the customers address book cannot be deleted
* Fixed CatalogSearch_Fulltext not being renewed for configurable products when editing attached simple products
* Fixed Google Checkout: shipping method info is empty at order page in admin backend
* Fixed Google Checkout: with discounted shipping - discount is applied again
* Fixed Wrong timezone/DST in reports
* Fixed coupon_code attribute inconsistency in some upgrade paths (from 1.4.0.0 to 1.4.1.0)
* Fixed  Created extension archive through Magento Connect include ".svn" directories
* Fixed version of downloader
* Fixed Magento Connect: User should has a possibility to choose version for extension upgrade
* Fixed Magento Connect: User shouldn't be able to download Magento into "0000 permissions" folders
* Fixed Magento Connect: JS validation is absent for "Authors" tab on  package extensions page
* Fixed Magento Connect: Saving information on settings page
* Fixed Magento Connect: "Configuration" step - server validation is absent during installation
* Fixed Magento Connect: "Log in" page - Message or some information about required fields doesn't appeared
* Fixed Magento Connect: "Configuration" step - incorrect message appeared during installation
* Fixed wrong shipping price in case of sales rule with fixed cart discount and 1 item in cart
* Fixed the label for the configurable product attribute does not reflect correctly on the frontend
* Fixed sales rule with fixed discount for whole cart doesn't work

==== 1.4.x-devel-80991 ====

== Improvements ==
* Optimized rewrite selection from DB, added url rewrite and suffix validation at admin backend
* Added verification of access level for app/etc/local.xml. 
** Now if server configuration has issue and this file accessible from browser admin user gets notification in backend.

== Changes ==
* Compilation scope for some EAV models which was causing blank page after enabling compilation

== Fixes ==
* Fixed "Slash for category or product urls causes error 404" 
* Fixed Shared shopping cart on the stores with different domains
** check origin url in all store urls
** prevent to getting SID param from current query
* Fixed #18454: Import profiles do not reset websites values
* Fixed Issue with zero grand total express checkout for recurring products.
* Fixed "Allow Gift message" setting on the product page doesn't work in Front.
* Fixed "Duplicate" of bundle product leads to an error
* Fixed Catalog sitemap for categories shows inactive sub categories if flat catalog enabled
* Fixed Added support of all product attributes in conditions/actions of salesRules.
* Fixed Disabling product attribute usage in promo rules not affect existing promo rules
* Fixed "Cart Price Rule not working with Product Attributes" (boolean values not properly shown in rule conditions)
* Fixed Wrong amounts invoiced with FPT
* Fixed Wrong order status after refund and additional related issue on frontend during checkout
* Fixed Unable to delete uploaded sample for downloadable product
* Fixed Paypal Direct send wrong billing address to API
* Fixed Incorrect viewing of category settings after refreshing page
* Fixed Catalog price rule discount not working during backend order creation
* Fixed Double headers for session cookie set

==== 1.4.x-devel-80262 ====

== Improvements ==
* Upgraded Zend Framework to version 1.10.8
* Added the Recurring Profiles tab in customer management

== Changes ==
* Deleted Mage_Sales_Model_Recurring_Profile_Info, which was not on its place and added accidentally
* Category and product design settings inheritance logic

== Fixes ==
* Fixed Custom design is not reset properly after shipment comment emails
* Fixed Tax report displays incorrect figures
* Fixed Removed invoice creation on "completed" IPN message with payment_entity = "auth" to prevent double capture creation on single transaction with IPR.
* Fixed Image browser in WYSIWYG editor doesn't fill mouse over/out fields
* Fixed Added rounding to "Refund Shipping" field on credit memo creation page.
* Fixed Added additional error messages to customer address validation on PHP side while creating.
* Fixed "No server side check for password length when customer edits his account information" 
** Also added proper processing for password == '0', earlier it was considered as non-set password
* Fixed WYSIWYG editor breaks directives that are not in src attribute
* fixed directives decoding for a case when the secret key is present in URLs
* Fixed Duplicate of a product creates it with no SKU value and is saved
* Fixed Redundant catalog product attribute "category_ids" remains during upgrade from 1.3 to 1.4
* Fixed Reports/Shopping cart/Products in carts optimization
* Fixed "If all Storeviews value set up - disabled --> Front end shows default storeview instead of 404 page"
* Fixed Added error on zero subtotal checkout with paypal express. Removed paypal express button on shopping cart with zero grand total.
* Fixed Field labels and field values are not aligned vertically on Sales Orders in Admin
* Fixed Spacing between field labels and field values is inappropriate on the Recurring Profiles tab in My Account section
* Fixed Not searchable attributes are searched by Quick search.
** Checking if attribute used in quick search before adding to fulltext field
* Fixed Mage_Customer_Model_Customer::getGroupId can't return zero value
* Fixed #23184: Huge memory consumption on flat shipping rates import
* Optimized and refactored Table Rate import
* Fixed Scrolling during category load results in some js-errors
* Fixed "Javascript alert on "manage category" page"
* Fixed Security Vulnerability on Mage_Core_Block_Template level
* Fixed Merged CSS breaks Secure Pages (https)

==== 1.4.x-devel-79607 ====

== Improvements ==
* Implemented cache for shipping rates and fixing issues with rounding

== Changes ==
* Refactored one routine in Inventory Observer to remove code duplication
* Disabling product attribute usage in promo rules not affect existing promo rules

== Fixes ==
* Fixed SOAP webservices do not work when enabling "Add Store Code to URLs"
* Fixed Incorrect displaying of the Start Date entered by customer while adding to the cart recurring product
* Fixed Downloadable Product "lable" typo
* Fixed While creating gift message from backend it disappears in case of refreshing page
* Fixed Product export fails when the quantity of exported products is 25 000 or more (memory leak in products)
* Fixed While creating gift message from backend it disappears in case of refreshing page
* Fixed Google Chekout: Discount for shipping amount doesn't apply
** onepage checkout recalculates shipping charges after setting the payment method (not solved yet in multishipping)
** added warning about Carrier Calculated Shipping in Google Checkout system configuration
** GC API callback now sets the payment method to quote on requests
** the free shipping calculator now marks the entire address as "free shipping" if all its items have free shipping
* Fixed On wide monitors checkbox "Create Permanent redirect" in admin backend wraps up to the end of input box
* Fixed Tag isn't showed in Product Page and My account->My Tags, if tag are deleted by customer, approved by administrator, added by customer
* Fixed Non standard images make troubles with "Next"/"Previous" buttons
* Fixed There is no validation of the Tracking number field during first time creation of the shipment
* Fixed Missed dollar sign in variable name
* Fixed Incorrect escaping of Mage_Catalog_Model_Abstract::loadByAttribute method
** Zend_DB_Select::where must get null values to skip quoting into $cond empty strings if value is null
* Fixed "URL rewrites duplicating when assigning to root category"
* Fixed Shipping method UPS_XML missing titles
* Fixed The pager is missing for tagged product list
* Fixed Report > Products Ordered ignores Store view switcher
* Fixed Flat catalog index problem after upgrade with customizations present
* Fixed Incorrect bundle items inventory decrements
* Fixed Category and product design settings inheritance
* Fixed Removed fatal error on removing non existent quote item from quote
* Fixed Credit Card Maestro/Solo: The field "Start Date" is not displayed on order information page
** deleted unused Maestro/Solo from Payment module config
** moved Maestro/Switch and Solo card definition from Chronopay to Payment module config
** deleted Meastro/Switch definition with incorrect code MS from Cybersource module config
** fixed logic of showing "Issue number" and "Start Date" of Switch/Solo card on frontend
* Added warning about offline refund
* Fixed Mage_Checkout_Block_Cart_Item_Renderer::getIsInStock bug
* Fixed Fatal on edit configurable product page, if custom required price attribute is used
* Fixed #0011135: View invoice error with changed query string
* Fixed Trailing semi-colon displayed on Profile Export page
* Fixed New Orders & Other Authenticated RSS feeds should use HTTPS
* Fixed Dataflow export products sku filter works as not "starts with", but "like"
* Fixed Removed default shipping address assign on paypal express checkout
* Fixed The customers from Puerto Rico can't pay with PayPal (Express Checkout in PaypalUk)
* Fixed Shared shopping cart on the stores with different domains
* Fixed Discount amount for the whole cart divide proportionally between all affected items according to their base price and then applied.
* Fixed Removed store selector in single store mode on url rewrite edit page
* Fixed Javascript validator's translation strings missing
* Fixed Quick Search Autocomplete does not work via ajax http protocol for https page
* Fixed Inventory->Qty Increments - unable to add
* Fixed Loading search query performance issue
* Fixed Changed labels in checkout and payment information blocs for credit cards Solo Maestro Switch 
* Fixed Product q-ty doesnt decrease after google checkout
** added same 'checkout_submit_all_after' event to  AmazonPayments
** removed 'TODO' notice from Multishipping Checkout, because current scheme is better and will not be influenced by any Multishipping refactoring
** fixed Observer reaction on 'checkout_submit_all_after' to include needed reindexing
* Added checkout_multishipping_controller_success_action and checkout_onepage_controller_success_action events that pass the created order ids on frontend checkout success actions
* Fixed Google Analytics tracking pages with wrong URI:
** Completely reimplemented googleanalytics/ga block:
*** it doesn't depend on session/quote, but just uses order_ids, if passed
*** the page_name parameter is reimplemented as it was intended to be: an optional parameter that can be customized via layout for certain actions
*** moved out the integration part with google checkout to observer
*** eCommerce tracking passes shipping address instead of the billing address, if available
*** replaced the "affiliation" into store frontend name in eCommerce tracking (as it is intended to be)
*** eliminated passing order item "category" in eCommerce tracking (that never existed)
*** optimized javascript code of GA with Google Checkout integration
** Eliminated mutual code coupling between Google Analytics and Google Checkout modules
** Improved integration of Google Analytics and Google Checkout:
*** the GA integration should appear only when GC buttons are available
*** there will be no integration when there is no GA tracking code configured
*** the GA/GC integration seems like wasn't working because there was no pageTracker js variable accessible to the GC scripts
* Fixed Wrong links in backend to "New Products/Low Stock/Customer reviews" RSS feeds
* Fixed "Send auto-generated password" generates e-mail with incorrect template
* Fixed Unable to refund Credit Memo because of Shipping Rounding
* Fixed Added custom option info to recurring profile info page on frontend and backend.
* Fixed Product Visibility and Status disappear when in search
* Fixed Removed validation of new customer shipping address on backend for orders with virtual products only 


==== 1.4.x-devel-78617 ====

== Improvements ==
* Design packages and themes optimization/refactoring/improvements:
** minor improvements and fixes
** improved upgrade-ability of CE themes
* iPhone Theme Refactoring
* Added Widget settings sharing between widget types
* For Invoices, Shipment, Credit Memos added possibility to show admin comments at user frontend (checkboxes "Visible on Frontend" in admin interface)
** Added JS to enables/disable checkbox 'Append Comments' depending on checkbox 'Email Order Confirmation'
** Refactored invoice/shipment/refund comments collections models to one abstract Comment Collection Model
** Refactored Block Order Invoice/Shipment/Creditmemo comments to usage of common block and design - Block Order Comments
* A little more accurate profiler - important for very quick measurements
* Add Shopping Cart API
* Implementing payment refund notifications
* Added website price scope for bundle items
* Added support of pending transaction to payflow pro. Also fixed "denied payment review" message in payment

== Changes ==
* Refactoring validation states for Centinel
** Added template method Mage_Centinel_Model_StateAbstract::isLookupSuccessful
* Add boolean type for catalog price rules and condition for category_ids
* Removed Maestro/Switch/Solo card from system. Added Maestro/Switch and Solo cards to Chronopay and Cybersource methods
* Mage_Adminhtml_Block_Sales_Order_Creditmemo block had dependence from 'canCapture' 'canCapturePartial'. It was changed to 'canRefund' 'canRefundPartialPerInvoice'. For set result of Mage_Adminhtml_Block_Sales_Items_Abstract::CanEditQty`s we can use setCanEditQty
* Added Maestro/Switch and Solo Dollars card types for paypal_direct payment method. Also removed Maestro/Solo/Switch card type for this method
* Removed "Shipping address" block on recurring profile view page if product is virtual. Also fixed virtual order detection
* Refactored PayPal cart line items and cart totals calculation to accommodate various discounts and tax settings
** added hidden discount and hidden shipping taxes to the calculation
** eliminated cart line items logic from the helper, moved it to the paypal/cart model
** simplified transferring of the totals and line items to PayPal API objects
* Refactored sales rule discount detection on "buy_x_get_y" rule type
* Added catalog_product table definition to product review collection
* Changed type of obscure input field to 'password', so this field is hidden even when user enters data in it
* Removed dependence to payment method on getting billing agreement method title. For now payment method title stored in billing agreement
* Removed invoice creation thought zero subtotal checkout with new order status "pending"

== Fixes ==
* Fixed ability to buy Product which have status "Out of Stock" through a direct link on button "Checkout with PayPal"
* Fixed All free shipping methods in absent in Transfer Shipping Options menu on PayPal side
* Fixed Payment methods titles for the PDF prints through admin gets from default config instead of the storeview config
* Fixed PayPal and Puerto Rico shipping address
* Fixed "Transfer Shipping Options" pass on PayPal side not correct value for Flat Rate method
* Fixed Centinel JCB validation test cases 8-9
* Fixed Saving caterory in store view scope
* Fixed Attribute upgrades moved from 1.4.0.0.15 to 1.4.0.0.33
* Fixed that product tagged by administrator has wrong URL at front-end
* Fixed refusal from Card Verification (through link Exit), does not allow to place order repeatedly
** If lookup was filed and customer tries again we will do new lookup.
** If lookup was success and customer tries again without some changes we will not do new lookup
** If authentication was filed and customer tries again we will do new lookup and authentication
** If authentication was success and customer tries again without some changes we will not do new lookup and authentication
* Fixed #22536: Light-weight email templates. Wishlist share email fix
* Fixed declaration of Mage_Cybersource_Model_Api_ExtendedSoapClient::__doRequest() compatibility with SoapClient::__doRequest()
* Fixed Two registration emails from a wrong store and without a logo are sent when a customer is created in Admin panel
* Fixed Reindex for bundle products with date fields
* Fixed Status is "Ready" instead to be "Reindex required" then creating new subcategory in mode "Manual Update"
** index status changed to STATUS_REQUIRE_REINDEX when search engine changes
* Fixed #23321: Wrong type casting in method
* Fixed Print-All Includes Tracking # from All Shipments on Every Shipment
* Fixed Ignored 'Include in Navigation Menu' category option with enabled flat catalog.
* Fixed Admin unable to add Image through WYSIWYG to description and Short description without intermediate product saving
* Fixed QTY decrement after multishipping
* Double clicking adds product to cart twice
* Fixed Catalog Price Rule(for NOT LOGGEN IN customers) is not applied for shopping cart and while checkout as guest or while first registration.
* Fixed Payment methods titles for the PDF prints through admin gets from default config instead of the storeview config
* Fixed Mage_Adminhtml_Model_System_Config_Backend_Serialized::_afterLoad() does not check input for unserialize()
* Fixed Sending letters through "Contact Us" form, leads to error
* Fixed PayPal Express with Flat Rate: incorrect counting Shipping amounts per order
* Fixed Saving attribute value in store view scope only causes data loss.
* Fixed #22607: Dispose of Mage_GiftRegistry module
* Fixed Related products are not saved when you attach them to a product
* Fixed Added qty to bundle unit price calculation to quote totals recalculating.
* Fixed Saving category cause: 'Exception' with message 'File was not uploaded.' in /home/vadim.kusakin/dev/qa/2759/lib/Varien/File/Uploader.php:139
* Fixed Fixed Magento Connect -> MCM -> If agreement checkbox is unchecked, "Continue" button should be disabled
* Fixed Set the same column font size as in cells in PDF documents printing
* Fixed Home page appears instead of predefined 404 page
* Fixed Removed converting of "is one of" and "is not one of" values in decimal.
* Fixed Wrong column type for order_increment_id on Invoice, Shipments, Creditmemo grids
** order_increment_id was setted as "text" instead of "number" type
* Fixed Inconsistency with credit memos showing buttons online vs offline
* Fixed PayPal Express shortcut is missed on product page
* Fixed An email is sent to a customer after its profile is edited in the Admin panel
* Fixed that Payflow Pro includes only the first line of billing/shipping addresses into request
* Fixed Incorrect showing of product page when inputing a product description with table which have attribute align = left
* Fixed Wrong link for bestsellers in admin dashboard. Grids.php fixture doesn't do anything for this bug - just to beautify code.
* Fixed Added fixes to reports - base_discount_amount is actually kept negative in DB.
* Fixed Empty dropdown 'status' at the creation New Review Grid.
* Fixed Incorrect work of "Recently Compared Products" functional on category's page
* Fixed behavior when having single store, javascript raises exception and all followed code is not executed
* Fixed that Special price for dynamic bundle applies twice
* Fixed #21960: Labels in page/html_wrapper and core/text_list in layout 
* Fixed GUI bugs on Recurrent Profile frontend part
* Fixed Magento Connect -> Message about invalid URL is duplicated
* Fixed that suspend Recurring Profile from front side leads to error
* Fixed Missing pager for tagged product list
* Fixed Wrong profiler output for getUrl in Category
* Fixed Saving of billing agreement relation with order - added force billing agreement re-saving and fixed isValid method in agreement detection.  
* Fixed Incorrect sort order reliable on mysql internal order during eav attribute load
** move prepare select to separate method
* Fixed passing additional totals to PayPal when cart line items are disabled:
** simplified paypal/abstract api to just set the paypal/cart instance and the needed configuration settings
** moved workarounds of setting shipping and discount totals as line items into the appropriate APIs: WPS and NVP
* Fixed In My product Review short description HTML tags are shown
* Fixed that Refund from google chekout don't display on the order in Magento
* Fixed that "Compare Products" block does not appear on the category page and product page
* Fixed Non-existing attribute's source model causes fatal error
* Fixed Varien_Db_Select memory leak


==== 1.4.x-devel-77975 ====

== Improvements ==
* Upgraded Zend Framework to version 1.10.5
* Upgraded TinyMCE to v.3.3.7
* Added to prototype validation by length min-length validation
* Added Varien.DateElement for front-end date form fields and re-implemented Varien.DOB
* Added functionality to disable dashboard charts in backend (System > Configuration > Admin > Dashboard)
* Added functionality to disable dashboard charts during installation
* Adminhtml W3C Validation improvements
* Added ability to use session save method from configuration

== Changes ==
* Removed SID from url generation when Use SID on Frontend option is disabled
* Added customer session validation for loadCustomerQuote method
* Iphone clears.css has been deleted

== Fixes ==
* Fixed #18569: Gift Messages not in OrderInfo returned array
* Fixed PayPal API credentials wizard popup size
* Fixed #11449: customer_id is mismatch with entity_id in customer.create
* Fixed merging CSS-files with different skin domain to pick a proper base URL
* Fixed Bad UI style on checkout success page
* Fixed buying more than 1 virtual product in multishipping checkout
* Fixed #22518: Wrong amount for second refund
* Fixed #22776: Bug Causing Recursion Error
* Fixed #22668: Incorrect reports for coupons
* Fixed Products -> Product with "Out of stock" status displayed on frontend, but shouldn't
* Fixed Password miss match for newly created in Back end customer
* Fixed "There has been an error processing your request" page is displayed when specified order status is selected on Reports->Sales->Tax page
* Fixed bug with 'Use Flat Catalog Category'
* Fixed #13770, #16300, #21040 : Product Media Api Broken, product_media.create API overwrites image itself each upload, product_media.update API does not upgrade the image itself
* Fixed #16306: Webservice with htaccess (changes in code style)
* Fixed #22536: Light-weight email templates 
* Fixed #18935: Soap api v2 multiple complexFilters with the same key
* Fixed incorrect Window titles on frontend
* Fixed Eliminated display currency usage (instead of the base website currency) in shopping cart price rule conditions
* Fixed #21146: Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
** corrected syntax mistakes
* Fixed batch of issues related to google checkout:
** Invoice don't create automatically with Google Checkout
** Google checkout invoice duplication
** Automatically authorize the buyer's credit card for the full amount of the order
** Refund from google checkout don't display on the order in Magento
** Google Chekout: Discount for shipping amount doesn't apply
** Different order amount in Google checkout and Magento orders
** Applying of discount for shipping, when using google checkout
** Order is in google sandbox doesn't contain gift card
* Fixed #23461: Wrong attribute value in catalog link widget XML
* Fixed getting complete state for orders with zero grand total when processed
* Added Store id param to billing agreement entity.  Also fixed store setting in billing agreement payment method.
* Fixed #22575: Trace error during using filter "Products" on Tags page
* Fixed Grids with settings remain active while disabled PayPal methods
* Fixed configuration merger fatal error when store/website resource structure is inconsistent
* Fixed PayPal admin setup: checkbox problem
* Fixed Adding shipping address transferring on non guest checkout in Paypal Standard
* Fixed "Save in address book" checkbox in the Shipping address area doesn't work while admin order creation
* Fixed pre-selecting default address during checkout
* Fixed Email with empty password is sent to a customer after an order is created in the Admin panel
* Fixed Necessary to add data validation for filed "Trial Billing Frequency" in Recurring Profile
* Fixed "Out of Stock" product is possible to purchase successfully through Shortcut button
* Fixed phpdocs in lib/Varien and removed junk file


==== 1.4.x-devel-77328 ====

== Improvements ==
* Rendering customer attributes
* Added favicon manager under System > Configuration > Design > HTML Head

== Fixes ==
* Fixed #21146: Magento falls into the white screen when saving URL rewrite for a product on the Default Store View
* Fixed #21643: Fixed "wsdl" parameter validation for Soap V2
** Changed class SoapServer with class Zend_Soap_server
** Added ability to set response charset from admin panel: System->Configuration->Magento Core API
* Fixed #21499: Default billing and shipping address
* Fixed #21565: missing "comment" for salesOrderStatusHistoryEntity
* Fixed #20481: Access Control List not retrieved for API user for resources() and resourceFaults() operations
* Fixed #18367: FCGI Error on WSDL Url with Apache and mod_fastcgi
* Fixed #22053: use HTTP 301 code instead of 302 in case of web/url/redirect_to_base
* Fixed #20654: Admin order creation->Move mouse cursor isn't changed into hand while move it on some product for adding 
* Fixed #21590: Attribute 'Date': testing for uniqueness fields not working
* Fixed #21566: Type of attribute 'Price': Possible to add text value for field 'default value'
* Fixed #22053: added optional behavior (301 or 302)
* Fixed #21570: Review from not logged in user is saved in list of All Reviews when "Allow guests to write reviews = No"
* Fixed #22090: Different values of Qty Increments during create and after duplicate products
* Fixed #22489: Eliminate difference between bundle.js in different skins 
* Fixed #22419: Set default stock_data if not exist in create/update product
* Fixed #20227: "Review(x)" link should be added to the compare page.
* Fixed #21570: Review from not logged in user is saved in list of All Reviews when "Allow guests to write reviews = No"
* Fixed #20959: Locale problem in shipping tracking popup raises exception 
* Fixed #21955: Layout cache ignores product column count update
* Fixed #20011: After using filter "Color" or "Manufacture" in Configurable Product meaning from column is disappear
* Fixed #21908: Incorrect attribute ordering in "Compare products" page.
* Fixed #22222: Edit review-> if browse stores in the "Visible In " drop-down, rating values reseted 
* Fixed #22075: Product Attribute title specified for StoreView isn't showing on the configurable product's page
* Fixed #22605: catalog_category.level return root categories when website or store are null
* Fixed #21806: Different values display on the shopping cart in front-end and back-end 
* Fixed #20113: Shipping address display as default on the front-end and as not default on admin for one customer 
* Fixed #22575: Trace error during using filter "Products" on Tags page
** added 'filter_index' to array parameter in addColumn() method call
* Fixed #14591: Incorrect SKU for Configurable Product with Custom Options 
* Fixed #22476: Blank Column in Related Products Grid
** deleted duplicate <col> output for editable columns
* Fixed #22575: Trace error during using filter "Products" on Tags page
** apply filter_index field values to index
* Fixed #22644: A discrepancy between GT(Base) and GT(Purchased) 
* Fixed #22645: Incorrect original price when using custom price in order. 
* Fixed #22653: Missed checking for file existents in JS/CSS merger
** cheking in source file exists. If not - do not check last modification and force to merge target file again
* Fixed #22594: Unable to place orders through checkout with multiple addresses with PayPal direct + zero subtotal for one order 
* Fixed #21185: Newsletter confirmed automatically BEFORE account email is confirmed. 
* Fixed #22167: "Add new row" button in downloadable product 
* Fixed #21952: BUG - Category / Url Model (UYN-886991) 
* Fixed #15334, #17794
** API category did not pass validation process due to available_sort_by must be ArrayOfString
** Added category validation for backend (missed)
** Creating separate validation for available_sort_by and default_sort_by attributes
* Fixed #22599 Upgrade from 1.1.8 to 1.8.0.0 database compatibility issues (PARTIAL)
* Fixed #22661: 1 cent bug 
* Fixed #22434: 100% discount of products -> the amounts of Tax and Grand Totals are or negative or not corectly 
* Fixed #10073: Unnecessary option for downloadable products
* Fixed #20014: Qty use decimals for downloadable
* Fixed #22164: Incorrect message for maximum shipping amount
* Fixed #22174: Custom 'Qty to Refund' isn't remembered after message about incorrect amount
* Fixed #22182: The value of 'Customer Since' field to duplicate clients at different sites.
* Fixed #22243: Add new review by admin->type of this review is 'guest', but should be 'administrator'
* Fixed #22313: Time of order creation if not displayed by the "Order Created At (datetime)" template variable.
* Fixed #22348: "Add to card" button is absent for giftcard product in the catalog
* Fixed #22640: Creating customer unable after adress tab manipulations
* Fixed #22670: Credit memo - incorrect shipping price displaying
* Fixed #22798: Excl and Inc. Tax don't display on the Estimate Shipping and Tax block
* Fixed #20088: Admin able to push on-line refund button for the capture off-line invoice
* Fixed #16306: Webservice with htaccess. Added server authorization (.htaccess)
* Fixed #22266: HEADERS ALREADY SENT Error during dataflow import
** Additionally: moveing layout update in separate layout file of dataflow module.
* Fixed #21412: The "Save Attribute" and "Save and Continue Edit" buttons become disabled after saving attribute with attribute code that exists
* Fixed #22844: After login to admin got 404 instead Startup Page 
* Fixed #22852: shopping cart price rule - search by ID - error page 
* Fixed #15897: Unsubscription Email Sender in the Newsletters Subscription Options is not working correctly
* Fixed #15899: Newsletters subscription confirmation in not working
* Fixed #22908: Grid Serializer doesn't handle dropdowns as edit columns
* Fixed #22946: 'Products Tagged by Administrators' grid contains information about product that is assigned by the customer
* Fixed #22935: Issue with Google AdWords and DSMM Code 
* Fixed #22910: view of system/design table with no records under IE 8 
* Fixed #22914: view of URL rewrite table with no records under IE 8
* Fixed #22935: Issue with Google AdWords and DSMM Code 
* Fixed #22536: Light-weight email templates 
* Fixed #23017: Memcache session fallback does not work
* Fixed #22992: Trace appears during create reorder from front-end 
* Fixed #22991: Cannot add items to shopping cart after active 'Use Flat Catalog Product' 
* Fixed #22813: Google base Undefined Offset when Managing attribute mapping
* Fixed #23138: URL rewrite error on product creation
* Added Regions for baltic states and Finland
* Fixed #23092: Memcached and compiler
* Fixed #19804: sorting/searching by "inventory" field
* Fixed #23241: Catalog price rule not correctly appy for customer group
* Fixed #16294: WSDL missing attributes for customerCustomerEntity
* Fixed #22851: Used wrong resource model for api/user
* Fixed #18207: SOAP-ERROR: Parsing Schema: can't import schema from 'http://schemas.xmlsoap.org/soap/encoding/'
* Fixed Fatal error: Call to undefined function eaccelerator_fetch() 



==== 1.4.2.0-beta1 ====

=== Major Highlights ===
* Included new Magento Connect Manager 2

==== 1.4.1.1 ====

=== Changes ===
* Checkout: added dispatching event 'checkout_submit_all_after' into all checkout models
* Centinel: changed event for resetting validation state 
* Added check for Order ID before try to lookup transactions by Transaction Id
* Added cvv field for Mastero/Switch/Solo cards. Also fixed html formatting.
* Re-factored saving relation of billing agreement with order.
* Added Qty Increments update in products mass-update.
* Added ability to update filter map in Varien_Data_Collection_Db
* Added comment about American Express cards in PayPal system configuration (http://www.paypal.com/amexupdate).

=== Fixes ===
* Fixed Tax calculation for Downloadable product in purchase it through PayPal Express Checkout
* Fixed "Notice: Undefined property: Mage_Catalog_Model_Template_Filter::$_useAbsoluteLinks " when you use WISIWYG Editor for field "Description"
* Fixed Website PayPal Standard payment method is not working with Reward Point, Store Credit and gift Cards
* Fixed Multiple address checkout with PauPalUK direct + 3d secure validation. Payment information error. Please start over.
* Fixed Fatal error onBilling Agreement Related page with applied filters
* Fixed The product's "Stock Status" is not changed from "In Stock" to "Out of Stock"
* Fixed Qty of the product continues to decline when the "Decrease Stock When Order is Placed" is set to "No"
* Fixed If set "Manage Stock" to "No": Qty decreasing when product is ordered
* Fixed The bottom part of the list "Payment Method" in SCPR has too much free place
** if title of Payment Method is empty, get it from overloaded configData('title') method of concrete Payment Method class
** rework. Delegate to Mage::helper('payment')->getPaymentMethodList method for retrieve all payment methods
** fixed by used new config features in 1.4.1 ver - <config_path> in system.xml
** delete getConfigData method
** add config_path with 'payment' section to each field in system.xml
** in sql-upgrade change path to 'payment' section in core_config_data table
* Fixed tax calculation in case Unit Price Tax with settings applying customer tax "After Discount".
* Fixed Solo cards JS validation. Added expdate field to solo and maestro cards. Also removed some duplicates in credit card IIN ranges.
* Fixed Maestro/Switch/Solo cards js validation on payment form: Added additional issue_number and issue_date checks.
* Fixed fatal error in catalog/shopping cart rules based on recently deleted attribute.
* Fixed incorrect redirect after order placing failed, during second try of order placing.
* Fixed exception when "Created At" filter used on Transactions page.
* Fixed incorrect redirect during multishipping checkout as guest.
* Fixed issue with updating qty and addresses during checkout with multiple addresses which resets shipping address to the default billing address.
* Payflow pro:
** "Sale" action does not work.
** Missed transaction ID on fraud services filter triggered.
** Sub-standard order processing flow control and verbosity.
** Inappropriate "state" passed to the gateway in the order addresses.
* Fixed centinel JCB validation.
* Fixed #14885: Unable to upload products into GoogleBase.
* Fixed issue with creating credit memo for partial capture online invoice for the order witch where placed through Website Payments Pro (Payflow Edition) Payment method.
* PayPal: fixed grammar in payment form/redirect text messages (EC, WPS)
* Fixed: Subscribe to Order Status at the front end causing Fatal error: Call to undefined method Mage_Sales_Model_Mysql4_Order_Invoice::getDefaultAttributes() in app/code/core/Mage/Eav/Model/Config.php on line 438
* Fixed fatal error when a configured payment method doesn't exist anymore
* Fixed fatal error: Call to a member function getError() on a non-object in app/code/core/Mage/Shipping/Model/Shipping.php on line 143
* Fixed syntax error caused by accidental manual conflict resolving in Mage_Api_Model_Server_Adapter_Soap
* Fixed qty increments checking business logic for bundle products
* Fixed Mage_Sales_Model_Mysql4_Order_Collection::addFieldToSearchFilter() to be compatible with flat sales structure
* Fixed salesOrderList() broken API call
* Fixed #18534: order_increment_id empty with api salesOrderInvoiceInfo
* Fixed missing files and typo in Mage_Sales_Model_Order::prepareShipment() method described at http://www.magentocommerce.com/boards/viewthread/195761/P0/#top
* Fixed adding tracking for sales_order_shipment.create API call; fixed #17820: Api v2 Shippment create not working
* Fixed upgrading Sales module from backported 1.3 to 1.4: copied 0.9.38-0.9.39 upgrades to 1.3.99-1.4.0.0

=== Known Issue ===
* Google checkout notification duplicates orders or double-process them on timeouts



==== 1.4.x-devel-73934 ====

=== Changes ===
* Re-factored saving relation of billing agreement with order.
* Added Qty Increments update in products mass-update.

== Fixes ==
* Fixed tax calculation in case Unit Price Tax with settings applying customer tax "After Discount".
* Fixed Solo cards JS validation. Added expdate field to solo and maestro cards. Also removed some duplicates in credit card IIN ranges.
* Fixed Maestro/Switch/Solo cards js validation on payment form: Added additional issue_number and issue_date checks.
* Fixed fatal error in catalog/shopping cart rules based on recently deleted attribute.
* Fixed incorrect redirect after order placing failed, during second try of order placing.
* Fixed exception when "Created At" filter used on Transactions page.
* Fixed incorrect redirect during multishipping checkout as guest.
* Fixed issue with updating qty and addresses during checkout with multiple addresses which resets shipping address to the default billing address.
* Payflow pro:
** "Sale" action does not work.
** Missed transaction ID on fraud services filter triggered.
** Sub-standard order processing flow control and verbosity.
** Inappropriate "state" passed to the gateway in the order addresses.
* Fixed centinel JCB validation.
* Fixed #14885: Unable to upload products into GoogleBase.
* Fixed issue with creating credit memo for partial capture online invoice for the order witch where placed through Website Payments Pro (Payflow Edition) Payment method.

==== 1.4.x-devel-71052 ====

=== Fixes ===
* PayPal: fixed grammar in payment form/redirect text messages (EC, WPS)
* Fixed: Subscribe to Order Status at the front end causing Fatal error: Call to undefined method Mage_Sales_Model_Mysql4_Order_Invoice::getDefaultAttributes() in app/code/core/Mage/Eav/Model/Config.php on line 438
* Fixed fatal error when a configured payment method doesn't exist anymore
* Fixed fatal error: Call to a member function getError() on a non-object in app/code/core/Mage/Shipping/Model/Shipping.php on line 143
* Fixed syntax error caused by accidental manual conflict resolving in Mage_Api_Model_Server_Adapter_Soap


==== 1.4.x-devel-70699 ====

=== Changes ===
* Added ability to update filter map in Varien_Data_Collection_Db
* Added comment about American Express cards in PayPal system configuration (http://www.paypal.com/amexupdate).

=== Fixes ===
* Fixed qty increments checking business logic for bundle products
* Fixed Mage_Sales_Model_Mysql4_Order_Collection::addFieldToSearchFilter() to be compatible with flat sales structure
* Fixed salesOrderList() broken API call
* Fixed #18534: order_increment_id empty with api salesOrderInvoiceInfo
* Fixed missing files and typo in Mage_Sales_Model_Order::prepareShipment() method described at http://www.magentocommerce.com/boards/viewthread/195761/P0/#top
* Fixed adding tracking for sales_order_shipment.create API call; fixed #17820: Api v2 Shippment create not working
* Fixed upgrading Sales module from backported 1.3 to 1.4: copied 0.9.38-0.9.39 upgrades to 1.3.99-1.4.0.0


==== 1.4.1.0 ====

=== Improvements ===
* Added ability to use static URLs for media in WYSIWYG or image browser. Added ability to enable parsing {{store}} and {{media}} directives on catalog frontend.
* URL rewrites history: ability to auto-generate custom rewrite with redirect from old to new URL when changing product URL-key
* Added ability to exclude a category from navigation menu
* Various improvements in system configuration UI. Introduced ability to make actual configuration structure to be independent on the system.xml structure
* Added "Only X left" inventory feature
* Implemented Centinel functionality in iphone theme
* Upgraded TinyMCE to v.3.3.2
* Improved PayPal integration, includes:
** Recurring payment profiles entity and purchasing of "subscription" products. In checkout they are treated as "nominal" items.
** Billing agreements
** "Pending Review" order state, "Pending Review" and "Suspected Fraud" order statuses and logic related with this. Triggers by PayPal IPR, FMF and Unilateral payments.
** Functionality of transactions listing/searching and fetching from gateway
** Fetching PayPal settlement reports via SFTP
** Various improvements of PayPal integration on the frontend and admin UI
* Added notice about creating offline creditmemo from order view page.
* Added getter for recurring payment methods in payment helper.
* Implemented abstract block ability to have arbitrary groups of child blocks and a method that returns such a group. Implemented a method that fetches data from child block by specified alias.
* Implemented ability to specify "sort_order" instead of "before" and "after" in the totals declaration. All nominal totals declaration utilize "sort_order"
* Added getter for specified object data by key in core/template block: method getObjectData()
* Defined payment methods grouping, implemented getter for payment method list (with option to group them). Added ability to render grouped options in the "select" grid filter.
** Moneybookers: utilized the payment methods grouping for all its methods; removed redundant "translate" attribute in the methods definition in config.
*** Utilized payment methods grouping for PayPal peyment methods.
* Added more verbosity to PayPal NVP and IPN debugging

=== Changes ===
* Sales module database structure changed from EAV into flat tables
* Product custom URL rewrites redirect to SEF URL, rather than to catalog/product/view/id/
* Reimplemented frontend top menu rendering logic (cross-browser and usability improvements)
* Reviewed [logic of the sales reports|http://www.magentocommerce.com/wiki/doc/sales_reports_specifications]: Orders, Tax, Invoiced, Shipping, Refunds, Coupons
* Reimplemented bestsellers report
* Implemented 3D Secure validation for Maestro International and JCB cards
* (!) Changed Shopping cart methods output (top + bottom): removed <li>-dependance from templates in other modules \-> moved to Checkout module
* Moved the Payflow Pro payment method to PayPal module
* Refactored sales/service_quote model: instead of submit() method the submitAll() should be used. It can submit nominal items separately from the order. The methods for submitting nominal items and order separately - are available as well.
* Refactored onepage checkout model to use the new method sales/service_quote::submitAll(), added recurring profiles and billing agreements passing through the process until the success page
* Utilized child blocks grouping to improve flexibility of rendering additional information in catalog/product/view template. The group is called "detailed_info"; any block from layout may insert itself to this group.
* Removed redundant wrappers hard-coded into some catalog templates. Template of parent block is responsible for wrapping.
* Refactored onepage checkout success block and template: simplified fetching related checkout information, added ability to render billing agreement and recurring profiles that might be created with the payment placement.

=== Fixes ===
* Fixed read/write connection issue during new customer order place. See http://www.magentocommerce.com/boards/viewthread/19363/P0/
* Fixed tax rule ZIP range matching (numeric values were matched as strings)
* Various tax fixes
* Optimized search reindex process

=== Known Issues ===
* PayPal and Payflow pro modules are officially backwards incompatible.
* The `sales_order_aggregated_created` table was re-created with new columns, it is not backwards compatible.

=== Upgrade Path ===
* Once upgraded, go to system configuration section and re-enter all PayPal-related settings carefully. Make sure to specify the proper merchant country and email.




==== 1.4.x-devel-69025 ====

=== Improvements ===
* PayPal integration:
** Settlement reports fetching from SFTP
** Billing Agreements
* Added website and store data to backend model when invoking in system configuration block
* Added "original_data" key to elements when generating system configuration form

=== Changes ===
* Mage_Sales_Model_Order_Payment::canCapture() - move methodInstance::_canCapture before authorization transaction check
* Sales/Payment changes:
** Implemented pending payment review functionality. Includes "Payment Review" order state and statuses "Payment Review" and "Suspected Fraud". In this state the order cannot be fulfilled until the payment is approved.
** Holding orders on pending transactions was replaced in favor of "Payment Review" state. The 'fraud' status was removed from 'holded' order state.
** Transactions resource model unsets the "isObjectNew" if it had a lookup of autoincrement key before saving
** Payment capture and capture notification mark invoice as paid only if needed: when it is pending and the transaction is not pending
** fixed float casting error in Mage_Sales_Model_Order_Payment::_isCaptureFinal()
** fixed showing up credit card type in CC payment block, if there is no credit card type information
* PayPal Instant Payment Review and Fraud Management:
** implemented methods for handling PayPal-specific payment statuses
** added more data importing to payment info in PayPal: payment status, pending reason, "is_fraud_detected"
** added importing of all required for payment processing information in different points of WPP API calls
** implemented IPR and FMF handling for Website Payments Pro methods family (Express Checkout, Direct Payments)
* Fixed PayPal payment info block to not render redundant CC-related information (it extends CC info block)
* (!) Changed Shopping cart methods output (top + bottom): removed <li>-dependance from templates in other modules -> moved to Checkout module
* Added throwing exception on an incorrect attempt of unholding order (TRJ-148987).




==== 1.4.x-devel-68590 ====

=== Improvements ===
  * Implemented serializing/unserializing model fields on abstract level. See Mage_Core_Model_Mysql4_Abstract::$_serializableFields
  * Implemented recurring payment profiles entity and purchasing of "subscription" products. In checkout they are treated as "nominal" items
  * Implemented functionality of transactions listing/searching and fetching from gateway
  * Upgraded TinyMCE to v.3.3.2
  * Added ability to parse "{{media}}" and "{{store}}" CMS directives in the catalog
  * Added ability to insert media content as static URLs in WYSIWYG or media browser mode
  * Implemented "Pending Review" order state, "Pending Review" and "Suspected Fraud" order statuses and logic related with this
  * Added ability to set fieldset always expanded (<expanded> node in system configuration for fieldset)
  * Added ability to set number of "levels up" to form javascript dependencies controller block
  * EAV: implemented a 'serialized' backend model
  * Added ability to separate actual configuration path and form field path in system.xml - use node <config_path>
  * Added ability to render "tooltips" in system configuration fieldsets - use node <tooltip>
  * Enhanced PayPal integration:
    * frontend and backend UI experience of PayPal solutions
    * Instant update API integrataion
    * Recurring payments integration
    * Instant Payment Review and Fraud Management Filters integration
    * EC unilateral payments integration
    * Transactions fetching for PayPal WPP methods

=== Changes ===
  * Reimplemented PayPal system configuration in a dedicated section.
  * Moved Payflow Pro payment method into PayPal module. Got rid of obsolete system configuration fields of this method.
  * Refactored implementation of serializing 'additional_information' field in sales/order_payment, sales/quote_payment and sales/order_payment_transaction
  * Introduced "Is Nominal" term in sales logic:
  * Nominal items participate in catalog, but during checkout and order processing they have zero row total.
  * Implemented separate shopping cart and address totals for nominal items: nominal totals, various changes/adjustments in existing totals
  * Added ability to calculate shipping charges for a quote/address item individually (on code level, utilized by the nominal items)
  * Reviewed credit card types supported by PayPal payment methods
  * Changed skin styles from "tax-total" to more generic "summary-total" (it is used now not only for tax totals, but for nominal items as well)
  * Moved field comments (aka "notes") of the product edit form from the last column under the field element.
  * Varien_Data_Form_Element_Time: added a hidden element with ID to maintain HTML consistency
  * Varien_Data_Form - changed logic of adding suffix/prefix to an element: when element doesn't have a name, the suffix will be result
  * Varien_Data_Form_Abstract and Varien_Data_Form_Element_Abstract: moved adding 'required-entry' class to the element to the moment of its generation instead of the moment of its adding. It adds more flexibility to change properties when the object is not yet rendered.
  * Added to Varien_Data_Collection_Db::_beforeLoad(), moved 'core_collection_abstract_load_before' event dispatching to Mage_Core_Model_Mysql4_Collection_Abstract::_beforeLoad()

=== Fixes ===
  * Fixed #21225: catalogProductUpdate / catalogProductCreate and tier_price attribute
  * Fixed #16596: category.assignedProducts always returns an empty result
  * Fixed js reference to non-existing element when CVV verification disabled and gateway supports SS-type credit cards

=== Known Issues ===
  * PayPal modules and Payflow Pro payment method backwards compatibility is officially not retained.
  * Nominal item total calculations do not work properly for multishipping checkout.




==== 1.4.x-devel-67099 ====

=== Improvements ===
  * Added isModuleEnabled() to core helper; Added ability to hide configuration fields if related module is not enabled (use 'if_module_enabled' node in system.xml)
  * Implemented IDNA domains support in registration and login forms (see also #20203)

=== Fixes ===
  * Fixed #22490: .Biz domain email addresses cause checkout to throw error and return to main Checkout page. Fixed path argument passed to include function in Zend_Validate_Hostname::isValid() to be valid whether source code compiler is used or not
  * Fixed Negative value in Shopping Cart in case Tax Calculation Method Based On Unit Price
  * Fixed Subtotal (Incl.Tax) = -$0.01 during created credit memo with refund shipping
  * Fixed: 100% discount of products -> the amounts of Tax and Grand Totals are or negative or not corectly




==== 1.4.x-devel-66609 ====

=== Improvements ===
  * Implemented 3D Secure validation for Maestro International and JCB cards
  * Added comments to system configuration fields "Catalog" > "Price" > "Catalog Price Scope" and "Currency Setup" > "Currency Options" > "Base Currency" that explain that base currency scope depends on the catalog prices scope.
  * Added note to reports that aggregated data depends on timezone and must be re-aggregated completely after global timezone change.

=== Changes ===
  * Cleaned up iphone theme from redundant files
  * Added Maestro International card type to credit card based payment methods (abstract).
  * Changed option "Notify Customer" into two options "Notify Customer by Email" and "Visible on Frontend" when adding an order comment. All comments that had the old value = 0, will be not visible on the frontend.
  * System configuration option "Sales" -> "Dashboard" -> "Use Aggregated Data" is marked as "beta"
  * Added "delta" rounding during shipping excluding/including tax calculation
  * Added discount tax as line item in PayPal
  * Reviewed logic of the sales reports:
    * Orders
    * Tax
    * Invoiced
    * Shipping
    * Refunds
    * Coupons

=== Fixes ===
  * Fixed issue when product quantity was incorrectly updated in stock after an order is placed for a configurable and a bundle products
  * Fixed #20697: wrong url rewrite resource model
  * Fixed duplicating of coupon code in shopping cart view
  * Fixed Catalog RSS feed showing prices including and excluding tax
  * Fixed #21501: Problem with translate inline and translations
  * Fixed setting URL key when using quick-create for simple products of the configurable.
  * Fixed adding comments to sales documents (invoices, shipments, credit memos)
  * Fixed #21816: Google Analytics Issue with Registration Checkout and Already Logged In
  * Fixed issue with number of orders that were created by Google Checkout
  * Fixed #22199: Duplicated Code - Useless Check
  * Fixed applied tax saving for shipping tax
  * Fixed issue that invoiced orders after cancelling become completed
  * Fixed #21533: Missing tranlation for "This date is a required value" in javascript
  * Fixed: Sales report last update date doesn't change after re-aggregating
  * Fixed rounding special price of selections in bundle product view
  * Fixed one day forward shift of dates in sales reports when showing empty rows
  * Fixed missed calculation of base_total_canceled & total_canceled fields on order cancellation
  * Fixed wrong calculation of base_discount_canceled & base_discount_canceled because of negative values of base_discount_amount in the sales order tables

=== Known Issues ===
  * The `sales_order_aggregated_created` table was re-created with new columns, it is not backwards compatible.



==== 1.4.x-devel-66014 ====

=== Improvements ===
  * Enabled "Refresh" mass-action as default in cache management grid
  * Implemented Centinel functionality in iphone theme
  * Optimized search reindex process a bit

=== Changes ===
  * Added 3rd optional argument to javascript function toggleValueElements(checkbox, container, excludedElements) in tools.js (products mass-update javascript)
  * Fixed #9600: Security compromised, Guest can subscribe a client to the newsletter
    * Checking if subscribing email adress does not belong to another user
    * If confirmation option selected and subscribing email is not user's login email - then confirmation is needed
  * Fixed #21304: Security compromised, guest can spam any email address
    * New config field added into cms -> customer -> newsletter "Allow Guest Subscription"

=== Fixes ===
  * Fixed order taxes report with Match Period To = Order Updated Date (typo)
  * Fixed issue when invoiced and not shipped yet orders after cancelling becomes completed
  * Fixed #21533: Missing tranlation for "This date is a required value" in javascript
  * Fixed stock management checking for a stock item when the stock management is disabled for this item (the check should be bypassed)
  * Fixed "New Products" RSS: added grouped and bundle products
    * Fixed the feed so that it contains grouped products now
    * The feed now shows the same products as shown in category view or "New products" widget (before the fix, incomplete products might be shown)
  * Fixed: virtual / downloadable product isn't deleted from the shopping cart, if change qty to '0'
  * Fixed #21866: 'Master Card' misspelling, should be spelled 'MasterCard' in credit card drop down options in checkout
  * Fixed #21771: Adjustment Refund & Adjustment Fee not showing in View Credit Memo
  * Fixed admin timeout issue inside iframe of Centinel validation
  * Fixed/reviewed tax calculation for components:
    * shipping price including tax in checkout process block
    * order/invoice/creditmemo shipping incl tax calculation
    * applied tax saving for shipping tax
    * applied tax saving for shipping tax
  * Fixed #16577: Dual Order with same Product
  * Fixed: #14502: Newsletter un-subscription message on customer account inappropriate

=== Known Issues ===
  * PayPal Direct PayFlow Edition may stuck with processing orders, if transactions are processed at manager.paypal.com. The problem is that IPN does not contain PNREF - the PayFlow transaction ID. This issue won't be fixed neither on PayPal, nor on Magento side. The only recommendation to merchant is to either process orders on Magento side only or on manager.paypal.com only.




==== 1.4.x-devel-65494 ====

=== Improvements ===
  * Added ability to have a comment for promotion rule fielset, similar to generic fieldset.
  * Added method for getting self child selection options recursively for promotion rule combines
  * Optimized catalog search system configuration fields sort order to make it more extendable.
  * Added icon for some buttons in admin that don't do some action instantly, but redirect to other page.
  * Added cache key generation on core template block level
  * Added ability to register product ids for last viewed products index
  * Added ability to disable observer call with <type>disabled</type> node (after backwards compatibility violation discovered)
  * Performance improvements on Mage_Catalog_Helper_Output::productAttribute method level
  * Added ability to use lazy connection instantiation on EAV resource models
  * Added "_isStraight" flag support on Mage_Core_Controller_Request_Http - allows to process request without additional logic (url rewrites, custom design visitor logging)

=== Changes ===
  * Sales reports refactoring after migration to flat sales structure: added a few indexes, optimized statistics reaggregation, fixed issue with generating statistics in wrong timezone (it was in UTC, but needs to be in the admin timezone)
  * Added Mage_Core_Helper_Abstract::stripTags() and utilized it in templates instead of strip_tags()
  * Improved and optimized base design package templates and layouts, minor fixes in payment method templates.
  * Moved fireEvent() function from adminhtml/events.js to a more generic js.js for future use
  * Added Mage_Core_Model_Config_Data::getFieldsetDataValue($key) - ability to get a neighbour system configuration value in backend model, when saving system configuration
  * Reviewed Magento user interface text labels and messages for proper grammar, informativeness and capital letters usage.
  * Reimplemented top menu rendering logic: implemented Mage_Catalog_Block_Navigation::_renderCategoryMenuItemHtml(), deprecated Mage_Catalog_Block_Navigation::drawItem() and reimplemented to work through _renderCategoryMenuItemHtml for compatibility
  * Added url rewrites on last viewed products collection
  * Reimplemented products bestsellers report: report uses pre-aggregated data to improve performance
  * Moved logic of reaggregating reports data from sales report controller into separate controller, added bestsellers report handling there

=== Fixes ===
  * Fixed #20782: Wrong prices exc. tax with discount in cart
  * Fixed #21099: Wrong subtotal for manual order entry with manual price
  * Fixed #21271: Price inc tax and exc. tax same for grouped product
  * Fixed grid js object name in grid pager: now it uses block method instead of direct building
  * Fixed changing notification when editing a product in various tabs:
    * Downloadable products: links title (element had no id attribute and thus was omitted by the event dispatcher init code)
    * Custom options: whatever was added with "Add option"
    * Bundles: whatever was added with "Add option"
    * All date input fields when using the calendar widget
    * Prices: tiered prices box, all rows added with "Add tier"
  * Fixed #6321: Add RSS urls to head section
  * Fixed #21831: Tax Calculation Version 1.4.0.1 still incorrect
  * Fixed #12067: iPhone Terms and Conditions Box
  * Fixed #20631: Order totals when creating order from admin do not reflect currently selected currency
  * Fixed #21777: Catalog pricerules
  * Fixed #14591: Incorrect SKU for Configurable Product with Custom Options
  * Fixed #20832: PayPal Standard tax issue: implemented proper tax and discounts validation/transferring with cart line items
  * Fixed #17451: Header Links (top.links.phtml) does not output correctly because it is using the model code (the Toplinks block is deprecated)
  * Fixed #21302: PayPal PayFlow Pro: card expiration date format should be MMYY, not MMYYYY. Also fixed country code typo issue.
  * Fixed #21686: Typo in tag.xml
  * Fixed extra quoting in select html element
  * Fixed XHTML validation errors in admin in some places
  * Fixed #21912: calculation error transfer between multishipping address
  * Fixed typo in PayPal NVP API that caused impossibility to do partial captures




==== 1.4.x-devel-64603 ====

=== Improvements ===
  * Implemented 3D Secure validation for the JCB credit cards
  * Added "Only X Left" feature - an option to show on a product view page how many items remains in stock, if it is lower than specific threshold.
  * (in progress) implementation of #7741: Customer group increase order size . The feature is called "Qty Increments" - to trade items in boxes only. I.e. allow to purchase 6, 12, 18 items etc...

=== Changes ===
  * Refactored frontend navigation menu HTML structure and javascripts: the menu expands and collapses with small delay making it more accessible for users. Fixed possible compatibility issue in Mage_Catalog_Block_Navigation::drawItem() and marked as deprecated after 1.4. Removed local calls of onmouseover/onmouseout events to improve SEO.
  * Added ability to assign id for field containers (TR tag) using node <use_container_id>1</use_container_id> in system configuration
  * Moving widgets.css below in the code for proper styles overriding.
  * Moved JCB credit card declaration and implementation into the Mage_Payment module. Removed it from other modules (they will inherit JCB card from "CC" payment method)
  * Modified Varien_Object_Mapper to check arrays using array_key_exists() instead of isset()
  * Indexer changes (related to the #21031):
    * Removed DROP/CREATE statements for index temporary tables
    * Created static index temporary tables (InnoDB and MEMORY) and separated using those tables in reindexiAll() and reindexEntities()
  * Added ability to set a comment in adminhtml generic fieldset renderer

=== Fixes ===
  * Fixed #21313: Display price including TAX
  * Fixed #21632: Associated products don't get cached
  * Minor bugfixes in 3D Secure integration (API debugging, improvements in css and javascript)
  * 3D Secure integraion - fixed confused constant values in centinel service model
  * Fixed autocomplete in year field on new user registration
  * Fixed _isCaptureNeeded validation for PayPal pro (exception during invoicing captured transaction)
  * Fixed typo in PayPal Direct API variable "AUTHSTATUS3DS" (error in official documentation)
  * Moneybookers:
    * fixed translations in the activation email
    * minor fixes in account confirmation javascript
    * Fixed #21752: Moneybookers configuration per store
  * Fixed #21302: PayPal PayFlow Pro: card expiration date format should be MMYY, not MMYYYY
  * Fixed #20932: unique key in catalog_product_link
  * Fixed #21031: Simultaneous product->save() causes "Base table or view already exists: 1050 Table catalog_product_index_price_idx' already exists




==== 1.4.x-devel-64038 ====

=== Improvements ===
  * Minor CSS improvements in frontend themes
  * Image/media browser minor UI improvements
  * Added default placeholder for skin images in wysiwyg
  * Minor style improvements for widgets insertion overlay
  * Implemented 3D Secure transactions debugging
  * Added ability to set a writer adapter to the Mage::log() and to use Mage::log() regardless of system configuration settings
  * Added Magento Variable icon for WYSIWYG
  * Added ability to append custom class name to main pop-up window container
  * Added explanation comments for Centinel Api Custom URL

=== Changes ===
  * Added element as parameter of system configuration field getCommentText method
  * Added ability to use isObjectNew method of model for object save on resource model level
  * Added additional blocks support on order history and last orders blocks level
  * Made encryption key length check binary-safe
  * Added full exception trace logging to cron_schedule table
  * Moved shopping cart price rule coupon to separate table, improved shopping cart price rule management UI
  * Added ability to specify model for system config field comment generation (system.xml):
    * <comment><model>module/model</model></comment>
    * requires getCommentText method definition from defined model
  * Changed the way how payment methods debug transactions: instead of database the debug information is written into var/log/payment_<method_code>.log
  * Updated text labels in sales reports: terminology for "report type" (period matches to)
  * Added new column 'updated_at' for wishlist table. Changed controller and model logic to save new data.

=== Fixes ===
  * Fixed #21250: HTML code displaying like text in descriptions / List View Displaying HTML Entity Values
  * Fixed #21251: html code shows in category product listing
  * Fixed: Unit Price in Shopping Cart is incorrect when applying a Coupon Code
  * Fixed #18536: Rounding error on Shipping Tax calculations
  * Fixed bugs with row based tax calculation and shipping tax calculation
  * Fixed width/height in WYSIWYG image insertion
  * Fixed authorize.net payment transaction saving during capture
  * Fixed #20890: Incorrect function name
  * Fixed #21055: No Navigation on Advanced Search Results
  * Fixed #20912: memory_limit suffix other than 'M'
  * Fixed #20884: JS bug in Widget/Grid/Column/Action.php
  * Fixed #7228: Credit Memo - Adjustment Fee $ or %
  * Fixed #20832: paypal - standard Tax issue
  * (in progress) UI minor fixes in 3D Secure validation process
  * Added forgotten Moneybookers email template




==== 1.4.x-devel-63512 ====

=== Improvements ===
  * Implemented #6321: Add RSS urls to head section
  * Implemented #7293: Track IP in abandoned cart
  * (in progress) Ability to not include a category into navigation menu

=== Changes ===
  * Refactored Sales module resource from EAV into flat structure.
  * Sales entities data structure changes:
    * Dashboard optimization + configuration option "Use Aggregated Data" for dashboard
    * Inventory: moved stock items qty manipulations out of transaction, fixed qty upgrade logic (x+delta)
    * Added configuration option "Automatically return Credit Memo item to Stock" for refunds autogeneration
    * Removed downloadable products FK relation with sales module
    * Sales order tax logic moved to tax module and relation with sales module by FK
  * Sales, SalesRule and Checkout modules changes:
    * Added product customer group property validation on sales rules level
    * Added ability to assign quote object to checkout cart model
    * Prevented redundant customer model load in customer address
    * Optimized saveDownloadableOrderItem item in downloadable product observer
  * Prevented double "order by" in collection select statement
  * Added _beforeLoad support and not changed object save protection on core abstract level
  * Extended abstract collection with add/remove fields to/from select
  * Escaped html entities in mail form in 404, 503 and report.php error pages, prevented errors if global array $_SERVER is undefined
  * Minor text changes in PayPal modules
  * Added not existin observers methods calls protection
  * Separated tax shipping total from tax subtotal. Now taxes for store prices (code tax_subtotal) calculates before shipping, then calculates shipping (code shipping) and taxes for shipping (code tax_shipping) and then calculates customer taxes (code tax).


=== Fixes ===
  * Fixed #21061: Global country tax applied instead of specific state tax
  * Fixed catalog price rules different sorting when applying the rule vs. saving the product
  * Fixed #20603: Async Google Analytics throws js error (_gaq not defined)
  * Fixed SQL error possibility when adding bundle to cart
  * Fixed #16684: ini_set of auto_detect_line_endings during Varien_Io_File::streamReadCsv
  * Fixed #17748: Category chooser at price rules
  * Fixed #20161: Special From Date for website
  * Fixed Fatal error: Call to undefined method Mage_Admin_Model_Observer::actionPostDispatchAdmin() in \app\code\core\Mage\Core\Model\App.php on line 1207 (backward compatibility)




==== 1.4.x-devel-62916 ====

=== Improvements ===
  * Improved visual design of widget and variable insertion, and media browser overlay
  * Product custom URL rewrites redirect to SEF URL, rather than to catalog/product/view/id/
  * URL rewrites history: ability to auto-generate custom rewrite with redirect from old to new URL when changing product URL-key
  * Optimized getAttributeRawValue() method in catalog module for retrieving more then one attributes

=== Changes ===
  * Added javascript validation for JCB cards
  * Changed confusing error message about quantity in shopping cart into proper one
  * Added comments collection loading when invoice, credit memo or shipment created with adding comment: needed before adding first comment.
  * Added Varien_Db_Ddl_Table
  * Added method createTable from DDL to Varien_Db_Apater_Pdo_Mysql
  * Removed getting Varien_Object id in Varien_Debug

=== Fixes ===
  * Fixed read/write connection issue during new customer order place. See http://www.magentocommerce.com/boards/viewthread/19363/P0/
  * Fixed confusion with admin page title when editing product
  * Fixed bug in Mage_Bundle_Model_Product_Type::getSelectionsCollection(): retrieved collection depends on passed optionIds only on first method call
  * Fixed: New products RSS feed appears instead of the Special products RSS feed
  * Fixed tax rule ZIP range matching (numeric values were matched as strings)
  * Fixed #14055: New orders RSS feed displaying incorrect customer name
  * Fixed #19192: Error when product inventory messed up on viewing order.
  * Fixed minor visual design issues in themes and skins
  * Fixed getting secure host URL in 404, 503 and report.php error pages
  * Fixed up filtering of filenames of uploaded files
  * Fixed position issue for cross-sell products
  * Fixed #20372: importing images
  * Fixed: #17845: Validation and Ampersand Flaws in Layered Navigation and other locations that use the fake query string
  * Fixed #15592: Mage_Adminhtml_Model_System_Config_Source_Shipping_Allowedmethods::toOptionArray() not compatiable with parent method
  * Made proper validate() independent of submit in form.js (Visions contribution)
  * Fixed incorrect js logic on order create backend page (Visions contribution):
    * Fixed: when create order, it is not possible to resubmit after initial validation failed (because submit button is disabled)
    * Improved client side validation that new order has shipping address (it is required to click "get shipping method and rates"
    * Improved client side validation that payment method is selected (like in checkout of frontend)
  * Improved usability of sales admin (Visions patch):
    * added ability to export csv or excel for orders, shipments, creditmemos, invoices
    * made filter for creditmemo and shipment type text so it is possible to just enter one id and find object looking for (unified with orders and invoices, there it is already text not number)
  * Fixed #17659: UPS Minimum Weight Required for Negotiated Rates
  * Fixed #20580: Index module not translated

=== Known Issues ===
  * It is impossible to run more than one 3D Secure card validations simultaneously in one session. Not fixable.




==== 1.4.0.1 ====

=== Changes ===

  * The error report exception printing is disabled by default for security reasons. To print the error report, copy the errors/local.xml.sample to errors/local.xml
  * XSS vulnerabilities review
  * Added Phoenix_Moneybookers payment method module (from now bundled in Magento out of the box)

=== Fixes ===

  * Fixed #20680: Catalog - Google Sitemap
  * Fixed #20024: Error message 'Data saving problem' when try to checkout with multiple addresses (when address deleted during multishipping process)
  * Fixed #20625: Fatal error: Exception thrown without a stack frame in Unknown on line 0 (Fixed cache backend instantiation when a shared PEAR library is in the include path)
  * Fixed issues of upgrading from 1.3.x to 1.4.x through Magento Connect in some installations
  * Fixed #20659: Unable to choose images for upload (duplicates: #20588, #20573, #20616, #20595)
  * Fixed shell cron script runner
  * Refixed #17963: Ampersand in Search Breadcrumb: Double-encoded

=== Upgrade Notes ===

  * We highly recommend disabling Magento cache before upgrading
  * In layout of any custom theme the usage of catalog/product_list_toolbar block should be changed to page/html_pager:
    1) Replace the catalog/product/list/toolbar.phtml of your theme by the new one
    2) Update catalog.xml layout: <block type="catalog/product_list_toolbar" name="product_list_toolbar" template="catalog/product/list/toolbar.phtml"> should be replaced into <block type="page/html_pager" name="product_list_toolbar_pager"/>




==== 1.4.0.0 ====

=== 1.4 Major Improvements since 1.3 ===
  * Implemented 3D Secure credit card validation (Visa and Mastercard)
  * Full reimplementation of PayPal modules, includes lot of new functionality and numerous bugfixes
  * Full review of frontend themes, introduced design cross-package fallback and the base/default theme. Includes SEO and accessibility enhancements. Changes are oriented to dramatically reduce themes maintenance.
  * Added ability to define arbitrary cache backends
  * Optimized performance of sales reports, added new sales report types
  * Added image/media uploader/browser, that can browse entire media folder
  * Optimized performance of search indexer
  * Made order processing workflow more informative and severe
  * Reimplemented 404 and report pages, introduced 503 page, specifically for maintenance purposes
  * Improved javascript files merging, added CSS files merging
  * Added Widgets functionality, added several widgets out of the box
  * Added Custom Variables functionality
  * Added lot of new System Configuration options
  * Improved order placement reliability
  * Added WYSIWYG for CMS and Catalog
  * Optimized cache initialization during startup
  * Optimized export from grids in admin area
  * Improved tax and discount totals calculation
  * Replaced admin notification flash popup into a simple HTML overlay
  * Implemented product and category URLs per store view
  * Added ability to configure entry point using virtualhost environment configuration, rather than creating another physical entry point
  * Optimized simple product view without custom options

=== Coommunity Edition Changes since 1.4.0.0-rc1 ===

== Improvements ==
  * Implemented 3D Secure credit card (Visa, Mastercard) validation for payment methods:
    * Saved CC
    * PayPal Website Payments Pro - Direct Payments
    * PayPal Website Payments Pro (Payflow Edition) - Direct Paymens
    * Payflow Pro
  * Improved modern theme: significantly reduced number of files in virtue of cross-package fallback to base/default theme
  * Implemented #11012: Support canonical link tag
  * Implemented WYSIWYG for newsletter templates
  * Minor improvements in sales reports
  * Renamed button "Refund" to "Refund Offline" on Credit Memo page for order
  * 19963: Mage_Eav_Model_Entity_Setup::addAttributeToGroup() (visions patch)
  * improved print.css for CE themes
  * SEO and accessibility improvements in default/default, default/modern and default/blank themes
  * left and right callouts templates, both callouts images and links are now controlled via catalog.xml
  * Added relevant page titles in admin area
  * Implemented column decorators and ability to use getter callback in admin grids
  * Made fetching payment methods sort order properly: via getConfigData() rather getStoreConfig() (optimization for 3rd-party customizations)
  * Implemented ability for page/html_wrapper block to not render the wrapper tag, made it output children sorted
  * Implemented wrappers for inserting additional blocks in:
    * before shopping cart line items list
    * before onepage checkout login/registration form
    * before customer registration form
    * before newsletter subcription form (customer "My Account")
    * before product review form
    * before product tag submission form (product view page)
  * Implemented giropay integration with PayPal Express Checkout
  * Added before/after initialize and before/after validate events to opcheckout.js
  * Optimized products toolbar functionality, prevent saving to session default grid parameters (for sorting, pager etc.)
  * Added filter by website in "Last ordered items" block

== Changes ===
  * PayPal Website Payments Pro (Payflow Edition) is completely rewritten, as extending Mage_Paypal module. With breaking code backwards compatibility.
  * Mage_Core_Model_Flag - moved setting flag_code to _construct()
  * AmazonPayments module is removed from package and will be available as a separate extension on Magento Connect
  * #19595: Varien_File_Uploader_Image not working - class is deprecated and should not be used
  * Marked dead code Mage_Checkout_Model_Type_Abstract::_emailOrderConfirmation() as deprecated
  * Reimplemented 404, 503 and report.php error pages: now fully configurable from errors/local.xml, with ability to override theme per entry point or even store view
  * error report doesn't disclose the trace by default anymore
  * Added to Catalog Product Price indexer upgrade operation by removing old temporary index tables if exists
  * Product image uploader security measurements:
    * disabled ability to run php scripts in "media" folder
    * added callback validation to File/Uploader.php
    * added image file validation to Catalog/Product/GalleryController.php
  * Prevented flushing output buffer caused by exceptions in templates included by core/template block
  * added default _type param to Design Package getters in core/design_package model
  * Added additional qty parameter to event 'catalog_product_get_final_price'
  * Updated sales sql-upgrades: fixed missing table prefixes in some places, rewrote adding foreign keys via methods
  * Implemented 'any-value-validate' logic for Catalog Rules; common methods moved to parent (Mage_CatalogRule_Model_Rule_Condition_Product) class
  * Expanded width of fields on product and category edit pages
  * Added ability to render number sign in currency and number grid renderers
  * Fixed datetime grid renderer to make it use getters (see parent class)
  * Added Mage_Core_Block_Abstract::escapeHtml() instead of htmlEscape()
  * Added ability to make output optional in page/html_pager block (when items total quantity is less than page size)
  * Added ability disable product list toolbar params saving to session
  * Added sorting by param name to query params part of url
  * Made page/html_wrapper block treat children empty output as if there are no children.
  * Implemented dynamic BN codes for PayPal. Pattern: Varien_Cart_(EC|DP|WPS)[_<country_code>] where country code is one of 18 country codes currently PayPal has localized market sites.  * Fixed session cookie renew functionality, added ability define cookie settings for javescript methods
  * When LN filter for an anchor category is active not allow to use display mode "Static Block Only"
  * Sales: made online operations and notifications updating "online" totals, instead of totals mixed with online/offline sales documents. Removed updating "base_amount_canceled" total update when voided payment (this was backwards compatibility violation)

== Fixes ==
  * Fixed 'tax_rate_data_fetch' event params
  * Minor fixes in PayPal Express Checkout and PayPal Direct (non-reported bugs, terminology issues)
  * Fixed #16210: Input field size decreased in category products grid
  * Fixed #17281: Google Checkout: Incorrect assigning of [parent_id]
  * Fixed #14251: Google Checkout still does not allow free shipping
  * Fixed #11412: Rounding error in tax and shipping calculation
  * Fixed #11836: No authentication on customer reviews url
  * Fixed #13511: "Default web url" does not work as expected
  * Fixed #14469: Newly created products for configurable products do not stick
  * Fixed #14915: Invoice payment capture _needToAddDummy bug
  * Fixed #15235: Special price bug with multiple websites
  * Fixed #16425: printing in admin breaks top menu
  * Fixed #16499: Require customer login for reviews not 100% working
  * Fixed #17058: Currency Switch won't work on first time in shop frontend (session id issue)
  * Fixed #17504: Birthday getting swapped (Month and Day)
  * Fixed #17720: core_flag primary key is a smallint and has a max value of 65535
  * Fixed #17793: Google Base Special Price not mapped to Price
  * Fixed #Fixed #18127: Bundle Products pricing incorrectly when not required
  * Fixed #18341: Bugs in dataflow: number of records
  * Fixed #18745: Customer Import shouldn't send email
  * Fixed #18868: Unable to use Mage::log() before config is read
  * Fixed #19290: Changing 'My Account' info may destroy log in when password is blank
  * Fixed some XSS vulnerabilities in admin
  * Fixed #19448: Incorrect handling of empty attributes under PHP 5.2.0
  * Fixed #19449: Google Base
  * Fixed USPS First Class International and USPS Express Mail International shipping method that stopped working after gateway changes
  * Fixed #19512: /index.php/checkout/onepage/getAddress/address/ allows everyone logged in to get all addresses
  * Tax rates edit form won't clean on validation error anymore
  * Fixed #19702: getLastOrderId missing parameter
  * Fixed #19729: unable to translate "Display product options in" and "Product Type"
  * Fixed #19753: Compare products page breaks if no attributes are marked as "Comparable"
  * Fixed #19791: Shipment tracking not displayed from admin panel with store code in URLs enabled
  * Fixed #19838: missing two escape characters in validation.js at the validate-email regex
  * Fixed #19873: Minor warning fix
  * Fixed #19904: please remove double file extensions in filenames of uploaded files
  * Fixed #19954: Undefined variable
  * Fixed #19960: Google Analytics Asynchronous Tracking Code
  * Fixed #19964: cart sidebar shows zero total when displayed including tax
  * Fixed #19969: Css is wong for gift-message-form
  * Fixed #20023: Admin login is very slow when widgets.magentocommerce.com is down
  * Fixed #20080: Dataflow Profiles Need to be Sorted
  * Fixed #20250: Search'n'replace oversight
  * A few fixes in URL rewrites logic
  * Fixed #20350: WRONG "XML_PATH_SCHEDULE_GENERATE_EVERY"
  * Fixed #20361: Move Category Failed
  * Fixed #6564: Transactional Email Templates Using alt="Magento"
  * Fixed #8514: Negative Number in Sorting
  * Fixed Price indexer website date/rate
  * Fixed tier_price and website table names in Catalog Product Price Default indexer
  * Fixed command line installation - fatal caused by improper website initialization
  * Implemented correct setting attributes to entity including situation when there are no attribute value for default sore
  * Fixed #19263: Adminhtml Html Error: Double </label>
  * Fixed "undefined index" notice when saving Table Rates without uploading import rates file.

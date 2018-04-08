
# CleanBuild
A clean WordPress boilerplate to make creating custom sites quicker & easier.


### Required Plugins
ACF is required to enable the custom shortcodes/options that the skeleton html includes.
 * Advanced Custom Fields Pro


### Included 3rd party libraries
Theses libraries are enqueued in ``` functions/wordpress/site-enqueue.php ``` but are commented out by default.

 * Slick.js
 * Backstretch
 * Fancybox
 * FontAwesome  4 (_Requires a CDN ID_)


## Company Detail Shortcodes
These are all of the shortcodes & their options that are generated using the __Company Details__ tab in the backend of WordPress.

### Company Address
Returns the __Company Address__ field. It returns each row in to a separate ```li``` tag.
```php
<?php echo do_shortcode('[address]'); ?>
```
##### Options
Option | Type | Default | Description
--- | --- | --- | ---
row | int | 1 | Selects which repeater row phone number will be returned
include-name | boolean | false | Will return the company name as the first ``` li ```
container | boolean | false | Will wrap the returned list items in a ```ul``` with the class of ```address-list```

### Company Email Address
Returns the __Company Email Address__ field in plaintext.
```php
<?php echo do_shortcode('[email]'); ?>
```
##### Options
Option | Type | Default | Description
--- | --- | --- | ---
row | int | 1 | Selects which repeater row of the __Email Address__ field will be returned
link | boolean | false | Will return the email address with _mailto:_ before the email and a _?subject_ after
quick-link | boolean | false | Will return the email address automatically wrapped in an ```a``` tag

### Company Phone Number
Returns the __Company Phone Number__ field in plaintext.
```php
<?php echo do_shortcode('[phone]'); ?>
```
##### Options
Option | Type | Default | Description
--- | --- | --- | ---
row | int | 1 | Selects which repeater row of the __Phone Number__ field will be returned
link | boolean | false | Will return the phone number with _tel:_ before the number
quick-link | boolean | false | Will return the phone number automatically wrapped in an ```a``` tag

### Company Social Links
Returns the __Company Social Links__ field. It returns each row in to a separate ```a``` tag.
```php
<?php echo do_shortcode('[social]'); ?>
```
##### Options
Option | Type | Default | Description
--- | --- | --- | ---
container | boolean | false | Will wrap the returned social links in a ```div``` with the class of ```social-links```

### Company Name
Returns the __Company Name__ field in plaintext.
```php
<?php echo do_shortcode('[company-name]'); ?>
```

### Company Fax Number
Returns the __Company Fax Number__ field in plaintext.
```php
<?php echo do_shortcode('[fax]'); ?>
```

### Company Registration Number
Returns the __Company Reg Number__ field in plaintext.
```php
<?php echo do_shortcode('[reg-number]'); ?>
```

### Company Opening Hours
Returns the __Company Opening Hours__ field in plaintext.
```php
<?php echo do_shortcode('[opening-hours]'); ?>
```

# Template for WordPress projects with Composer

A full fledged composer template for setting up and managing a WordPress project with Composer. 

This template comes with the following standard plugins:
---
- [Schema – All In One Schema Rich Snippets](https://wordpress.org/plugins/all-in-one-schemaorg-rich-snippets/)
- [AMP](https://wordpress.org/plugins/amp/)
- [BBQ:Bad Block Queries](https://wordpress.org/plugins/block-bad-queries/)
- [Contact Form 7](https://wordpress.org/plugins/contact-form-7/)
- [Cloudflare](https://wordpress.org/plugins/cloudflare/)
- [Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/)
- [Flamingo](https://wordpress.org/plugins/flamingo/)
- [SSL Insecure Content Fixer](https://wordpress.org/plugins/ssl-insecure-content-fixer/)
- [Super Progressive Web Apps](https://wordpress.org/plugins/super-progressive-web-apps/)
- [Wordfence](https://wordpress.org/plugins/wordfence/)
- [YoastSEO](https://wordpress.org/plugins/wordpress-seo/)

---

## How To Setup:

Please see requirements below before moving on to the steps.

### Requirements:
- Server with PHP / Apache (or Nginx) / MySQL (or PostreSQL)
- Git
- Composer

### Steps:

1. Clone this repository into your website projects folder:

```
git clone git@github.com:martingrondein/wordpress-composer-full.git
```

2. Install this desired setup with Composer:

```
cd wordpress-composer-full
composer install
```

3. Copy web/index.php to your project folder. You can do this from the command line with

```
cp web/index.php ./index.php
```

4. Slightly modify index.php in your project root. The index.php in the root of your project (the one you just created via a copy command) should be modified.

So...
```
require( dirname( __FILE__ ) . '/wp-blog-header.php' );
```
... becomes ...
```
require( dirname( __FILE__ ) . '/web/wp-blog-header.php' );
```
--- 
Please note: If you are looking for a no-frills composer.json template, please see the [wordpress-composer-base](https://github.com/martingrondein/wordpress-composer-base) repo.

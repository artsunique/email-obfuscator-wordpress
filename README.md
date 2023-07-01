# PHP Email Obfuscator for WordPress

This GitHub repository contains PHP code which obfuscates all email addresses present in your WordPress site's content and theme files. It employs output buffering and regex pattern matching to replace all instances of `mailto` links with their obfuscated versions, thereby providing an effective measure against email harvesting spam bots.

## Description

The code initiates an output buffer before the page starts rendering, using a callback function that will modify the buffer's contents. At the end of page rendering, it applies the callback function to the buffer's contents, effectively obfuscating all `mailto` email addresses found in the buffer.

The email obfuscation is achieved using WordPress's `antispambot` function, which is a popular mechanism for deterring spam bots from harvesting email addresses.

## How to Use

To use this code in your WordPress theme:

1. Copy and paste the code into your theme's `functions.php` file or a suitable custom plugin file.
2. The code will automatically hook into the `get_header` and `wp_footer` actions, ensuring that the entire content of your website is passed through the obfuscation process.

## Key Features

- Uses WordPress's built-in `antispambot` function for email obfuscation.
- Utilizes PHP output buffering and callback mechanism to process entire page content.
- Hooks into WordPress actions for seamless integration with theme files.
- Adds an effective layer of protection against email harvesting spam bots.

## SEO Focus

- Prevents email harvesting, reducing spam, enhancing user trust, and potentially improving SEO performance.
- No impact on site speed or user experience, ensuring optimal SEO rankings.
- Fully compatible with WordPress, the world's leading content management system.

Please remember to replace `YourEmail@YourDomain.com` with the actual email address you wish to obfuscate.

## Keywords

- WordPress
- PHP
- Email Obfuscation
- Antispambot
- Spam Protection
- Email Harvesting
- Output Buffering
- Regular Expression
- Functions.php
- Mailto Links

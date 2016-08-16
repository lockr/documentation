---
title: WordPress
description: Learn how to bring WordPress sites on to the Pantheon Website Management Platform, and considerations for developing and running them.
keywords: wordpress, sites, pantheon
categories: [wordpress]
tags: [code]
---

WordPress began as a blogging platform and has now evolved into the most used Content Management System today. This open source software thrives through its expanding community and highly customizable core, making it a perfect fit for projects of any scope.

## Get Started
[Migrate WordPress](/docs/migrate-wordpress) using the [Pantheon Migrations](https://wordpress.org/plugins/bv-pantheon-migration/) plugin or [launch a new site](/docs/launch-wordpress).
## WordPress Code
WordPress site code repositories are clones of one our [WordPress upstream](https://github.com/pantheon-systems/wordpress), and consist of the following files and directories:
```
├── index.php
├── wp-activate.php
├── wp-config.php
├── wp-comments-post.php
├── wp-blog-header.php
├── wp-admin
├── wp-cron.php
├── wp-load.php
├── wp-links-opml.php
├── wp-includes
├── xmlrpc.php
├── wp-trackback.php
├── wp-signup.php
├── wp-settings.php
├── wp-mail.php
├── wp-login.php
├── wp-content
    ├── index.php
    ├── mu-plugins
    ├── themes
    ├── plugins
```
This repository includes the [core themes from twenty-ten to the present](https://github.com/pantheon-systems/WordPress/tree/master/wp-content/themes). Pantheon no longer updates these themes in the upstream repository after their release. They will likely be out of date when you install WordPress, and it is safe to update or remove them from your code repository without the potential of future conflicts.
The same is true for the [Akismet Plugin](https://github.com/pantheon-systems/wordpress/tree/master/wp-content/plugins). New WordPress sites ship with Akismet 3.1.5. Akismet is safe to upgrade or remove from your site's codebase.
## WordPress Dashboard
Learn how to [manage plugins and themes using the WordPress Dashboard](/docs/more-sftp#manage-plugins-and-themes-with-wp-admin) and SFTP mode.
## wp-config.php
The Pantheon architecture allows every environment on your site to run on it's own container, meaning variables within the `wp-config.php` file change periodically. Despite dynamic variables, you are still free to [configure `wp-config.php`](/docs/wp-config-php) on Pantheon to fit your unique needs.
## PHP Sessions
While WordPress core itself does not use PHP sessions, some plugins and themes do. Learn how to implement [built-in session handling functions](/docs/wordpress-sessions).
## WordPress Configuration Management
Keep track of database configurations with ease by using [wp-cfm](/docs/wp-cfm).
## WordPress Cron
You are probably familiar with cron jobs, but do you know how `wp-cron` works? Learn and understand how [cron for WordPress](/docs/wordpress-cron) is triggered.
## Launch Check
Pantheon analyzes code to provide performance and configuration recommendations for your dynamic WordPress sites. Go live with confidence using [Launch Check for WordPress](/docs/wordpress-launch-check).
## Additional Resources
- [WordPress FAQ](/docs/wordpress-faq)
- [WordPress Known Issues](/docs/wordpress-known-issues)
- [Adding HTTPS For Free with CloudFlare](/docs/guides/cloudflare-enable-https/)
- [CloudFront CDN Setup for WordPress](/docs/wordpress-cloudfront)
- [Configuring JetBrains PhpStorm IDE with WordPress on Pantheon](/docs/wordpress-phpstorm)
- [Fix Broken Links in WordPress](/docs/wordpress-broken-links)
- [Installing Redis on WordPress](/docs/wordpress-redis)

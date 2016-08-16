---
title: Scope of Support
description: Understand how Pantheon's support team can help you.
categories: [managing]
tags: [code, debug, featured]
keywords: support, scope, customer support, getting started
---
We love helping developers succeed! We also have limits to the support we can provide. The key to a great relationship is clear expectations of our support scope. For details on ways to contact our Support team and view ticket response times, visit [Getting Support](/docs/getting-support).

- We don't touch client code.
Your site code belongs to you. Pantheon provides updates to the upstream for the site, which only affect core files and Pantheon-specific additions. It is your responsibility not to overwrite the upstream. If you do, updates on the Dashboard will cause conflicts that you must [resolve manually](https://pantheon.io/docs/upstream-updates/#debug-failed-merges) with Git.

- Outdated versions of core are not supported on the platform. This includes importing a site, then manually downgrading to an older version of core. Sites utilizing a [custom upstream must be updated](/docs/managing-upstreams/) by the upstream maintainer each time the project releases a new version.

- We love adding features, but platform changes take time and consideration, and unfortunately feature requests are often declined if there is potential performance or user experience degradation.

- Pantheon provides a great backend, but cannot provide code-level debugging, Git training, or site architecture recommendations. New Relic and debugging can get you pretty far.  We have a [comprehensive list of docs](https://pantheon.io/docs/tags/debug/) to get you underway.

- If your site is slow or modules aren't working, please see our [performance articles](/docs/code/#performance). Issues with the platform are posted on our [status page](http://status.pantheon.io). If there are no platform events, the solution is probably within the site's code.

- Pantheon can only assist if we can replicate the problem. Intermittent issues and server errors are rarely random, rather, they are issues with a yet undefined trigger. Please try to replicate and debug [site errors](/docs/errors-and-server-responses/) in your Development environment. If you submit a ticket to our Support team, include your findings and attach screenshots whenever possible.

- We recommend development on the platform, rather than on a local environment. Unexpected behavior, not apparent on local instances such as MAMP or shared hosting, can be due to different versions of PHP, different levels of error reporting, Apache vs NGINX, or server configuration. Pantheon is not responsible for resolving such issues.

- Pantheon Support can quickly determine if an issue is platform related. We take full responsibility for our services and performance, but if something is affecting your site only, or a single environment only, we will most likely refer you to our debugging tutorials.

- If we see your site is a volcano of errors or overloading resources, we will contact you and ask you to take immediate action. If unresponsive, we may need to put the site into maintenance mode.

If you need a professional to provide development support for your site, use Pantheon's [Agency Finder](https://pantheon.io/agencies/agency-finder) to search for qualified partners you can trust.

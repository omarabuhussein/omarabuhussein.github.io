---
layout: post
title:  "Get Logged-in user ID"
image: ''
date:   2016-10-22 00:06:31
tags:
- session
description: ''
categories:
- CiviCRM Session
serie: learn
---

To get current logged-in user ID :

```php?start_inline=1
$userId = CRM_Core_Session::getLoggedInContactID();
```
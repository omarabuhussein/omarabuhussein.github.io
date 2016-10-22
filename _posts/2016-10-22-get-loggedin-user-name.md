---
layout: post
title:  "Get Logged-in user display name"
image: ''
date:   2016-10-22 00:06:31
tags:
- session
description: ''
categories:
- CiviCRM Session
serie: learn
---

To get current logged-in user diplay name :

```php?start_inline=1
$userFullName = CRM_Core_Session::getLoggedInContactDisplayName();
```
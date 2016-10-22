---
layout: post
title:  "Get CiviCRM version"
image: ''
date:   2016-10-22 00:06:31
tags:
- system-utilities
description: ''
categories:
- CiviCRM System Utilities
serie: learn
---

To get Current installed CiviCRM version :

```php?start_inline=1
$civicrmVersion = CRM_Utils_System::version();
```

To get only the first two parts (eg. 4.7) :

```php?start_inline=1
$civicrmVersion = CRM_Utils_System::majorVersion();
```


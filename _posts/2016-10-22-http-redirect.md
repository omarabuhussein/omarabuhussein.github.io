---
layout: post
title:  "HTTP Redirect"
image: ''
date:   2016-10-22 00:06:31
tags:
- system-utilities
description: ''
categories:
- CiviCRM System Utilities
serie: learn
---

To redirect to a specific page :

```php?start_inline=1
CRM_Utils_System::redirect('REDIRECT-URL');
```

Example :

```php?start_inline=1
$path = 'civicrm/admin/extensions';
$params = http_build_query(['reset' => 1]);
$url = CRM_Utils_System::url($path, $params); // generate URL
 
CRM_Utils_System::redirect($url); // Redirect to the generated URL
```

This will redirect the user to the extensions manager page.
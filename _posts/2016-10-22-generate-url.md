---
layout: post
title:  "Generate URL"
image: ''
date:   2016-10-22 00:06:31
tags:
- system-utilities
description: ''
categories:
- CiviCRM System Utilities
serie: learn
---

To generate a URL :

```php?start_inline=1
$path = 'you/relative/path';
$params = http_build_query(['param1' => 1, 'param2' => 'test']);
$url = CRM_Utils_System::url($path, $params)
```

Example (relative URL version):

```php?start_inline=1
$path = 'civicrm/admin/extensions';
$params = http_build_query(['reset' => 1]);
$url = CRM_Utils_System::url($path, $params);
```

absolute URL version : 

```php?start_inline=1
$path = 'civicrm/admin/extensions';
$params = http_build_query(['reset' => 1]);
$url = CRM_Utils_System::url($path, $params, true);
```
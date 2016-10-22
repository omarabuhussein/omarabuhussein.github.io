---
layout: post
title:  "Get Enabled Components"
image: ''
date:   2016-10-22 00:06:31
tags:
- components
description: ''
categories:
- CiviCRM Components
serie: learn
---

To get Enabled CiviCRM components you can use :

```php?start_inline=1
$config = CRM_Core_Config::singleton();
$enableComponents = $config->enableComponents);
return in_array('CiviCase', $config->enableComponents);
```


To check if specific component is enabled :

```php?start_inline=1
$config = CRM_Core_Config::singleton();
$enableComponents = $config->enableComponents);
if (in_array('CiviCase', $config->enableComponents)) {
  // Do Stuff
}
```
---
layout: post
title:  "Get CiviCRM current file upload directory."
image: ''
date:   2016-11-01 00:06:31
tags:
- configurations
description: ''
categories:
- CiviCRM Config
serie: learn
---

To get current file upload directory : 

```php?start_inline=1
$config = CRM_Core_Config::singleton();
$uploadDir= $config->customFileUploadDir;
```

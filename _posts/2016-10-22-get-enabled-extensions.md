---
layout: post
title:  "Get Enabled Extension"
image: ''
date:   2016-10-22 00:06:31
tags:
- extensions
description: ''
categories:
- CiviCRM Extensions
serie: learn
---

To get Enabled CiviCRM components you can use :

```php?start_inline=1
$config = CRM_Core_Config::singleton();
$enableComponents = $config->enableComponents);
return in_array('CiviCase', $config->enableComponents);
```


To check if specific extension is enabled :

```php?start_inline=1
$isEnabled = CRM_Core_DAO::getFieldValue(
'CRM_Core_DAO_Extension',
'EXTENSION_KEY',
'is_active',
'full_name'
);
```

Where EXTENSION_KEY = you extension unique key , for example :

```php?start_inline=1
$isEnabled = CRM_Core_DAO::getFieldValue(
'CRM_Core_DAO_Extension',
'uk.co.compucorp.civicrm.tasksassignments',
'is_active',
'full_name'
);
```

You can find EXTENSION_KEY inside the extension *info.xml* file :

```xml
<?xml version="1.0"?>
<extension key="uk.co.compucorp.civicrm.tasksassignments" type="module">
  <file>tasksassignments</file>
  <name>Tasks and assignments</name>
```  

hence

```xml
key="uk.co.compucorp.civicrm.tasksassignments"
```
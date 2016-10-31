
---
layout: post
title:  "Get Extension Directory"
image: ''
date:   2016-11-01 00:06:31
tags:
- extensions
description: ''
categories:
- CiviCRM Extensions
serie: learn
---

To get extension base directory :

```php?start_inline=1
$extensionDirectory = CRM_Core_Resources::singleton()->getPath('EXTENSION_KEY');
```

Where EXTENSION_KEY = the extension unique key , for example :

```php?start_inline=1
$extensionDirectory = CRM_Core_Resources::singleton()->getPath('uk.co.compucorp.civicrm.tasksassignments');
$isEnabled = CRM_Core_DAO::getFieldValue(
'CRM_Core_DAO_Extension',
'uk.co.compucorp.civicrm.tasksassignments',
'is_active',
'full_name'
);
```

You can find *EXTENSION_KEY* inside the extension *info.xml* file :

```xml
<?xml version="1.0"?>
<extension key="uk.co.compucorp.civicrm.tasksassignments" type="module">
  <file>tasksassignments</file>
  <name>Tasks and assignments</name>
  .....
   ...etc
```  

hence

```xml
key="uk.co.compucorp.civicrm.tasksassignments"
```

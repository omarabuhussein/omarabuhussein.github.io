---
layout: post
title:  "Show Pop-Up notification"
image: ''
date:   2016-10-22 00:06:31
tags:
- session
description: ''
categories:
- CiviCRM Session
serie: learn
---

To Show a popup notification on any page :

```php?start_inline=1
$title = ts("Any Title");
$message = ts("Any Message");
$type = 'error'; // available types ( alert, info, success, error, no-popup )
 
CRM_Core_Session::setStatus($message, $title, $type)
```

Example :

```php?start_inline=1
$title = ts("Task Added");
$message = ts("A new task added successfuly");
$type = 'success';
 
CRM_Core_Session::setStatus($message, $title, $type)
```
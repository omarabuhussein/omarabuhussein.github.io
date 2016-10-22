---
layout: post
title:  "get Enabled Components"
image: ''
tags:
- components
description: '
categories:
- CiviCRM Components
serie: learn
---

To get Enabled CiviCRM components you can use :

{% highlight php %}
$config = CRM_Core_Config::singleton();
$enableComponents = $config->enableComponents);
return in_array('CiviCase', $config->enableComponents);
{% endhighlight %}


To check if specific component is enabled :

{% highlight php %}
$config = CRM_Core_Config::singleton();
$enableComponents = $config->enableComponents);
if (in_array('CiviCase', $config->enableComponents)) {
  // Do Stuff
}
{% endhighlight %}
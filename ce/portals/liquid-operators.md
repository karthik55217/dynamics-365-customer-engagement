---
title: "Use Liquid operators for a portal | MicrosoftDocs"
description: "Learn about the available liquid operators in a portal."
ms.custom: 
  - dyn365-portal
ms.date: 10/01/2019
ms.service: dynamics-365-customerservice
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: article
ms.assetid: ce9b5b7d-2756-4a8e-8fab-f64ec9c1e11a
ms.reviewer: ""
author: sbmjais
ms.author: shjais
manager: shubhadaj
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365Portals
---
# Understand Liquid operators

Liquid has access to all common logical and comparison operators. These can be used in tags such as **if** and **unless**.

## Basic operators

| ==    | Equals                          |
|-------|---------------------------------|
| !=    | Does not equal                  |
| &gt;  | Greater than                    |
| &lt;  | Less than                       |
| &gt;= | Greater than or equal to        |
| &lt;= | Less than or equal to           |
| or    | Condition A **or** condition B  |
| and   | Condition A **and** condition B |

## contains

contains tests for the presence of a substring within a string.

```
{% if page.title contains 'Product' %}

The title of this page contains the word Product.

{% endif %}
```

contains can also test for the presence of a string within an array of strings.

## startswith

startswith tests whether a string starts with a given substring.

```
{% if page.title startswith 'Profile' %}

This is a profile page.

{% endif %}
```

## endswith

endswith tests whether a string ends with a given substring.

```
{% if page.title endswith 'Forum' %}

This is a forum page.

{% endif %}
```

### See also

[Add dynamic content and create custom templates](custom-templates-dynamic-content.md)  
[Store source content by using web templates](store-content-web-templates.md)  
[Liquid types](liquid-types.md)  
[Conditional](liquid-conditional-operators.md)  
[Liquid Objects](liquid-objects.md)  
[Liquid Tags](liquid-tags.md)  
[Liquid Filters](liquid-filters.md)  
[Create advanced templates for portals](create-advanced-templates.md)  


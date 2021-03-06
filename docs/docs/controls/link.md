---
layout: default
title: The "link" control
slug: link
subtitle: Learn how to create controls using Kirki
mainMaxWidth: 55rem;
bodyClasses: control page
returns: string
heroButtons:
  - url: ../controls
    class: white button round border-only
    icon: fa fa-arrow-circle-o-left
    label: Back to Controls
---

The `link` control is a simple text-input control, with URL sanitization. Values are sanitized using the `esc_url_raw()` function.

### Example:

```php
Kirki::add_field( 'theme_config_id', [
	'type'     => 'link',
	'settings' => 'my_setting',
	'label'    => __( 'Link Control', 'textdomain' ),
	'section'  => 'section_id',
	'default'  => 'https://wplemon.com/',
	'priority' => 10,
] );
```

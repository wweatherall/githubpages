---
layout: default
---

## Executives

President: {{site.data.executives.President.name}}

Vice President: {{site.data.executives.Vice-President.name}}

Treasurer: {{site.data.executives.Treasurer.name}}

### General Inquiries:
[{{site.data.executives.President.email}}](mailto:{{-site.data.executives.President.email-}})

## For Sport Specific Inquiries

{% for item in site.data.navigation %}

### {{ item.name }}

{{ item.contactName }}:
[{{ item.contact }}](mailto:{{-item.contact-}})

{% endfor %}

## Mailing Address

PO Box 494\
Black Diamond, AB\
T0L 0H0

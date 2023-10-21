---
title: My markdown index!
layout: default
---

This is my index

U-13 is for players born in
{{ "now" | date: "%Y" | minus: 13 }} and {{ "now" | date: "%Y" | minus: 12 }}

*U5 is for players born in {{ "now" | date: "%Y" | minus: 5 }} and {{ "now" | date: "%Y" | minus: 4 }}*

- [ ] This is a test of this part

<script>document.write(new Date().getFullYear()-13);</script>

and <script>document.write(new Date().getFullYear()-12);</script>.
<p><script>document.write( new Date().getFullYear() );</script>
    <script type="text/javascript">document.write( new Date().getFullYear() );</script></p>

I hope this works.

Does this make a dif

$$ \pi r^2 $$

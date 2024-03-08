---
layout: post
title: OS X sleep and Hibernate
date: 2009-01-30
categories: []
tags: []
status: publish
type: post
published: true
meta:
---
<div class="entry-content"><h4>To view current hibernation mode: (default for portables is 3, desktops use 0)</h4>
<blockquote>
<p><code>pmset -g|grep hibernatemode</code></p>
</blockquote>
<h4>sleep (3): save to RAM, until low battery, then hibernate</h4>
<blockquote>
<p><code>sudo pmset -a hibernatemode 3</code></p>
</blockquote>
<h4>hibernate (1): save directly to disk, consumes no power (can even remove battery?)</h4>
<blockquote>
<p><code><b>sudo pmset -a hibernatemode 1</b></code></p>
</blockquote>
<h4><b>hibernation disabled (0): goes to sleep, dies without power</b></h4>
<blockquote>
<p><code><b><b>sudo pmset -a hibernatemode 0 </b></b></code></p>
</blockquote>
</div>

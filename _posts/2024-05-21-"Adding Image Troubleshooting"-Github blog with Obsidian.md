---
layout: single
title: '"Adding Image Troubleshooting"-Github blog with Obsidian'
categories:
  - Tips
tags: 
toc: true
author_profile: true
aliases: 
connected:
---
## Obsidian + Web page image upload
Normally when we added images into the obsidian file, the format is like  `![[files/image]]`
But if you just leave it like that, at your webpage will show you nothing.

So, by changing the format like this
`![thejourneyofbabo](../files/image)`
can make it seen at your website.
## But.. when you added Category..
>It didn't work!

So, How can we solve this problem?
first what I tried is
`![thejourneyofbabo]({{site.url}}/files/image)`
It worked at the web page. But unfortunately, from your page preview at Obsidian will not work. It'll show you like "/files/image” could not be found."

Is there any way to solve this problem in both places?
And I found the format `![](../../files/image)` like this.
`../../` is the key.

Than you can see the lovely image either from your Obsidan pages and your website.
Happy:)
![](../../files/jslogo.jpg)
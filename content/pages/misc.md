---
title: "Misc Notes"
description: "These are your workshops"
menu:
  main:
    weight: 1
---


# Sample ordinary text

## Well, Mercia's a temperate zone!

Knights of Ni, we are but simple travelers who seek the enchanter who lives beyond these woods. How do you know she is a witch? We shall say 'Ni' again to you, if you do not appease us. The Knights Who Say Ni demand a sacrifice!

1. Bloody Peasant!
1. How do you know she is a witch?
1. Well, Mercia's a temperate zone!


# Embed a Youtube video 

Use syntax `youtube` followed by video id enclosed in two sets of curly braces and one set of pointy braces. 

{{< youtube Q2qg9TJm4Kk >}}

# Use shortcode to include blocks in this page.

## Include local data 

The text below is from the `test_local_data.html` file in the `layouts/shortcodes` directory.  It is set to take positional arguments.
It also uses data from feeds.carpentries.org to build a list of data. 

{{< test_local_data "mentos the freshmaker" "is da bomb" >}}

## Include remote data 

{{< test_remote_data "is_maintainer" >}}
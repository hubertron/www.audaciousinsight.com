---
title: CURL command to act as a mobile device
date: '2017-01-17 15:13:54'
layout: post
---
Say you are debugging a site on mobile and for whatever reason it is an endless redirect loop. An easy way to diagnose this is with the following command:

```curl -A "Mozilla/5.0 (iPhone; U; CPU iPhone OS 4_3_3 like Mac OS X; en-us) AppleWebKit/533.17.9 (KHTML, like Gecko) Version/5.0.2 Mobile/8J2 Safari/6533.18.5" -IL http://google.com```

The -A lets you set the User Agent string
The -I shows just headers
The -L says to follow redirects.

Check it out and enjoy!
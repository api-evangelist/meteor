---
title: "Meteor 3.4 dev: build tool leaks rspack server bundle + source-map SourceNodes on every rebuild → OOM"
url: "https://forums.meteor.com/t/meteor-3-4-dev-build-tool-leaks-rspack-server-bundle-source-map-sourcenodes-on-every-rebuild-oom/64651"
date: "2026-06-04"
author: "a4xrbj1"
feed_url: "https://forums.meteor.com/latest.rss"
---
In Meteor 3.4.1 dev mode, the meteor build-tool process leaks the rspack-generated server bundle and its source-map SourceNode graph on every incremental rebuild (“ => Server modified -- restarting... ”). Nothing from the previous compilation is released, so the tool process grows ~linearly with the number of rebuilds and eventually dies with: FATAL ERROR: Ineffective mark-compacts near heap limit Allocation failed - JavaScript heap out of memory This is the meteor-tool process (the one launched at ~/.meteor/meteor with --max-old-space-size=4096 ), not the application server — confirmed by the

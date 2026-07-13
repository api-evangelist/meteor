---
title: "Outdated mongodb driver dependency in @types/meteor package"
url: "https://forums.meteor.com/t/outdated-mongodb-driver-dependency-in-types-meteor-package/64608"
date: "2026-05-15"
author: "waldgeist"
feed_url: "https://forums.meteor.com/latest.rss"
---
The current @types/meteor package sets a dependency to "mongodb": "^4.3.1" However, since Meteor 3.1, Meteor uses mongodb 6.10.0 / 6.9.0: gist.github.com https://gist.github.com/Grubba27/ae928cba5772c9bc5ac5287fa240388a table.md | Meteor | MongoDB Driver | Latest Compatible MongoDB | MongoDB with all features | Oldest supported MongoDB | | :-------: | :----------: | :-----------------------: | :---------------------: | :--------------------: | | 3.3 | 6.9.0 | 8.0 | 8.0 | 3.6 | | 3.2 | 6.9.0 | 8.0 | 8.0 | 3.6 | | 3.1 | 6.10.0 | 8.0 | 8.0 | 3.6 | | 3.0 | 4.17.2 | 8.0 | 6.0 | 3.6 | | 2.15 | 4.17.

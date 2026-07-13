---
title: "Post-Fibers: can core server packages ship native async instead of transpiled generators? (async stack traces)"
url: "https://forums.meteor.com/t/post-fibers-can-core-server-packages-ship-native-async-instead-of-transpiled-generators-async-stack-traces/64686"
date: "2026-07-06"
author: "hexsprite"
feed_url: "https://forums.meteor.com/latest.rss"
---
I hit a debugging wall in a Meteor 3.4 app and want to sanity-check the build-target reasoning before I open an issue, in case I’m missing something obvious. A publication threw on the server. Here’s the entire stack trace that reached my error tracker: TypeError: Cannot read properties of null (reading 'id') at asyncGeneratorStep (programs/server/packages/ddp-server.js:255) at _throw (programs/server/packages/ddp-server.js:276) at Subscription.error (packages/ddp-server/livedata_server.js:970) ...

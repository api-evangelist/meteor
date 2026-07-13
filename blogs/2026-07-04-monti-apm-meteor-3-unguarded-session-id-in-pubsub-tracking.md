---
title: "Monti APM (Meteor 3): unguarded session.id in pubsub tracking crashes on mid-publish disconnects"
url: "https://forums.meteor.com/t/monti-apm-meteor-3-unguarded-session-id-in-pubsub-tracking-crashes-on-mid-publish-disconnects/64683"
date: "2026-07-04"
author: "a4xrbj1"
feed_url: "https://forums.meteor.com/latest.rss"
---
Hi @zodern flagging a small-but-live Meteor 3 bug in montiapm:agent that’s worth a quick patch release, since it affects any Meteor 3 app running Monti in production. Symptom (production): TypeError: Cannot read properties of null (reading 'id') at PubsubModel._trackReady (montiapm:agent/lib/models/pubsub.js:89) at Subscription. (montiapm:agent/lib/hijack/wrap_subscription.js:46) at Subscription.ready (ddp-server/livedata_server.js:1008) It fires as an unhandledRejection, so it doesn’t crash the process, but it lands as a status:error in APM/DataDog and pollutes error monitoring.

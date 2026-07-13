---
title: "SRI hashes are sometimes not valid"
url: "https://forums.meteor.com/t/sri-hashes-are-sometimes-not-valid/64667"
date: "2026-06-19"
author: "a4xrbj1"
feed_url: "https://forums.meteor.com/latest.rss"
---
github.com/meteor/meteor SRI hashes are sometimes not valid opened 01:34AM - 25 Sep 19 UTC mitar confirmed idle Running on Meteor 1.8.1 on Linux. Reproduction: https://github.com/mitar/mete … or-issue10710 If you run it and open in the browser, you should see in Chrome an error like this; ``` Failed to find a valid digest in the 'integrity' attribute for resource 'http://localhost:3000/packages/akryum_vue-component-dev-client.js?hash=547603629037ec5c040db59841e0ae93a1918dcb' with computed SHA-256 integrity 'XAccToISWRkBlpCrMQXQr5epxqzYxV1ewlltT+Wowdg='. The resource has been blocked. ``` I hav

---
title: "Anyone else running into this? Symbol.iterator polyfill in ecmascript-runtime-client breaks native iterator protocol on the client"
url: "https://forums.meteor.com/t/anyone-else-running-into-this-symbol-iterator-polyfill-in-ecmascript-runtime-client-breaks-native-iterator-protocol-on-the-client/64600"
date: "2026-05-12"
author: "drone1"
feed_url: "https://forums.meteor.com/latest.rss"
---
Symbol.iterator polyfill in ecmascript-runtime-client breaks native iterator protocol on the client Versions Meteor : METEOR@3.4 ecmascript-runtime-client : 0.12.3 core-js (transitive, bundled): 3.47.0 @meteorjs /rspack : 1.0.2 (modern web targets only) Symptom On the client, any code that uses the native iterator protocol on a built-in iterator — for (const x of arr.entries()) , for (const [k, v] of map.entries()) , for (const v of map.values()) , etc. — can throw at runtime: TypeError: b.entries is not a function or its return value is not iterable at … in our app bundle The first part of th

---
title: "Errors when building with meteor V3.4.1 using Rspack"
url: "https://forums.meteor.com/t/errors-when-building-with-meteor-v3-4-1-using-rspack/64622"
date: "2026-05-25"
author: "willemx"
feed_url: "https://forums.meteor.com/latest.rss"
---
I have just upgraded a project to meteor V3.4.1 and now I am using meteor build to create a deployment bundle. Building succeeded fine right after upgrading. Also when I added "meteor: {"modern": true} to package.json building with SWC went fine. However, when I tried to use rspack, the build process failed with lots of WARNINGS like this: WARNING in ./node_modules/node-aead-crypto/lib.js 32:37-75 ⚠ Module not found: Can't resolve './node-aead-crypto.android-arm64.node' in '/Users/willem/meteor/ctrlh/node_modules/node-aead-crypto' ╭─[32:28] 30 │ try { 31 │ if (localFileExisted) { 32 │ nativeBi

---
title: "Kmp-ddpclient — a Kotlin Multiplatform DDP client, now open source"
url: "https://forums.meteor.com/t/kmp-ddpclient-a-kotlin-multiplatform-ddp-client-now-open-source/64728"
date: "2026-08-05"
author: "osrl"
feed_url: "https://forums.meteor.com/latest.rss"
---
I’ve open-sourced the DDP client we’ve been running in production for the last two years in our Android + iOS app. Repo: GitHub - bordoio/kmp-ddpclient: Kotlin Multiplatform client for Meteor's DDP protocol — websocket connection management, subscriptions with an in-memory minimongo mirror, and method calls as coroutine Flows. · GitHub Subscriptions feed a local minimongo mirror you observe as coroutine Flow s, so collections stay in sync the way they do on the client.

---
title: "Is anyone else having login problems with passwordless after entering tokens with version 3.5?"
url: "https://forums.meteor.com/t/is-anyone-else-having-login-problems-with-passwordless-after-entering-tokens-with-version-3-5/64705"
date: "2026-07-23"
author: "a4xrbj1"
feed_url: "https://forums.meteor.com/latest.rss"
---
I’m still investigating what’s causing it and where it exactly stalls but it could be related to upgrading to Meteor 3.5 from 3.4.1 - has anyone else using passwordless and is experiencing the following: Login never reached data-ready — and the client onLogin hook runs after data-ready, so it never even ran (loginSuccessful was never called) ? Will update this thread when I get more information from instruments. 3 posts - 2 participants Read full topic

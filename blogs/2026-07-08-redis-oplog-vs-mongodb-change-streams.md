---
title: "Redis oplog vs MongoDB change streams"
url: "https://forums.meteor.com/t/redis-oplog-vs-mongodb-change-streams/64690"
date: "2026-07-08"
author: "necmettin"
feed_url: "https://forums.meteor.com/latest.rss"
---
I have been following Meteor for years, and I always had my reservations about MongoDB oplog tailing. As I understand it, with the release of Meteor 3.5, oplog tailing has been replaced by change streams. I have always thought Meteor would benefit from moving oplog tailing to Redis, and after seeing the redis-oplog package, I assumed the Meteor team would see the benefit in using Redis for change tracking and maybe integrate redis-oplog officially to Meteor.

---
title: "Significant speedup Meteor build process inside Docker"
url: "https://forums.meteor.com/t/significant-speedup-meteor-build-process-inside-docker/64681"
date: "2026-06-28"
author: "klaucode"
feed_url: "https://forums.meteor.com/latest.rss"
---
I’m sending this post just for info. I multiple times tested building process in same way in Docker container and on same host system and the result was always the same. Building process inside the Docker was multiple times - 5x and more slower, than run the same process on host system. Cache, resources limitation or another recommendations was not a problem. I tries the performance tests and the result was, that there was not signifficant difference between docker and host system, therefore the idea was, the reason why the building process is so slow in docker is filesystem. I tried to update

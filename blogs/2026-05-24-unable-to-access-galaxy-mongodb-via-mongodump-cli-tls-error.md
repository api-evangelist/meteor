---
title: "Unable to access Galaxy mongodb via mongodump CLI (TLS error)"
url: "https://forums.meteor.com/t/unable-to-access-galaxy-mongodb-via-mongodump-cli-tls-error/64619"
date: "2026-05-24"
author: "trusktr"
feed_url: "https://forums.meteor.com/latest.rss"
---
Trying to connect to mongodb from external, using mongodump , results in this error (formatted for readability): ~ ❯ mongodump --uri="mongodb://USERNAME_REDACTED:PASSWORD_REDACTED@galaxyadmin_galaxyfreedb-01.mongodb.galaxy-cloud.io:30025,galaxyadmin_galaxyfreedb-02.mongodb.galaxy-cloud.io:30025,galaxyadmin_galaxyfreedb-03.mongodb.galaxy-cloud.io:30025/myapp-meteorapp-com?replicaSet=galaxyadmin_galaxyfreedb&ssl=true" --archive=db.gz --gzip 2026-05-24T12:46:48.376-0700 Failed: can't create session: failed to connect to mongodb://USERNAME_REDACTED:PASSWORD_REDACTED@galaxyadmin_galaxyfreedb-01.mon

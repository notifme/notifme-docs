---
layout: default
title: Curl example
---

### Curl example
```shell
curl -X POST \
  https://[app].notif.me/api/notification \
  -H 'authorization: your-api-token' \
  -H 'content-type: application/json' \
  -d '{
    "toUserId": "your-user-id",
    "to": {
      "email": "demo@notif.me"
    },
    "template": {
      "name": "welcome",
      "channels": {
        "email": {
          "domain": "[app].notif.me",
          "from": "team@[app].com",
          "subject": "Welcome!",
          "html": "Hi {% raw %}{{name}}{% endraw %}, welcome to our service!"
        }
      }
    },
    "params": {"name": "James"}
  }'
```


```javascript
const x = 78;
```

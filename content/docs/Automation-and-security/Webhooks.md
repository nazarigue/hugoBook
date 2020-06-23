---
bookCollapseSection: true
bookFlatSection: false
weight: 1
title: Webhooks
---

# Webhook is a way to send structured data to other service

Slack example, more information check on their [website](https://api.slack.com/messaging/webhooks "Webhooks Slack")

This particular piece is sending message to specific url, that will accept it, if authorised.

```javascript
POST https://hooks.slack.com/services/T00000000/B00000000/XXXXXXXXXXXXXXXXXXXXXXXX
Content-type: application/json
{
    "text": "Hello, world."
}
```


But in order to receive the message, you should allow the webhook.

```javascript

{
    "ok": true,
    "access_token": "xoxp-XXXXXXXX-XXXXXXXX-XXXXX",
    "scope": "identify,bot,commands,incoming-webhook,chat:write:bot",
    "user_id": "XXXXXXXX",
    "team_name": "Your Workspace Name",
    "team_id": "XXXXXXXX",
    "incoming_webhook": {
        "channel": "#channel-it-will-post-to",
        "channel_id": "C05002EAE",
        "configuration_url": "https://workspacename.slack.com/services/BXXXXX",
        "url": "https://hooks.slack.com/TXXXXX/BXXXXX/XXXXXXXXXX"
    }
}
```

Message will be accepted and it will be posted to defined channel:

![](https://a.slack-edge.com/80588/img/api/messaging_getting_started_threading.png)

Webhooks logic works everywhere and is defined by POST PUT GET DELETE mehtods. It's fundamental to what Zapier does and other automaton tools. This is basis.
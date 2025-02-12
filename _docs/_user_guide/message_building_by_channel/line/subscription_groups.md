---
nav_title: Subscription Groups
article_title: Subscription Groups
page_order: 3
description: "This article covers LINE message subscription groups."
page_type: reference
channel:
 - LINE
hidden: true
permalink: /line/subscription_groups/
---

# LINE subscription groups

> There are two subscription states for LINE users: subscribed and unsubscribed. LINE can have up to 100 subscription groups per workspace, with each subscription group connected to its own LINE channel.<br><br>This article is part of the LINE beta collection. [Return to main page](https://www.braze.com/docs/line/).

{% alert important %}
LINE access is in beta and only available in select Braze packages. Reach out to your account manager or customer success manager to get started.
{% endalert %}

| State | Definition |
| --- | --- |
| Subscribed | The user followed the LINE channel from within their LINE app. Users are automatically subscribed when they follow after you've completed the integration steps. |
| Unsubscribed | The user didn't follow the LINE channel from within their LINE app, or the user explicitly unfollowed the LINE channel. <br><br> Users who unsubscribe from a LINE subscription group will no longer receive any LINE messages from sending channels that belong to the subscription group. |
{: .reset-td-br-1 .reset-td-br-2 }

## Setting a user's LINE subscription group

LINE hosts the users' subscription status. Braze processes the follow and unfollow events that update the subscription status.
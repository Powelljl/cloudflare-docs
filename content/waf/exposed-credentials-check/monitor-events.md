---
pcx-content-type: concept
title: Monitor exposed credentials events
weight: 6
---

# Monitor exposed credentials events

The Firewall **Activity log** contains entries for requests with exposed credentials identified by rules with the _Log_ action.

Check for exposed credentials events in the Firewall Analytics dashboard (**Security** > **Overview** tab), filtering by a specific Rule ID. For more information on filtering Firewall events, refer to [Adjusting displayed data](/waf/analytics/paid-plans/#adjusting-displayed-data).

{{<Aside type="warning" header="Important">}}

Exposed credentials events are only logged after you activate the Exposed Credentials Check Managed Ruleset or create a custom rule checking for exposed credentials.

The log entries will not contain the values of the exposed credentials (username, email, or password). However, if [matched payload logging](/waf/managed-rulesets/payload-logging/) is enabled, the log entries will contain the values of the fields in the rule expression that triggered the rule. These values might be the values of credential fields, depending on your rule configuration.

{{</Aside>}}

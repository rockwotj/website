---
description: Set alerts in Redash to get an update about your queries' status every time they run.
---

# Alert Status and Frequency

The alert status is checked every time the query is executed - alerts work only with scheduled queries.

Alerts have 3 status types:
1. Triggered - the value you set the alert for is triggered (if you set your alert to trigger when the value of "cats" is greater than 1500 as long as it's above 1500 your alert is triggered)
2. OK - the value you have set to trigger the alert is not reached for now (might happen after the alert was triggered or before it was ever triggered, if your "cats" value is now 1470 your alert will show as OK)
3. Unknown - you should see this status once you have set your alert and it wasn't yet checked. To make your alert in the know, run the query it is linked to after setting the alert.

## Get an Alert Upon Status Change

Leaving the REARM value empty will cause alerts to be sent only when the status changes (from OK to Triggered or vice versa).

## Get an Alert Everytime the Query Runs

To get an alert every time the query runs set the REARM value  - the value is for seconds that pass since the system detects a change until it sends the alert, a 1 minute "delay" would require entering '60' in the REARM field.

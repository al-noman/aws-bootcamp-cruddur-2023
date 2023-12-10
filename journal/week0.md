# Week 0 — Billing and Architecture

## Homework challenges
### Use EventBridge to hookup Health Dashboard to SNS and send notification when there is a service health issue
In order to solve this challenge I performed the following steps from AWS console:
1. Create a SNS topic:
   ![SNS topic with subscriber](assets/target_sns_topic_and_subscriber.png)

2. Create an EventBridge rule and use the SNS topic from the previous step as a `Target` for that rule
   ![Event bridge rule with event pattern to get data from AWS health dashboard](assets/event_bridge_rule_setup.png)
   ![Event bridge target to the SNS topic](assets/event_brdige_target.png)


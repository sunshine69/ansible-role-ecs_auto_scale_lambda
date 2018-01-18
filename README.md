# ecs_event_monitor_lambda

Creates a lamdba that monitors for ECS being
unable to allocate a service and fires an alarm

# Variables

* `ecs_event_cloudwatch_alarm` - ARN of the cloudwatch alarm
  that should be triggered when needing to autoscale

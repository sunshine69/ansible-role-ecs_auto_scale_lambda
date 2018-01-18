# ecs_event_monitor_lambda

Creates a lamdba that monitors for ECS being
unable to allocate a service and fires an alarm

# Variables

* `ecs_event_cloudwatch_alarm` - ARN of the cloudwatch alarm
  that should be triggered when needing to autoscale

# Requirements

Needs an implementation of `plugins/action/aws_s3.py` (note
that 2.5 action plugins don't work with 2.4 without removing
`AnsibleAction` import and changing `except AnsibleAction` to
`except AnsibleActionFail`)

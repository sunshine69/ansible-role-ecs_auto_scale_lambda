# ecs_auto_scale_lambda

Creates a lamdba that updates ECS Agent desired
count when unable to allocate a service

# Variables


# Requirements

Needs an implementation of `plugins/action/aws_s3.py` (note
that 2.5 action plugins don't work with 2.4 without removing
`AnsibleAction` import and changing `except AnsibleAction` to
`except AnsibleActionFail`)

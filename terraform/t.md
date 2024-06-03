1. Go to the Amazon CloudWatch console
2. In the left navigation pane, click on "Log groups"
3. Click on "Create log group"
4. For "Log group name", enter "/ecs/my-first-task"
5. Click "Create log group"

If you don't have permissions to create a log group, contact your AWS Administrator to grant the following permissions:

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow", 
            "Action": [
                "logs:CreateLogGroup"
            ],
            "Resource": "arn:aws:logs:*:*:log-group:/ecs/my-first-task"
        }
    ]
}
```
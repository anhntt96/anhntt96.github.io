# CloudFormation

### CloudFormation Stack Protection
1. Termination protection
2. Stack-level policy
3. Resource-level policy
4. IAM policy

Exercise:
- https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-protect-stacks.html
- https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/protect-stack-resources.html

### CloudFormation Drift Detection and Remediation
1. Detection steps:
   - Use the management console or CLI to detect drift
   - With AWS Config, the Config rule cloudformation-stack-drift-detection-check can be run to detect drift on our stack.

2. Steps to fix:
   - Evaluate drift details and decide to revert or keep changes.
   - Use stack updates to eliminate drift.


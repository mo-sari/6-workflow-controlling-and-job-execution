Conditional functions:
- failure() ==> true if any previous step or job failed
- success() ==> true is none of previous steps failed
- always() ===> Causes the step to always run, even when cancelled
- cancelled() ==> true if the workflow has been cancelled

When a continue-on-error step fails, the outcome is failure, but the final conclusion is success.
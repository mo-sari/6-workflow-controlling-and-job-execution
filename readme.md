Conditional functions:
- failure() ==> true if any previous step or job failed
- success() ==> true is none of previous steps failed
- always() ===> Causes the step to always run, even when cancelled
- cancelled() ==> true if the workflow has been cancelled

When a continue-on-error step fails, the outcome is failure, but the final conclusion is success.

we could just write the name of our artifact inside the reusable workflow, but that is not a reusable workflow anymore if we do so, so we have to provide it with inputs
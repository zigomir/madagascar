# Welcome to Madagascar!

Adjusted the 'environment' name to lowercase, in case that was blocking the Sleuth Action from completing.

Testing the new workflow with Sleuth Actions:
- AT-4 in status "Backlog"
- AT-5 in status "In Progress"
- AT-6 in status "Done"

Re-running the last test.

Last test successful. 

Testing the workflow with the added rule to restrict transitions when a condition is not met (field 'Approved' must be filled in):
- AT-1 in status "Done" and "Approved" = "Yes"
- AT-5 in status "Done" and "Approved" = empty

Test again.

Testing after fix released to production:
- AT-4 in status "Done" and "Labels" = empty
- AT-5 in status "Done" and "Labels" = "Website"
- AT-7 in status "Backlog" and "Labels" = empty

Testing with the JMWE validator in place.
- KJ-1 in status "Done" and "Labels" = empty
- KJ-2 in status "Done" and "Labels" = "Website"
- KJ-3 in status "Backlog" and "Labels" = "Website"

Testing Slack notifications for failed rules again.

Testing Slack notifications for failed rules with:
- KJ-1 in status "Done" and "Labels" = "Website"

- KJ-3 in status "Backlog" and "Labels" = "Website"

This is to test if the rules actually refresh upon deploy.

Trying Ines's suggestion !=0 (updated the YML file now)

Testing with a deployed for >5m delay. Reduced the delay to >3m and updated the message to include deploy URL.

Testing with the deploy_slack variable. Forgot to refresh the rules.

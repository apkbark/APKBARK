# APKLUB-Extension-Code

Automatically close stale Issues and Pull Requests that tend to accumulate during a project.

How it works
After a period of inactivity, a label will be applied to mark an issue as stale, and optionally post a comment to notify contributors that the Issue or Pull Request will be closed.

If the Issue or Pull Request is updated, or anyone comments, then the stale label is removed.

If no more activity occurs, the Issue or Pull Request will be automatically closed with an optional comment.

Installation
After installing the app, create .github/stale.yml in the default branch to enable it:

# Number of days of inactivity before an issue becomes stale
daysUntilStale: 60
# Number of days of inactivity before a stale issue is closed
daysUntilClose: 7
# Issues with these labels will never be considered stale
exemptLabels:
  - pinned
  - security
# Label to use when marking an issue as stale
staleLabel: wontfix
# Comment to post when marking an issue as stale. Set to `false` to disable
markComment: >
  This issue has been automatically marked as stale because it has not had
  recent activity. It will be closed if no further activity occurs. Thank you
  for your contributions.
# Comment to post when closing a stale issue. Set to `false` to disable
closeComment: false

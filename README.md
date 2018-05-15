# git-hooks

Git hooks that we are using.

## post-redmine-comment

Post comment to a redmine issue. It extracts id of the linked issue from the last commit message using next pattern:

```
"refs #ISSUE_ID; ...".
```

Also, you must set `REDMINE_API_TOKEN` environment variable.

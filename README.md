# git-hooks

Git hooks we are using.

## Requirements

`ruby 2.4.1+`

## Example installation:

```
git clone https://github.com/websecret/git-hooks /tmp/git-hooks
cp /tmp/git-hooks/validate-commit-message .git/hooks/commit-msg
chmod +x .git/hooks/commit-msg
```

## post-redmine-comment

Post comment to a redmine issue. It extracts id of the linked issue from the last commit message using next pattern:

```
"refs #ISSUE_ID; ..."
```

Also, you must set `REDMINE_API_TOKEN` environment variable.

## validate-commit-message

`commit-msg` hook that validates commit message.

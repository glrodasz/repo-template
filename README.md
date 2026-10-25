# repo-template

Starting point for new repositories, with secure defaults:

- `.github/CODEOWNERS`: every change, including `.github/`, needs review from @glrodasz.
- `.github/dependabot.yml`: monthly grouped updates for GitHub Actions, with a 7-day cooldown.
  Uncomment the `npm` block for JS/TS projects.
- `SECURITY.md`: points reporters to private vulnerability reporting.

Templates copy files, not settings. Branch rules and repo settings are applied by
`harden-repos.sh`.

## Using it

```bash
gh repo create my-new-repo --template glrodasz/repo-template --public --clone
```

After creating the repo, replace this README.

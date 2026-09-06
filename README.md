# LeaderWork

This repository holds the public organization profile for
[github.com/LeaderWork](https://github.com/LeaderWork).

| What | Where |
|---|---|
| Profile page shown on the org home | [`profile/README.md`](profile/README.md) |
| Org settings (description, website, location) | [`org-profile.json`](org-profile.json), applied with [`scripts/apply-org-profile.sh`](scripts/apply-org-profile.sh) |

## Organization settings

GitHub keeps an organization's description, website, and location in org
settings rather than in a repository, so this repo records the intended values
and ships a script that applies them.

| Field | Value |
|---|---|
| Display name | LeaderWork |
| Description | Great leaders create thriving organizations. Leader development and leadership-process consulting grounded in decades of real operating experience. |
| Website | https://leader-work.com |
| Location | Zeeland, MI |

To apply, an org owner runs the following from a machine with an authenticated
[GitHub CLI](https://cli.github.com):

```sh
./scripts/apply-org-profile.sh --dry-run   # preview
./scripts/apply-org-profile.sh             # apply
```

Edit `org-profile.json` first when the values need to change, then re-run the
script so the repo and the org settings stay in step.

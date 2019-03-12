# irredeemables
## General abuse list for filtering from frontends via hivemind

This repository contains the abuser (irredeemables) username list for the [Hivemind](https://github.com/steemit/hivemind) application.

The users in the `irredeemables` list will have their comments filtered out and their flags will not be considered in the logic that determines if comments or posts are hidden in most front end applications including [Condenser](https://github.com/steemit/condenser) (the software that powers steemit.com).

## Update Procedure

1. Make a new branch
2. Check in file using `YYYYMMDD.filename.txt` format (optionally removing old version)
3. Run `make` to regenerate `full.txt` (which is derived data and technically shouldn't be in git, but the file is actually fetched from `github.com` by redeemer so the full list needs to be in git). Note: the sorting of the records in the full.txt file uses "C" collation.
4. Create a pull request to `master`. All pull requests must include sufficient documented proof for a reviewer to conclude (without a doubt) that an account is violating our ToS or otherwise behaving in a way that would be considered abuse.

# Hotfix policy

Each scverse core package is maintained by one or multiple core developers who merge pull requests and make releases. 
While all core team members are welcome to contribute to all repos, it is typically the realm of the maintaiers
to review and merge pull requests. The purpose of this document is to document under which circumstances we 
deviate from this rule and to the process we adhere to. 

**If a critical fix is required for any core package (security issue, package not installable, CI breaks, ...)
other core team members are allows to make required fixes and make a patch release.** Please adhere to the following rules: 
 * Reach out to the maintainer(s) first. Depending on the severity of the issue give them one business day to react.
 * Four-eye principle: find another developer to review your pull request with the fixes.
 * Only fix what is absolutely necessary. Do not add new features or refactor the codebase. 

## Documenting release process

A prerequisite for others to make a release of the package is that the release process is properly documented
and permissions are properly set. Releases to PyPI are to be automated via GitHub actions using 
a [trusted publishing](https://docs.pypi.org/trusted-publishers/) workflow. 



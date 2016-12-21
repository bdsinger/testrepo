# testrepo
For improving my jenkins and github fu.
That might change depending on how it is repurposed.

Nothing to see here if you aren't me!

## Some things learned about github push webhooks
  - Push webhooks received from github during pull request (PR) process:
    - When **user-patch-num** branch is created by a PR
      - Filter using *branch specifier* in jenkins config
    - When merged, for the branch being updated
      - This is a relief. No need to deal with PRs at all
        if you just want to build iff the PR is accepted
    - for a git push, by definition

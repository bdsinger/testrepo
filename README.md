# testrepo
For improving my jenkins and github fu.
That might change depending on how it is repurposed.

Nothing to see here if you aren't me!

## Some things learned about github push webhooks
  - Push webhooks received from github during pull request (PR) process:
    - When **user-patch-num** branch is created when starting PR
      - On github when editing this README.md, for instance:
        - The webhook is triggered when **Propose file change** button is pushed
        - *Not* when **Create pull request** button is pushed
      - To skip building, filter using *Branch specifier* in Jenkins configuration
    - When PR is merged, for the branch being updated
      - This is a relief. Do not have to inspect PR trigger payload, or know it was a PR at all.
        
    - Fires for a git push by definition.

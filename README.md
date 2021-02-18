# github-actions-test

Usefule links:

https://docs.github.com/en/actions/managing-workflow-runs/enabling-debug-logging

https://docs.github.com/en/actions/managing-workflow-runs#enabling-debug-logging

https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#using-a-specific-shell

https://github.com/actions/hello-world-javascript-action

https://github.com/marketplace/actions/checkout

Event Trigger Workflows:\
https://docs.github.com/en/actions/reference/events-that-trigger-workflows
    By Default: pull-request wil trigger pipeline on open, reopen, and synchronize. Some events have activity type, so instead of passing values of "on:" as an array, we can pass as object and add activity types.  

Cron is use for scheduling:\
https://crontab.guru/ \
https://crontab.guru/examples.html \

External Event Trigger: \
https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event \
ex:curl -X POST --user "teodik:{PTA}" -H "Accept: application/vnd.github.v3+json" -d "{\"event_type\": \"build\"}" https://api.github.com/repos/teodik/github-actions-test/dispatches \
EX: curl -X POST --user "teodik:{token}" -H "Accept: application/vnd.github.v3+json" -d "{\"event_type\": \"build\", \"client_payload\":{\"Repositories\": \"tcom,lcom\"}}" https://api.github.com/repos/teodik/github-actions-test/dispatches \

Filtering workflaws by branches, tags, and paths
https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet \

Environment Variables: \
https://docs.github.com/en/actions/reference/environment-variables
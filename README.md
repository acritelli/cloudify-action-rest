This blueprint example shows how to run a GitHub Actions workflow from Cloudify and wait until it completes. The example blueprint runs the following pipelines, which are all just simple scripts:

* run-basic-script pipeline: Runs a [basic script](./workflow_scripts/basic_script.sh) that has no delay
* run-script-with-delay: Runs a [script with an artificial delay](./workflow_scripts/script_with_delay.sh) to demonstrate how the logic works to wait for completion

The "wait until workflow is completed" logic is complicated by the nature of GitHub's API.


Caveat

The workflow that you are attempting to run must have been run at least once.

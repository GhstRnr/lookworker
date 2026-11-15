# lookworker

## Launch a Copilot agent

The `launch-agent` workflow runs a Copilot coding agent on a task you provide:

1. Add a repository Actions secret named `COPILOT_GITHUB_TOKEN` with a Copilot-enabled token.
2. Open **Actions** → **Launch a Copilot coding agent** → **Run workflow**.
3. Enter the task description and start the run.

The agent can propose changes only through a draft pull request; it cannot merge the pull request. The workflow source is `.github/workflows/launch-agent.md`, and its compiled Actions workflow is `.github/workflows/launch-agent.lock.yml`. Recompile the lock file after changing the source with `gh aw compile`.
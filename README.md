# powershell-devops

PowerShell module for dealing with commands in Azure DevOps Pipelines and GitHub Workflows.

## Set-EnvironmentVariable

Sets the environment variable for the current process and optionally marks it as a secret.

```powershell
set-env MY_VALUE 'Hello World!'
```

*Note: `set-env` is an alias for `Set-EnvironmentVariable`.*

## Test-AdoPipeline

Returns true if running in an Azure DevOps Pipeline, determined by the environment variable `TF_BUILD` having a value.

```powershell
Test-AdoPipeline
```

## Test-GitHubWorkflow

Returns true if running in a GitHub Workflow, determined by the environment variable `GITHUB_ACTIONS` having a value.

```powershell
Test-GitHubWorkflow
```

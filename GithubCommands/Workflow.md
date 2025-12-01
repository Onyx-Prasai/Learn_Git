## Github Workflows

GitHub Workflows are one of the powerful feature of github actions that helps to automate taks such as building,testing and deploying your directly from your Github repository. Workflows are highly customizable, allowing you to create automated processes that fit your specific projects needs. 

<br>

## What are GitHub Workflows?
It is simply cutomizable or configurable automated process made up for one or more tasks that run on Github Actions. Workflows are usually defined in YAML files stored in the .github/workflows/ directory of your repository.

<br>

## Anatomy of a workflow (the parts you’ll use)
# Top-level keys

name: — friendly name of the workflow.

on: — triggers (events that start the workflow): e.g. push, pull_request, workflow_dispatch (manual), schedule (cron), workflow_call (reusable). 

jobs: — one or more jobs that run (possibly in parallel).

# Jobs
Each job runs on a runner (runs-on:). Runners can be GitHub-hosted (e.g. ubuntu-latest, windows-latest) or self-hosted. Jobs contain steps that run in order. Steps can:

run shell commands with run:,

or call an action with uses: (e.g. uses: actions/checkout@v4). 
GitHub

# Steps & Actions

Actions are reusable units of work (published on GitHub Marketplace or in repos).

Steps can set env, copy files, run scripts, etc. Steps share the same workspace for a given job.

# Contexts & expressions

Use ${{ }} to access contexts (e.g., ${{ github.ref }}, ${{ secrets.MY_SECRET }}) and to write conditional expressions in if:.

## Example of a simple CI workflow:
<img src ="../Images/Example workflow.png" alt="Link" width=250px>

## Powerful workflow features you’ll want to use
Matrix builds (parallel CI for many versions/platforms)
<img src ="../Images/matrix builds.png" alt="Link" width=250px>
Matrix runs speed up cross-platform/version testing by running multiple jobs in parallel. 


# Caching dependencies

Use actions/cache to save dependencies between runs (speeds up builds). You create a cache key usually based on lockfile checksum. Cache lookup falls back to restore-keys. 

# Artifacts

Use actions/upload-artifact and actions/download-artifact to pass build results (artifacts) between jobs or to keep logs/build outputs after a run finishes.

# Secrets & environment variables

Put sensitive values (tokens, passwords) in repo/org Secrets and reference them as ${{ secrets.MY_SECRET }}.

Use environment protection rules (environments, approvals) for jobs that deploy to production.

# Reusable workflows & composite actions

Reusable workflows let one workflow file be called from others using workflow_call. Great for centralizing CI steps across many repos. 

Composite actions let you bundle steps into a single action you can uses: inside a job (good for small shared step sets)
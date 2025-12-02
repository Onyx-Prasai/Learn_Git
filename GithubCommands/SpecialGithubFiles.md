# Special GitHub Files (Explained Simply)

These are files that GitHub treats differently because they control documentation, configuration, automation, or community rules of your repository.

## README.md

The first file people see in your repo.

Used to explain your project clearly.

Usually contains:

- What the project does

- How to install/use it

- Examples

- Badges

## LICENSE

Tells others what they can or cannot do with your code.

Examples: MIT, Apache 2.0, GPL.

Without a license, nobody legally has permission to use your code.

## .gitignore

Tells Git which files NOT to track.

Common things to ignore:

- node_modules

- .env

- compiled binaries

- temporary files

## CONTRIBUTING.md

Provides instructions for contributors:

- Coding style

- How to create issues

- How to submit PRs

- Branch naming rules

## CODE_OF_CONDUCT.md

Sets the rules for community behavior in your project.

Helps maintain a respectful environment.

## CHANGELOG.md

A list of updates or changes made in the project over time.

Makes it easier for users/developers to track versions.

## SECURITY.md

Tells users how to report security vulnerabilities safely.

Very important for open-source.

## FUNDING.yml

Used to show a Sponsor button.

Supports GitHub Sponsors, Patreon, Ko-fi, etc.

## issue templates & PR templates

Located in:

``` bash
.github/
   ISSUE_TEMPLATE/
   PULL_REQUEST_TEMPLATE.md
```

Predefined formats for issues and pull requests.

Helps maintain consistency.

## workflows (GitHub Actions)

Located in:

``` bash
.github/workflows/
```

YAML files used to automate:

- Tests

- Builds

- Deployment

- CI/CD processes

## .gitattributes

Controls how Git handles files, like:

- Line endings

- File diff behavior

- Large file handling

## .github folder

Contains many of the special files above.

Exists only for GitHub-specific configurations.

[<<Back to Previous Page](./Fork.md) 
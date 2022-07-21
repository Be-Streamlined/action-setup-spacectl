# :gear: `setup-spacectl`
> An action that can be used to setup the [Spacelift](https://spacelift.io) Spacectl CLI tool in a github action

## About
This action sets up the Spacelift CLI, [`spacectl`](https://github.com/spacelift-io/spacectl), on GitHub's hosted Actions runners.

This action can be run on `ubuntu-latest`, `windows-latest`, and `macos-latest` GitHub Actions runners, and will install and expose a specified version of the `spacectl` CLI on the runner environment.

## Usage

Setup the `spacectl` CLI:

```yaml
steps:
- uses: be-streamlined/action-setup-spacectl@v1
```

A specific version of the `spacectl` CLI can be installed:

```yaml
steps:
- uses: be-streamlined/action-setup-spacectl@v1
  with:
    version: '0.10.0'
```

## Inputs
The actions supports the following inputs:

- `version`: The version of `spacectl` to install, defaulting to `1.2.0`

## License
[MIT](LICENSE).
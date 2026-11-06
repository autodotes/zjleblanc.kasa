# Changelog

All notable changes to this collection will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

### Added

- pre-commit hooks for whitespace, YAML, secrets, shell, Python syntax, and ansible-lint.
- GitHub Actions publish workflow that tags the commit, stamps `galaxy.yml`, builds the collection, and publishes it to Ansible Galaxy.
- This changelog.

### Changed

- `galaxy.yml` version is the `0.0.0-semantic-version` placeholder substituted at publish time. A commit message containing `#major` or `#minor` bumps that component; otherwise the workflow increments the patch version.
- Collection links now point at the `autodotes/zjleblanc.kasa` GitHub repository.
- `meta/runtime.yml` requires Ansible `>=2.15.0`, and `galaxy.yml` includes the `tools` tag required by ansible-lint.
- Module examples use the sequence indentation ansible-lint expects, and trailing whitespace and missing final newlines were normalized.

## [1.1.0] and earlier

Releases prior to this file being introduced were tracked only via [GitHub tags](https://github.com/autodotes/zjleblanc.kasa/tags) and commit history.

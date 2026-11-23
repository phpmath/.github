# Contributing

Thank you for helping. A bug report, a question and a pull request are all welcome. Open an issue or a pull request in the repository of the library you are using.

## Before you open a pull request

Run the same checks as the CI of the library:

```bash
composer test
composer analyse
composer check-style
```

- The code follows [phpmath/coding-standard](https://github.com/phpmath/coding-standard). `composer fix-style` fixes most findings.
- Every change comes with tests. Coverage stays at 100%.
- Tests follow Arrange, Act and Assert, with one behavior and one Act per test, in `tests/unit/<Class>/<Method>Test.php`.
- Objects are immutable. Classes are `final` and `readonly`, or `abstract`.
- Update the documentation in `docs/` when behavior changes.
- Write commit messages in the imperative mood, with a subject line of about 50 characters.
- Use plain punctuation in code, documentation and commit messages. Do not use em dashes, the repositories check for them.

## Documentation

The documentation of each library is written in Markdown in `docs/` and published on https://phpmath.github.io. See [docs-builder](https://github.com/phpmath/docs-builder) for the format.

## Releases and the changelog

Every library keeps a `CHANGELOG.md` in the format of [Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/) and follows [semantic versioning](https://semver.org).

- A pull request that changes behavior adds a line under `## [Unreleased]`, in the group that fits: **Added**, **Changed**, **Deprecated**, **Removed**, **Fixed** or **Security**. Each line says what changed for the user, not what changed in the code.
- To release, move the lines of `[Unreleased]` under a new heading with the version and the date, for example `## [2.1.0] - 2027-02-01`, and update the links at the bottom of the file.
- A tag is just the version, for example `2.1.0` (no `v` prefix). The GitHub release of that tag has the same text as its changelog section.
- A breaking release links to the upgrading page of the documentation. That page explains how to move from the previous major version.
- Every library supports the PHP versions that are in active support on php.net when a major version is released, and keeps that minimum for the whole major version. A higher minimum PHP version is a new major version.
- Only the latest major version receives fixes, see the [security policy](SECURITY.md).
- The documentation of every tag is published automatically, so the version selector on https://phpmath.github.io lists every release.

## Security problems

Do not report them in a public issue. See the [security policy](SECURITY.md).

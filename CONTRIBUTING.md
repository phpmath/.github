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

## Security problems

Do not report them in a public issue. See the [security policy](SECURITY.md).

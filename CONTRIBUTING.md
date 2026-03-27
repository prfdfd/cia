# Contributing to Citizen Intelligence Agency

---

## Contributing

[fork]: /fork
[pr]: /compare
[code-of-conduct]: CODE_OF_CONDUCT.md

Hi there! We're thrilled that you'd like to contribute to this project. Your help is essential for keeping it great.

Please note that this project is released with a [Contributor Code of Conduct][code-of-conduct]. By participating in this project you agree to abide by its terms.

## Issues and PRs

If you have suggestions for how this project could be improved, or want to report a bug, open an issue! We'd love all and any contributions. If you have questions, too, we'd love to hear them.

We'd also love PRs. If you're thinking of a large PR, we advise opening up an issue first to talk about it, though! Look at the links below if you're not sure how to open a PR.

## Submitting a pull request

1. [Fork][fork] and clone the repository.
1. Configure and install the dependencies: `mvn clean install`.
1. Make sure the tests pass on your machine: `mvn test`.
1. Create a new branch: `git checkout -b my-branch-name`.
1. Make your change, add tests, and make sure the tests still pass.
1. Push to your fork and [submit a pull request][pr].
1. Pat yourself on the back and wait for your pull request to be reviewed and merged.

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Write and update tests.
- Keep your changes as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

Work in Progress pull requests are also welcome to get feedback early on, or if there is something blocked you.

### Test Naming Conventions

This project follows strict test naming conventions to separate unit tests from integration tests:

- **Unit Tests**: Use `*Test.java` suffix
  - Pure unit tests with mocked dependencies
  - No database access, no external API calls
  - Fast execution (< 1 second per test)
  - Example: `RiksdagenDateUtilTest`, `ApiDtoSanityTest`

- **Integration Tests**: Use `*ITest.java` suffix  
  - Tests that require database access
  - Tests that call external APIs
  - Tests that use Spring application context
  - Slower execution, require infrastructure
  - Example: `WorldbankTopicApiImplITest`, `DataDAOITest`

**Why this matters**: The build system excludes `**ITest*` from unit test runs to keep CI fast and avoid external dependencies. Always use the correct suffix based on whether your test has external dependencies.

## Security Guidelines

### Security Requirements for Contributors

- No hardcoded credentials or secrets in code
- Proper input validation and output encoding
- Use parameterized queries for database access
- Follow OWASP secure coding guidelines
- Report security vulnerabilities privately via [SECURITY.md](SECURITY.md)

### Automated Security Checks

All pull requests are automatically scanned:
- **CodeQL Analysis** - Static application security testing (SAST)
- **Dependency Review** - Software composition analysis (SCA)
- **Secret Scanning** - Credential leak detection
- **OSSF Scorecard** - Security best practices verification

### Reporting Security Vulnerabilities

**Do not open public issues for security vulnerabilities.** Follow our [Security Policy](SECURITY.md) to report vulnerabilities privately.

## Resources

- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)

---

## Related Documents

- [Unit Test Plan](./UnitTestPlan.md) - Unit testing requirements
- [E2E Test Plan](./E2ETestPlan.md) - End-to-end testing standards
- [CI/CD Workflows](./WORKFLOWS.md) - CI/CD pipelines
- [Code of Conduct](./CODE_OF_CONDUCT.md) - Community standards
- [Security Policy](./SECURITY.md) - Vulnerability reporting
- [README](./README.md) - Project overview


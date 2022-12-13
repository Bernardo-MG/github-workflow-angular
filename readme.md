# Github Workflow Files for Angular

Github workflow files for using CI in Angular projects.

## Features

- Tests
- Site deployment
- Deployment to Github
- Deployment to OSSRH

## Usage

Use these files as any reusable workflow:

```
jobs:
  tests:
    name: Tests with Node ${{ matrix.node }}
    strategy:
      matrix:
        node: [ 16.x ]
    uses: Bernardo-MG/github-workflow-angular/.github/workflows/testing.yml@v1
    with:
      node: ${{ matrix.node }}
```

## Collaborate

Any kind of help with the project will be well received, and there are two main ways to give such help:

- Reporting errors and asking for extensions through the issues management
- or forking the repository and extending the project

### Issues management

Issues are managed at the GitHub [project issues tracker][issues], where any Github user may report bugs or ask for new features.

### Getting the code

If you wish to fork or modify the code, visit the [GitHub project page][scm], where the latest versions are always kept. Check the 'master' branch for the latest release, and the 'develop' for the current, and stable, development version.

## License

The project has been released under version 2.0 of the [Apache License][license].

[archetype]: https://github.com/Bernardo-MG/library-angular-archetype
[issues]: https://github.com/Bernardo-MG/github-workflow-angular/issues
[license]: https://www.apache.org/licenses/LICENSE-2.0
[scm]: https://github.com/Bernardo-MG/github-workflow-angular

---
#layout: home
title: Casal2 Contributor Guidelines
permalink: /contributing/
---

# Casal2 Contributor Guidelines

## Start with the documents, create GitHub issue(s), then work in git branches

All work in the NIWA Casal2 GitHub repository will be coordinated by the Casal2 Development Team and tracked using GitHub issues. Supporting documents can be attached to these issues. The changes will be managed in branches and integrated in pull requests.

The required documents include:

- A technical description or software design document, including equations and references;
- A detailed test plan for validation and verification, including test case input and output files; and
- Any revisions to the Casal2 User Manual and/or other project documentation

Please provide documents in LaTeX format.

All contributions to the Casal2 project are made via Pull Requests against the *master* branch. Non-trivial developments must be discussed and agreed to **in advance** in a GitHub issue.

### Reporting bugs

Report bugs by opening an issue in the [GitHub repository](https://github.com/NIWAFisheriesModelling/Casal2/issues).

For source code bugs: provide a description of the bug(s), the filename(s) for the code that has the bug(s), and the initial steps that will be taken to fix the bug(s).

For executable bugs: provide the version of the software affected by the bug, the operating system type and version, the input files necessary to reproduce the bug, how the expected result differs from the actual result, whether the released version of the executable was used or if the executable was built from source (then provide the compiler and version, and information on the other build tools used), and any other relevant information.

### Requesting enhancements

Request enhancements by opening an issue in the GitHub repository. Provide, at minimum, a technical description document with equations that provides detailed conceptual information on the new feature/functionality, and the rationale for implementing it. Please also describe how implementing and using this enhancement would affect existing functionality, proposals for changes to the input data and/or output formats, example use cases, and other supporting information.

### Maintenance and feature development

Work with the Casal2 Development Team to create document(s) and GitHub issue(s) to fully describe the existing functionality and the changes required to achieve the planned maintenance or development work. The description should also include the scope of the changes and which sections of the repository will be updated.

Include details about the contracted milestones, objectives, and deliverables that this work is associated with.

### Order of activities

1. Work with the Casal2 Development Team to create a GitHub issue with detailed task information and narrow scope

2. Have the Casal2 Development Team create a branch to work on the issue in the format `<topic area>_YYYYMM`, e.g., `retention_unit_tests_201911`

3. Review the issue and add additional information about the work to be performed

4. Comment regularly in the issue as work progresses about what decisions were made and why, problems or questions that arise and proposed solutions, requests for clarification, etc.

5. Create a pull request after completing the changes and passing the unit and system tests locally

6. Work with the Casal2 Development Team to review the changes

7. The Casal2 Development Team will merge the changes after the code review

### git commit messages

The first part of each line of the commit message should indicate the type of modification:

- ADD - Added a new file
- UPD - Modified an existing file
- DEL - Removed an existing file
- FIX - Fixed something

NOTE: commits pertaining to a specific issue should include `Ref issue #[issue number]` in the commit message

## Code review

The Casal2 project uses the [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html) and the [Google R Style Guide](https://google.github.io/styleguide/Rguide.html), which is a fork of the [Tidyverse Style Guide](https://style.tidyverse.org/). Other Google Style Guides are available [here](https://google.github.io/styleguide/).

The code review will include:

- a review of the GitHub issue describing and discussing the bug or enhancement request and its requirements;
- a check that `doBuild release`, `doBuild release [optimizer]`, `doBuild rlibrary`, and `doBuild documentation` all complete successfully;
- a check that `doBuild test`, unit tests, `doBuild modelrunner`, and system tests complete successfully;
- a review of any changes to the Casal2 User Manual and/or other project documentation;
- a review of any new or revisions to existing unit tests and their supporting information (e.g., the R or Python 3 files used to produce the values in the unit test(s), which should also be committed to the git repository); also discuss test coverage and whether additional unit tests should be added;
- a review of the doxygen comments in the C++ or roxygen comments in the R source code;
- a review of the source code (C++, R, Python, etc.); and
- a review of the commit message(s)

Code reviews will be coordinated with the Casal2 Development Team.

After the pull request has been applied, the Casal2 Development Team will check that the CI/CD jobs completed successfully.

Note: as well as using the above style guides, development with the C++ source code in the Casal2 repository should also have these style characteristics:

- use two-space indentation (with spaces, not tabs);
- use spaces on both sides of equal signs;
- use a space after a comma;
- include comments within functions and classes; and
- include doxygen information for each function


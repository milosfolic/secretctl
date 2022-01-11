- [SecretCTL](#secretctl)
  - [About the project](#about-the-project)
    - [Design](#design)
    - [Status](#status)
  - [Getting started](#getting-started)
    - [Layout](#layout)
  - [Notes](#notes)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# SecretCTL

## About the project

This project is used to get familiar with GoLang cli apps, along with cobra generator.

### Status

This project is in alpha status.

## Getting started

Below we describe the conventions or tools specific to golang project.

### Layout

```tree
├── .gitignore
├── CHANGELOG.md
├── Makefile
├── README.md
├── bin
├── cmd
├── test
│   ├── README.md
│   └── test_make.sh
```

A brief description of the layout:

* `.gitignore` varies per project, but all projects need to ignore `bin` directory.
* `Makefile` is used to build the project.
* `CHANGELOG.md` contains auto-generated changelog information.
* `README.md` is a detailed description of the project.
* `bin` is to hold build outputs.
* `cmd` contains main packages.
* `build` contains scripts, yaml files, dockerfiles, etc, to build and package the project.
* `test` holds all tests (except unit tests), e.g. integration, e2e tests.

## Notes

* Makefile **MUST NOT** change well-defined command semantics, see Makefile for details.
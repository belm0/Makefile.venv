# Changelog for Makefile.venv

<!--Template for new entries


## CURRENT

*
*

[Source code tree](https://github.com/sio/Makefile.venv/tree/CURRENT)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/CURRENT)
| [Commit history](https://github.com/sio/Makefile.venv/compare/PREVIOUS...CURRENT)
-->


## v2022.07.20

* Support another edge case: "make -R" (running without builtin variables)
* Minor documentation improvements

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2022.07.20)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2022.07.20)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2022.04.13...v2022.07.20)


## v2022.04.13

* Makefile.venv is now installable from [PyPI](https://pypi.org/project/Makefile.venv/)
* No changes to Makefile.venv itself

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2022.04.13)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2022.04.13)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2021.12.16...v2022.04.13)


## v2021.12.16

* Added support for `py` entrypoint on Windows (thanks to [@gschwaer], issue [#15])
* Improved cross-platform support: now Windows without a POSIX shell should
  work too (wrappers for `cmd.exe` missing capabilities were added)
* Minor improvements to debug messages and test suite common tools

[@gschwaer]: https://github.com/gschwaer
[#15]: https://github.com/sio/Makefile.venv/issues/15

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2021.12.16)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2021.12.16)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2021.12.01...v2021.12.16)


## v2021.12.01

* Move setup․py path to variable (SETUP_PY): now multiple paths are supported
  and setup․py processing may be skipped by providing empty value (issue [#14])
* Improve documentation and extend test suite

[#14]: https://github.com/sio/Makefile.venv/issues/14

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2021.12.01)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2021.12.01)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2020.08.14...v2021.12.01)


## v2020.08.14

* Install 'wheel' package automatically when creating virtual environment

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2020.08.14)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2020.08.14)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2020.08.04...v2020.08.14)


## v2020.08.04

* Allow REQUIREMENTS_TXT to be generated with a Makefile recipe
* Improve documentation

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2020.08.04)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2020.08.04)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2020.05.07...v2020.08.04)


## v2020.05.07

* Add `debug-venv` target for troubleshooting

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2020.05.07)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2020.05.07)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2020.05.05...v2020.05.07)


## v2020.05.05

* Mark paths with spaces as unsupported
* Do not convert WORKDIR into absolute path
* Sanitize path when removing VENVDIR - avoid destructive consequences of
  paths with spaces

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2020.05.05)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2020.05.05)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2020.02.26...v2020.05.05)


## v2020.02.26

* Update setuptools when creating venv
* Trigger venv update on setup.cfg changes

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2020.02.26)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2020.02.26)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.12.05...v2020.02.26)


## v2019.12.05

* Use Python to detect if Windows paths are required. This helps to avoid
  mistakes when using different combinations of Cygwin/native Windows
  environments. Thanks to [@jpc4242](https://github.com/jpc4242)

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.12.05)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.12.05)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.12.04...v2019.12.05)


## v2019.12.04

* New configuration variable: FORCE_UNIX_PATHS. If this variable is set,
  unix-like file paths are assumed and no Windows detection takes place.
  Thanks to [@jpc4242](https://github.com/jpc4242) for reporting
  [the issue](https://github.com/sio/Makefile.venv/issues/2) with Cygwin.

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.12.04)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.12.04)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.11.22...v2019.12.04)


## v2019.11.22

* Upgrade pip only at initial environment creation. This helps to avoid build
  failures with old Python versions where pip can not be upgraded to newer
  releases. [Example](https://circleci.com/gh/sio/bash-complete-partial-path/53)

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.11.22)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.11.22)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.11.08...v2019.11.22)


## v2019.11.08

* Support multiple requirements.txt files via REQUIREMENTS_TXT environment
  variable

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.11.08)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.11.08)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.11.07...v2019.11.08)


## v2019.11.07

* Virtual environment creation happens only once. Dependencies change does not
  trigger a redundant call to `-m venv` if environment already exists.

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.11.07)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.11.07)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.11.06...v2019.11.07)


## v2019.11.06

* New pattern rule for rarely used dependencies (CLI tools in virtual
  environment)
* Improved code readability and documentation

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.11.06)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.11.06)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.10.04...v2019.11.06)


## v2019.10.04

* Automated testing for new releases with GitHub CI
* Deduplicated code for interactive shell targets

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.10.04)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.10.04)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.10.03...v2019.10.04)


## v2019.10.03

* Cleaner process tree thanks to launching interactive shells via `exec`

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.10.03)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.10.03)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.10.01...v2019.10.03)


## v2019.10.01

* New targets for interactive shells in virtual environment:
  `make bash`, `make zsh`
* Promotional post in author's blog: [https://potyarkin.ml/...][blog]

[blog]: https://potyarkin.ml/posts/2019/manage-python-virtual-environment-from-your-makefile/

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.10.01)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.10.01)
| [Commit history](https://github.com/sio/Makefile.venv/compare/v2019.09.30...v2019.10.01)


## v2019.09.30

* First reusable version of Makefile.venv. All essential features are available.

[Source code tree](https://github.com/sio/Makefile.venv/tree/v2019.09.30)
| [Tarball](https://github.com/sio/Makefile.venv/tarball/v2019.09.30)
| [Commit history](https://github.com/sio/Makefile.venv/compare/9c9b6d5aae8955d207d5c9d45b754c01c20be650...v2019.09.30)

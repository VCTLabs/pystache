v0.6.2  (2022-09-14)
--------------------

New
~~~
- Add full sphinx apidoc build, include readme/extras. [Stephen L
  Arnold]

  * add new tox commands for 'docs' and 'docs-lint'
  * cleanup link errors found by docs-lint
  * add sphinx doc build workflow, update ci workflow
  * remove new version var from __init__.py globals

Changes
~~~~~~~
- Convert readme.md to readme.rst, move extra docs. [Stephen L Arnold]

Fixes
~~~~~
- Fix included filename and link cleanup. [Stephen L Arnold]
- Remove more py2 cruft from doctesting (py3.10 warnings) [Stephen L Arnold]
- Update maintainer info and spec test cmd. [Stephen L Arnold]

  * update coverage value for delta/base, allow digits only
- Use updated bandit action and workflow excludes (exclude test)
  [Stephen L Arnold]

  * also fix missing PR event check in coverage workflow
- Use current org-level coverage workflow. [Stephen L Arnold]

  * increase fetch depth and update regex
  * updated action deps, relaxed run criteria
  * go back to "normal" tokens, remove permission hacks
  * still needs more job isolation => refactor for another day

Other
~~~~~
- Use buildbot account. [Katelyn Gigante]
- Use ACCESS_TOKEN secret rather than provided GITHUB_TOKEN. [Katelyn
  Gigante]

  Should fix the coverage badge


v0.6.1 (2021-11-24)
-------------------

Changes
~~~~~~~
- Add shallow checkout for testing. [Stephen L Arnold]
- Bump comment action to latest release, verify checkout depth. [Stephen
  L Arnold]

  * see: https://github.com/marocchino/sticky-pull-request-comment/issues/298
    in upstream action repo

Fixes
~~~~~
- Use workflow PR target and checkout params. [Stephen L Arnold]
- Split coverage (checkout) job from PR comment job. [Stephen L Arnold]
- Use correct tox env cmd for single platform/version. [Stephen L
  Arnold]

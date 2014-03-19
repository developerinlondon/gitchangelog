Changelog
=========

2.0.0.1dev_r201309212000 (unreleased)
------------------------

Fix
~~~

- Gitchangelog shouldn't fail if it fails to parse your git config.
  [Michael Hahn]

2.0.0 (2013-08-20)
------------------

New
~~~

- Added a ``mako`` output engine with standard ReSTructured text format
  for reference. [Valentin Lab]

- Added some information on path lookup scheme to find
  ``gitchangelog.rc`` configuration file. [Valentin Lab]

- Added templating system and examples with ``mustache`` template
  support for restructured text and markdown output format. [David
  Loureiro]

Changes
~~~~~~~

- Removed ``pkg`` and ``dev`` commits from default sample changelog
  output. [Valentin Lab]

Fix
~~~

- Some error message weren't written on stderr. [Valentin Lab]

1.1.0 (2012-05-03)
------------------

New
~~~

- New config file lookup scheme which adds a new possible default
  location ``.gitchangelog.rc`` in the root of the git repository.
  [Valentin Lab]

- Added a new section to get a direct visual of ``gitchangelog`` output.
  Reworded some sentences and did some other minor additions. [Valentin
  Lab]

Changes
~~~~~~~

- Removed old ``gitchangelog.rc.sample`` in favor of the new documented
  one. [Valentin Lab]

Fix
~~~

- The sample file was not coherent with the doc, and is now accepting
  'test' and 'doc' audience. [Valentin Lab]

1.0.2 (2012-05-02)
------------------

New
~~~

- Added a new sample file heavily documented. [Valentin Lab]

Fix
~~~

- ``ignore_regexps`` where bogus and would match only from the beginning
  of the line. [Valentin Lab]

- Display author date rather than commit date. [Valentin Lab]

0.1.2 (2011-05-17)
------------------

New
~~~

- Added ``body_split_regexp`` option to attempts to format correctly
  body of commit. [Valentin Lab]

- Use a list of tuple instead of a dict for ``section_regexps`` to be
  able to manage order between section on find match. [Valentin Lab]

Fix
~~~

- ``git`` in later versions seems to fail on ``git config <key>`` with
  errlvl 255, that was not supported. [Valentin Lab]

- Removed Traceback when there were no tags at all in the current git
  repository. [Valentin Lab]

0.1.1 (2011-04-07)
------------------

New
~~~

- Added section classifiers (ie: New, Change, Bugs) and updated the
  sample rc file. [Valentin Lab]

- Added a succint ``--help`` support. [Valentin Lab]



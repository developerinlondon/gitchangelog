# Changelog

## %%version%% (unreleased)

### Fix

* gitchangelog shouldn't fail if it fails to parse your git config. [Michael Hahn]


## 2.0.0 (2013-08-20)

### New

* added a ``mako`` output engine with standard ReSTructured text format for reference. [Valentin Lab]

* added some information on path lookup scheme to find ``gitchangelog.rc`` configuration file. [Valentin Lab]

* added templating system and examples with ``mustache`` template support for restructured text and markdown output format. [David Loureiro]

### Changes

* removed ``pkg`` and ``dev`` commits from default sample changelog output. [Valentin Lab]

### Fix

* some error message weren't written on stderr. [Valentin Lab]


## 1.1.0 (2012-05-03)

### New

* new config file lookup scheme which adds a new possible default location ``.gitchangelog.rc`` in the root of the git repository. [Valentin Lab]

* added a new section to get a direct visual of ``gitchangelog`` output. Reworded some sentences and did some other minor additions. [Valentin Lab]

### Changes

* removed old ``gitchangelog.rc.sample`` in favor of the new documented one. [Valentin Lab]

### Fix

* the sample file was not coherent with the doc, and is now accepting 'test' and 'doc' audience. [Valentin Lab]


## 1.0.2 (2012-05-02)

### New

* added a new sample file heavily documented. [Valentin Lab]

### Fix

* ``ignore_regexps`` where bogus and would match only from the beginning of the line. [Valentin Lab]

* display author date rather than commit date. [Valentin Lab]


## 1.0.1 (2011-06-29)


## 1.0.0 (2011-06-29)


## 0.1.4 (2011-05-27)


## 0.1.3 (2011-05-23)


## 0.1.2 (2011-05-17)

### New

* added ``body_split_regexp`` option to attempts to format correctly body of commit. [Valentin Lab]

* use a list of tuple instead of a dict for ``section_regexps`` to be able to manage order between section on find match. [Valentin Lab]

### Fix

* ``git`` in later versions seems to fail on ``git config &lt;key&gt;`` with errlvl 255, that was not supported. [Valentin Lab]

* removed Traceback when there were no tags at all in the current git repository. [Valentin Lab]


## 0.1.1 (2011-04-07)

### New

* added section classifiers (ie: New, Change, Bugs) and updated the sample rc file. [Valentin Lab]

* added a succint ``--help`` support. [Valentin Lab]



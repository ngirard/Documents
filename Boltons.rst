.. —— Source: https://github.com/mahmoud/boltons/blob/master/docs/index.rst

.. boltons documentation master file, created on Sat Mar 21 00:34:18 2015.
boltons
=======

*boltons should be builtins.*

|release| |calver| |changelog|

**Boltons** is a set of pure-Python utilities in the same spirit as —
and yet conspicuously missing from — `the standard library`_,
including:

  * :func:`Atomic file saving <boltons.fileutils.atomic_save>`, bolted on with
    :mod:`~boltons.fileutils`
  * A highly-optimized :class:`~boltons.dictutils.OrderedMultiDict`,
    in :mod:`~boltons.dictutils`
  * Two types of :class:`~boltons.queueutils.PriorityQueue`, in
    :mod:`~boltons.queueutils`
  * :func:`Chunked <boltons.iterutils.chunked>` and
    :func:`windowed <boltons.iterutils.windowed>` iteration, in
    :mod:`~boltons.iterutils`
  * A full-featured :class:`~boltons.tbutils.TracebackInfo` type, for
    representing stack traces, in :mod:`~boltons.tbutils`
  * A lightweight :class:`UTC timezone <boltons.timeutils.UTC>`
    available in :mod:`~boltons.timeutils`.
  * Recursive mapping for nested data transforms, with :func:`remap
    <boltons.iterutils.remap>`

And that's just a small selection. As of |today|, ``boltons`` is
|b_type_count| types and |b_func_count| functions, spread across
|b_mod_count| modules. See them all in the :ref:`genindex`, and see
what's new by `checking the CHANGELOG`_.

.. counts are appx 50, 75, and 23, respectively, as of initial docs writing
.. in mid 2016, the counts are now 62, 112, and 25, respectively

.. _the standard library: https://docs.python.org/2.7/library/index.html
.. _checking the CHANGELOG: https://github.com/mahmoud/boltons/blob/master/CHANGELOG.md



.. ——— Source: https://github.com/mahmoud/boltons/blob/master/docs/architecture.rst

Architecture
============

``boltons`` has a minimalist architecture: remain as consistent, and
self-contained as possible, with an eye toward maintaining its range
of use cases and usage patterns as wide as possible.

.. _arch_integration:

Integration
-----------

Utility libraries are often used extensively within a project, and
because they are not often fundamental to the architecture of the
application, simplicity and stability may take precedence over version
recency. In these cases, developers can:

  1. Copy the whole ``boltons`` package into a project.
  2. Copy just the ``utils.py`` file that a project requires.

Boltons take this into account by design.  The ``boltons`` package
depends on no packages, making it easy for inclusion into a
project. Furthermore, virtually all individual modules have been
written to be as self-contained as possible, allowing cherrypicking of
functionality into projects.

Design of a ``bolton``
----------------------

``boltons`` aims to be a living library, an ever-expanding collection
of tested and true utilities. For a bolton to be a bolton, it
should:

  1. Be pure-Python and as self-contained as possible.
  2. Perform a common task or fulfill a common role.
  3. Demonstrate and mitigate some insufficiency in the standard library.
  4. Strive for the standard set forth by the standard library by
     striking a balance between best practice and "good enough",
     correctness and common sense. When in doubt, ask, "what would the
     standard library do?"
  5. Have approachable documentation with at least one helpful
     :mod:`doctest`, links to relevant standard library functionality, as
     well as any 3rd-party packages that provide further capabilities.

Finally, boltons should be substantial implementations of commonly
trivialized stumbling blocks and not the other way around. The larger
the problem solved, the less likely the functionality is suitable for
inclusion in boltons; boltons are fundamental and self-contained, not
sweeping and architecture-defining.

Themes of ``boltons``
---------------------

``boltons`` has had a wide variety of inspirations over the years, but
a definite set of themes have emerged:

1. From the Python docs:

   1. :mod:`~boltons.queueutils` - `heapq docs`_
   2. :mod:`~boltons.iterutils` - `itertools docs`_
   3. :mod:`~boltons.timeutils` - `datetime docs`_

2. Reimplementations and tweaks of the standard library:

   1. :func:`boltons.fileutils.copytree` - :func:`shutil.copytree`
   2. :class:`boltons.namedutils.namedtuple` - :func:`collections.namedtuple`

3. One-off implementations discovered in multiple other libraries' ``utils.py`` or equivalent

   1. :func:`boltons.strutils.slugify`
   2. :func:`boltons.strutils.bytes2human`
   3. :func:`boltons.timeutils.relative_time`

4. More powerful multi-purpose data structures

   1. :class:`boltons.dictutils.OrderedMultiDict`
   2. :class:`boltons.setutils.IndexedSet`
   3. :class:`boltons.listutils.BList`
   4. :class:`boltons.namedutils.namedlist`
   5. :class:`boltons.tableutils.Table`

5. Personal practice and experience

   1. :mod:`boltons.debugutils`
   2. :mod:`boltons.gcutils`
   3. :mod:`boltons.tbutils`


.. _heapq docs: https://docs.python.org/2/library/heapq.html#priority-queue-implementation-notes
.. _itertools docs: https://docs.python.org/2/library/itertools.html#recipes
.. _datetime docs: https://docs.python.org/2/library/datetime.html#tzinfo-objects

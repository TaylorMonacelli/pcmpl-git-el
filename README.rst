==========================
 Git Completion for Emacs
==========================
 
Provide completion support for ``git`` in Emacs in places pcomplete is
used (mainly shell/eshell).

install
-------

Place file ``pcmpl-git.el`` in ``load-path`` and ``git-options`` in
``data-directory`` by default. You can put file ``git-options``
anywhere and customise ``pcmpl-git-options-file`` to point to it.

File ``pcmpl-git-parse.el`` is not needed for running this package. It
is used for generating ``git-options``.

usage
-----

Complete both git commands and their options and arguments. Type '-'
to complete short options and '--' to complete long options. For
commands that accept commit as argument, branches and tags will be
tried first and then the SHAs in the first few hundred commits.

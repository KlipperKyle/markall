markall
=======

A simple script to convert all markdown files in a directory to HTML

Synopsis
----------

    bash markall

Description
-------------

`markall` converts all Markdown files in a directory into HTML. All
files ending in `*.md` are piped through markdown and copied to a file
of the same name with a `.html` extension.

`markall` creates a file named `index.html`. This file is a listing of
the Markdown files in the current directory, each linked to the
corresponding HTML document.

`markall` currently does not recurse into subdirectories.

`markall` will display the list of files converted. If an HTML version
of a Markdown file exists, the HTML version is updated if the timestamp
of the Markdown file is more recent than the timestamp of the HTML
version.

Options
---------

- `-h` `--help` -- Display a brief message describing how to use
  `markall`

Exit Status
-------------

- 0 -- Success
- 1 -- Error (Make sure markdown is installed)
- 2 -- Displaying help

Errors
--------

- "Cannot find markdown" -- Make sure markdown is installed, is named
  `markdown`, and is located in the $PATH environment variable.

<!-- vim: spell ft=markdown tw=72 sw=4 ts=4 et :
-->

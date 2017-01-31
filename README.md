# The `union` command for Unix text processing

Print the lines that are in any of the inputs.

Syntax:

    union <input> ...


## Examples

Example with two files:

    $ union a.txt b.txt
    => lines that are in either of the files.

Example with three files:

    $ union a.txt b.txt c.txt
     => lines that are in any of the files.


## Specifics

The order does not matter.


## Related commands

These commands are related:

  * `union`: print lines in (A union B)
  * `intersect`: print lines in (A intersect B)
  * `except`: print lines in (A except B) a.k.a. (A - B)
  * `extra` : print lines in (A extra B) a.k.a. (B - A)


## Notes

In set theory, this command is (A union B).

This command aims to be fast, not to sort.

This command is currently implemented using `awk` and POSIX.


## Tracking

* Program: union
* Version: 2.0.2
* Created: 2017-01-30
* Updated: 2017-01-30
* License: GPL
* Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)

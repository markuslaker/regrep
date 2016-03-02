# regrep
A fast grep clone written in Perl 5, offering the power of Perl 5 regular expressions

This program was an attempt to answer the question: how fast could a grep implementation possibly be if it were written in Perl?  As such, it sacrifices all readability in the name of speed.  Don't use it to argue that Perl is always unreadable; that would be a cheap shot.  Instead, marvel at how fast Perl can be.

Regrep was also a way to circumvent the limitations of the regular expressions offered by `grep`(1).  If you're a regex guru, you're going to love regrep.

Most of the options work in the same way as Gnu `grep`.  To see which options are supported, including several that Gnu `grep` doesn't provide, run `regrep` with no command-line arguments.

Regrep was originally written as a reusable module, ReGrep.pm, and a command-line front end.  If you're a Perl author and you want to reuse the regrep engine, just pull packages `ReGrep::Options` and `ReGrep` into a separate file called ReGrep.pm and use it freely.  There's some documentation in the source file explaining how to use it.

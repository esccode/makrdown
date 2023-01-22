## NAME
gawk - pattern scanning and processing language
## SYNOPSIS
gawk [ POSIX or GNU style options ] `-f` program-file [ -- ]..
gawk [ POSIX or GNU style options ] [ .. ] program-text file ...

## DESCRIPTION
Gawk is the GNU Project's implementation of the AWK programming language. It conform to the definition of the language in the POSIX 1003.1 standard. This version in turn is based on the description in <u>The AWK Programming Language</u>, by Aho, Kerninghan, and Weinberger. GAwk provides the additional features found in the current version of Brain Kerninghan's <u>awk</u> and numerous GNU-specific extensions.

The command line consists of options to gawk itself, the AWK program text (if not supplied  via the -f or `--incude` options), and values to be made available in the ARGC and ARGV pre-defined AWK variables.

When <u>gawk</u> is invoked with the `--profile` option, it starts gathering profiling statistics from the execution of the program. <u>Gawk</u> runs more slowly in this mode, and automatically produces an execution profile in the file awkprof.aut when done. See the `--profile` options. The debugger is documented in <u>GAWK</u>

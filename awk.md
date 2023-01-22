---
title: "awk"
author: Jacek Wieteska
description: 'copy from man Ubuntu 20.04.5 LTS'
date: January 22, 2023
output: markdown
---

## NAME
gawk - pattern scanning and processing language

## SYNOPSIS
gawk [ POSIX or GNU style options ] `-f` program-file [ -- ]..
gawk [ POSIX or GNU style options ] [ .. ] program-text file ...

## DESCRIPTION
Gawk is the GNU Project's implementation of the AWK programming language. It conform to the definition of the language in the POSIX 1003.1 standard. This version in turn is based on the description in <u>The AWK Programming Language</u>, by Aho, Kerninghan, and Weinberger. GAwk provides the additional features found in the current version of Brain Kerninghan's <u>awk</u> and numerous GNU-specific extensions.

The command line consists of options to gawk itself, the AWK program text (if not supplied  via the -f or `--incude` options), and values to be made available in the ARGC and ARGV pre-defined AWK variables.

When <u>gawk</u> is invoked with the `--profile` option, it starts gathering profiling statistics from the execution of the program. <u>Gawk</u> runs more slowly in this mode, and automatically produces an execution profile in the file awkprof.out when done. See the `--profile` options, below.

<u>Gawk</u> also has an integrated debugger. An interactive debugging session can be started by supplying the `--debug` option to the command line. In this mode of execution, <u>gawk</u> loads the AWK source code and then prompts for debugging commands. <u>Gawk</u> can only debug AWK program source provided with the `-f` and `--include` options. The debugger is documented in <u>GAWK</u>: <u>Effective AWK Programming</u>.

## OPTION FORMAT
<u>Gawk</u> options may be either traditional POSIX-style one letter options, or GNU-style long option, or GNU-style long option. POSIX options start with a single `"-"`, while long options start with `"--"`. Long options are provided for both GNU-specific features and for POSIX-mandated features.

<u>Gawk</u>-specific options are typically used in long-options form. Arguments to long options are either joined with the options by an = sign, with no intervening space, or they may be provided in the next command line argument. Long options may be abbreviated, as long as abbreviation remains unique.

Additionally, every long options has a corresponding short options, so that the option's functionality may be used from within `#!` executable csripts.

## OPTIONS
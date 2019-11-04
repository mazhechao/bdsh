# For Your Information
This is a magical Bash which can logging all commands and detect reverse shell, developed based on GNU Bash 4.4.
To build, just run:

```
./configure
make
```

## Logging bash commands to syslog
bdsh uses facility `local6` as default. For example, to restore logs into a file,

```
local6.*  /var/log/bash.log
```

# Introduction

This is GNU Bash, version 4.4.  Bash is the GNU Project's Bourne
Again SHell, a complete implementation of the POSIX shell spec,
but also with interactive command line editing, job control on
architectures that support it, csh-like features such as history
substitution and brace expansion, and a slew of other features. 
For more information on the features of Bash that are new to this
type of shell, see the file `doc/bashref.texi'.  There is also a
large Unix-style man page.  The man page is the definitive description
of the shell's features. 

See the file POSIX for a discussion of how the Bash defaults differ
from the POSIX spec and a description of the Bash `posix mode'.

There are some user-visible incompatibilities between this version
of Bash and previous widely-distributed versions, bash-4.2 and
bash-4.3.  For details, see the file COMPAT.  The NEWS file tersely
lists features that are new in this release. 

Bash is free software, distributed under the terms of the [GNU] General
Public License as published by the Free Software Foundation,
version 3 of the License (or any later version).  For more information,
see the file COPYING. 

A number of frequently-asked questions are answered in the file
`doc/FAQ'.

To compile Bash, type `./configure', then `make'.  Bash auto-configures
the build process, so no further intervention should be necessary.  Bash
builds with `gcc' by default if it is available.  If you want to use `cc'
instead, type

	CC=cc ./configure

if you are using a Bourne-style shell.  If you are not, the following
may work:

	env CC=cc ./configure

Read the file INSTALL in this directory for more information about how
to customize and control the build process.  The file NOTES contains
platform-specific installation and configuration information.

If you are a csh user and wish to convert your csh aliases to Bash
aliases, you may wish to use the script `examples/misc/alias-conv.sh'
as a starting point.  The script `examples/misc/cshtobash' is a
more ambitious script that attempts to do a more complete job.

# Reporting Bugs

Bug reports for bash should be sent to:

	bug-bash@gnu.org

using the `bashbug' program that is built and installed at the same
time as bash.

The discussion list `bug-bash@gnu.org' often contains information
about new ports of Bash, or discussions of new features or behavior
changes that people would like.  This mailing list is also available
as a usenet newsgroup: gnu.bash.bug. 

When you send a bug report, please use the `bashbug' program that is
built at the same time as bash.  If bash fails to build, try building
bashbug directly with `make bashbug'.  If you cannot build `bashbug',
please send mail to bug-bash@gnu.org with the following information:

	* the version number and release status of Bash (e.g., 2.05a-release)
	* the machine and OS that it is running on (you may run
	  `bashversion -l' from the bash build directory for this information)
	* a list of the compilation flags or the contents of `config.h', if
	  appropriate
	* a description of the bug
	* a recipe for recreating the bug reliably
	* a fix for the bug if you have one!

The `bashbug' program includes much of this automatically.

Questions and requests for help with bash and bash programming may be
sent to the help-bash@gnu.org mailing list.

If you would like to contact the Bash maintainers directly, send mail
to bash-maintainers@gnu.org.

While the Bash maintainers do not promise to fix all bugs, we would
like this shell to be the best that we can make it.

Enjoy!

Chet Ramey
chet.ramey@case.edu

Copying and distribution of this file, with or without modification,
are permitted in any medium without royalty provided the copyright
notice and this notice are preserved.  This file is offered as-is,
without any warranty.

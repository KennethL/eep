Erlang Enhancement Process
--------------------------

This repository contains EEPs (Erlang Extension Proposals) in the subdirectory `eeps/`.


## What is the EEP?

There are always many discussion threads on the mailing list erlang-questions
and other places about enhancements,
changes and extensions to the Erlang runtime system, the standard libraries
and the language.

To document the various proposals and the decisions taken we use the Erlang Enhancement Process inspired by the Python Enhancement Process.

Because Erlang is a programming language with millions of lines of
running business critical code in the world, the development process must
impose some rigidity and provide resistance against accepting premature changes.

Users have Erlang code, linked in drivers written in C, and applications that
embed Erlang, so it is important that the inconvenience of upgrading to
new versions of Erlang is minimized. Language changes might also make the
language more difficult for new users to learn.

To ensure that changes are carefully considered, significant changes must be
described in an EEP, short for Erlang Extension Proposal.

Each EEP should explain, among other things, why the change is needed,
document how it should work, and give an overview how it should be implemented.
The EEP author should listen to the community's feeback and edit the EEP as
necessary.

Before submitting an EEP; read EEP 1 - EEP Purpose and Guidelines that
thoroughly explains the purpose of EEPs, their life cycle,
and prescribed format.

The EEP editor will reject EEPs that do not follow the guidelines.
Also check the list of existing EEPs before reinventing something.

## EEP Editorial

There is a mailing list for EEPs: eeps (at) erlang (dot) org, see Mailing Lists. Anyone interested can subscribe to the list.
The EEP editor(s) are subscribed to the list, as well as the EEP repository owner.
New EEPs should be sent here, as well as EEP updates. Note that as with all erlang.org mailing lists only subscribers are allowed to post to the list.

## Erlang Extension Proposal repository

The EEP source texts are in a Github GIT version control repository.
Anyone with a Github account can fork the repository,
add or change any EEP, inform the eeps mailing list about the new version,
and the origin repository owner will (if approving) pull the commit.

## Creating an EEP

The EEPs are in [Markdown][MD] (`*.md`) format according to this [EEP-template][Template].

The [EEP Index][EEP 0] in [EEP 0][] gathers all EEPs and is built with
the tools in the following paragraphs from the EEPs themselves.

This repository also contains a version of a [Markdown.pl][] script in
subdirectory `md/` that can be used, for example with the also contained
Perl [build script][build.pl] and some helper scripts,
to produce HTML versions of the `*.md` EEPs.

Type `perl build.pl` or `./build.pl` depending on your environment to
rebuild all HTML that needs to be rebuilt. A reasonable `perl` (5.8)
is all that is needed.

Patch suggestions to this repository should be sent to <eeps@erlang.org>
(remember to subscribe to the list first) as stated in the
[Erlang Enhancement Process][EEP].



[MD]: http://daringfireball.net/projects/markdown/
    "The Markdown Project"

[Markdown.pl]: md/Markdown.pl
    "Markdown.pl"

[EEP]: http://www.erlang.org/eep.html
    "Erlang Enhancement Process"

[build.pl]: build.pl
    "Perl build script to overcome Makefile inportability"

[EEP 0]: http://erlang.org/eep/eeps/eep-0000.html
    "EEP 0: Index of EEPS"

[Template]: eeps/eep-0033.md
    "EEP template"


Copyright
---------

This document has been placed in the public domain.

### Author
Erlang/OTP, Raimo Niskanen, 2010, 2018



[EmacsVar]: <> "Local Variables:"
[EmacsVar]: <> "mode: indented-text"
[EmacsVar]: <> "indent-tabs-mode: nil"
[EmacsVar]: <> "sentence-end-double-space: t"
[EmacsVar]: <> "fill-column: 70"
[EmacsVar]: <> "coding: utf-8"
[EmacsVar]: <> "End:"

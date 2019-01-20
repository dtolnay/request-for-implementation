Crates that don't exist, but should
===================================

A collection of [Rust] project ideas.
[*Skip the introduction and jump to the list*](#the-list)

These are bite-sized ideas for which someone already has a mostly clear design
in mind. They are waiting on an interested library developer to carry through
the implementation and own the code. The requester should be prepared to offer
guidance on any API design questions that arise during implementation.

Ideas should result in their own useful library, even if that is just a few
functions. Ideas for which the code would go in some existing project should be
filed on that project's issue tracker rather than being listed here.

Many of these would make neat projects for a Rust novice.

[Rust]: https://www.rust-lang.org/

<br>

### Contributing

To work on an idea, click through on one of the "Design" links to read more
about the idea and coordinate as you make progress on the library.

To add a project idea, please file an issue with enough detail so that anyone
interested can understand the design you have in mind. Include links to relevant
background material if possible. Then send a PR adding a link to your issue.
Feel free to add a new heading if none of the existing ones apply to your idea.

<br>

### Relationship to Not-Yet-Awesome Rust

The [not-yet-awesome] list is similarly a catalog of project ideas, but appears
to be geared toward relatively broad problem spaces that are not well addressed
by the Rust library ecosystem. Some examples from their list:

- A stream processing pipeline with back pressure for asynchronous processing;
- A deep learning toolkit with GPU support;
- A mature framework for Windows native UI.

These are things that will involve a significant amount of design work, feedback
from multiple stakeholders, a responsive and dedicated maintainer or team, and
likely months to years of bake time before they would be considered awesome.

In contrast, the Request For Implementation list is intended for ideas where a
design mostly already exists and can be concisely described. It should be clear
when a library has accomplished that design.

[not-yet-awesome]: https://github.com/not-yet-awesome-rust/not-yet-awesome-rust

<br><br>

<a name="the-list"></a>

<!--
TEMPLATE:

<table><tr><td><ul><li></li></ul></td><td>
description description description description description description
<br>
<a href="...">[Origin]</a>
—
<a href="...">[Design]</a>
</td></tr></table>

-->

<a name="command-line"></a>
# [:tractor: Command line](#command-line)

<table><tr><td><ul><li></li></ul></td><td>
Library for a Cargo subcommand to find components installed under a different
toolchain
<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/5">[Design]</a>
</td></tr></table>

<br>

<a name="de-serialization"></a>
# [:bullettrain_side: De/serialization](#de-serialization)

<table><tr><td><ul><li></li></ul></td><td>
A <code>dtd</code> macro that you could point at an
<a href="https://en.wikipedia.org/wiki/Document_type_definition">XML DTD file</a>
and have it generate struct definitions for you
<br>
<a href="https://twitter.com/chriskrycho/status/1085537088647249920">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/2">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Derive macros to serialize and deserialize struct as an array of values
<br>
<a href="https://github.com/serde-rs/serde/issues/637">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/3">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Derive macro to derive Default from Serde default attributes
<br>
<a href="https://github.com/serde-rs/serde/issues/1416">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/4">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Serde format for in situ JSON deserialization
<br>
<a href="https://github.com/serde-rs/json/issues/318">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/7">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Minimalist YAML parser with support for borrowed string slices
<br>
<a href="https://github.com/dtolnay/serde-yaml/issues/94">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/9">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Miniserde derive macro that supports enums
<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/10">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Miniserde utilities library, like adapters for Display and FromStr
<br>
<a href="https://github.com/dtolnay/miniserde/issues/3">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/11">[Design]</a>
</td></tr></table>

<br>

<a name="procedural-macros"></a>
# [:steam_locomotive: Procedural macros, Syn](#procedural-macros)

<table><tr><td><ul><li></li></ul></td><td>
Query syntax and extractor for syntax tree elements
<br>
<a href="https://github.com/dtolnay/cargo-expand/issues/8">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/1">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Library to inline out-of-line <code>mod</code> items and resolve <code>#[path =
"..."]</code>
<br>
<a href="https://github.com/dpc/crev/issues/89">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/6">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Procedural macro reimplementation of
<a href="https://github.com/dtolnay/quote"><code>quote!</code></a>
to resolve some longstanding limitations
<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/8">[Design]</a>
</td></tr></table>

<br>

<a name="visualization"></a>
# [:mountain_cableway: Visualization](#visualization)

<table><tr><td><ul><li></li></ul></td><td>
Minimal API for generating color scheme for a chart that needs <i>n</i> colors
<br>
<a href="https://github.com/dtolnay/cargo-tally/issues/10">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/12">[Design]</a>
</td></tr></table>

<br>

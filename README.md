Crates that don't exist, but should
===================================

A collection of Rust project ideas.&emsp;[<i><b>&gt;</b>Skip the introduction
and jump to the list<b>&lt;</b></i>](#the-list)

These are bite-sized ideas for which someone already has a mostly clear design
in mind. They are waiting on an interested library developer to carry through
the implementation and own the code. The requester should be prepared to offer
guidance on any API design questions that arise during implementation.

Ideas should result in their own useful library, even if that is just a few
functions. Ideas for which the code would go in some existing project should be
filed on that project's issue tracker rather than being listed here.

Many of these would make neat projects for a Rust beginner.

<br>

### Contributing

To work on an idea, click through on one of the "Design" links to read more
about the idea and coordinate as you make progress on the library.

To add a project idea, please file an issue with enough detail so that anyone
interested can understand the design you have in mind. Include links to relevant
background material if possible. Then send a PR adding a link to your issue.
Feel free to add a new heading if none of the existing ones apply to your idea.

<br>

### Getting help

For some ideas the person who posted them may be available to provide mentorship
on the design thread, but this is not a requirement. If you find yourself stuck,
swing by the [Rust Users] forum or the [Rust Discord] chat channel. Explain what
you are working on and where you got stuck, and they will be able to help you
out.

[Rust Users]: https://users.rust-lang.org/
[Rust Discord]: https://discord.gg/rust-lang

If you are interested in providing mentorship to people working through a
project idea, subscribe to individual design threads or "Watch" the whole repo
([here][subscription]) to follow all the threads.

[subscription]: https://github.com/dtolnay/request-for-implementation/subscription

<br>

### Relationship to Not-Yet-Awesome Rust

The [not-yet-awesome] list is similarly a catalog of project ideas, but the
scope is much broader than the one here. Some examples from their list:

- A stream processing pipeline with back pressure for asynchronous processing;
- A deep learning toolkit with GPU support;
- A mature framework for Windows native UI.

These are things that will involve a significant amount of design work, feedback
from multiple stakeholders, a responsive and dedicated maintainer or team, and
likely months to years of bake time before they would be considered awesome.

Their list does include some smaller project ideas too but very few of them come
with a thought-out design that someone could get started implementing
immediately.

In contrast, the Request For Implementation list is intended for ideas where a
design mostly already exists and can be concisely described. It should be ready
for someone to dive straight into code and it should be clear when a library has
accomplished the intended design.

[not-yet-awesome]: https://github.com/not-yet-awesome-rust/not-yet-awesome-rust

<br><a name="the-list"></a><br>

<!--
TEMPLATE:

<table><tr><td><ul><li></li></ul></td><td>
description description description description description description<br>
<a href="...">[Origin]</a>
—
<a href="...">[Design]</a>
</td></tr></table>

-->

<a name="command-line"></a>
# [:tractor:&ensp;Command line](#command-line)

<table><tr><td><ul><li></li></ul></td><td>
Cargo subcommand to perform pluggable expansions against rustdoc<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/20">[Design]</a>
</td></tr></table>

**Completed ideas:**

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library for a Cargo subcommand to find components installed under a different
toolchain<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/5">[Design]</a>
—
<a href="https://github.com/gsquire/toolchain_find">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Tool to enforce that Cargo.toml dependencies are written in sorted order<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/29">[Design]</a>
—
<a href="https://github.com/DevinR528/cargo-sort-ck">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Tool to streamline running public crate examples<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/30">[Design]</a>
—
<a href="https://github.com/BrandtM/cargo-example">[Outcome]</a>
</td></tr></table>
</blockquote>

<br>

<a name="cross-platform"></a>
# [:helicopter:&ensp;Cross platform](#cross-platform)

<table><tr><td><ul><li></li></ul></td><td>
Functions for normalizing and joining paths with consideration for UNC on
Windows<br>
<a href="https://github.com/rust-lang/cargo/issues/6198">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/34">[Design]</a>
</td></tr></table>

<br>

<a name="data-structures"></a>
# [:articulated\_lorry:&ensp;Data structures](#data-structures)

**Completed ideas:**

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library for writing const-compatible phantom types with explicit variance and
autotrait behavior<br>
<a href="https://github.com/rust-lang/rust/pull/57682#pullrequestreview-193857577">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/21">[Design]</a>
—
<a href="https://github.com/djmcgill/rich_phantoms">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Types for checked arithmetic on instants and durations<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/27">[Design]</a>
—
<a href="https://github.com/taiki-e/easytime">[Outcome]</a>
</td></tr></table>
</blockquote>

<br>

<a name="de-serialization"></a>
# [:bullettrain\_side:&ensp;De/serialization](#de-serialization)

<table><tr><td><ul><li></li></ul></td><td>
A dtd macro that you could point at an
<a href="https://en.wikipedia.org/wiki/Document_type_definition">XML DTD file</a>
and have it generate struct definitions for you<br>
<a href="https://twitter.com/chriskrycho/status/1085537088647249920">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/2">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Data format adapter to expose control over the representation of bytes<br>
<a href="https://github.com/serde-rs/json/pull/656">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/48">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Serde format for in situ JSON deserialization<br>
<a href="https://github.com/serde-rs/json/issues/318">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/7">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Minimalist YAML parser with support for borrowed string slices<br>
<a href="https://github.com/dtolnay/serde-yaml/issues/94">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/9">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Miniserde utilities library, like adapters for Display and FromStr<br>
<a href="https://github.com/dtolnay/miniserde/issues/3">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/11">[Design]</a>
</td></tr></table>

<table><tr><td><ul><li></li></ul></td><td>
Attribute macro to generate de/serialization functions for fields of big array
type<br>
<a href="https://github.com/serde-rs/serde/issues/631">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/17">[Design]</a>
</td></tr></table>

**Completed ideas:**

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Macro to serialize and deserialize trait object using internal type tag<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/14">[Design]</a>
—
<a href="https://github.com/dtolnay/typetag">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Attribute macro to skip serializing all fields of Option type<br>
<a href="https://github.com/serde-rs/serde/issues/947">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/18">[Design]</a>
—
<a href="https://docs.rs/serde_with_macros/1.0/serde_with_macros/attr.skip_serializing_none.html">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Derive macro to derive Default from Serde default attributes<br>
<a href="https://github.com/serde-rs/serde/issues/1416">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/4">[Design]</a>
—
<a href="https://github.com/TedDriggs/serde_default">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Derive macros to serialize and deserialize struct as an array of values<br>
<a href="https://github.com/serde-rs/serde/issues/637">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/3">[Design]</a>
—
<a href="https://github.com/kardeiz/serde_tuple">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Derive macro to compute Bincode size of type<br>
<a href="https://github.com/TyOverby/bincode/issues/263">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/26">[Design]</a>
—
<a href="https://github.com/jrmuizel/bincode-size">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Attribute macro to apply prefix to name of serialized fields or variants<br>
<a href="https://github.com/serde-rs/serde/pull/1426">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/19">[Design]</a>
—
<a href="https://github.com/jonathan-s/serde-prefix">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Wrapper to strip pseudo-JSON comments from an io::Read input stream<br>
<a href="https://github.com/serde-rs/json/pull/514">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/24">[Design]</a>
—
<a href="https://crates.io/crates/json_comments">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Miniserde derive macro that supports enums<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/10">[Design]</a>
—
<a href="https://github.com/eupn/miniserde-derive-enum">[Outcome]</a>
</td></tr></table>
</blockquote>

<br>

<a name="procedural-macros"></a>
# [:steam\_locomotive:&ensp;Procedural macros, Syn](#procedural-macros)

<table><tr><td><ul><li></li></ul></td><td>
Attribute macro for conditional compilation options<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/44">[Design]</a>
</td></tr></table>

**Completed ideas:**

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Query syntax and extractor for syntax tree elements<br>
<a href="https://github.com/dtolnay/cargo-expand/issues/8">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/1">[Design]</a>
—
<a href="https://github.com/TedDriggs/syn-select">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Attribute macro to make a trait boxed clonable<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/13">[Design]</a>
—
<a href="https://github.com/kardeiz/objekt-clonable">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Procedural macro reimplementation of
<a href="https://github.com/dtolnay/quote">quote!</a>
to resolve some longstanding limitations<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/8">[Design]</a>
—
<a href="https://github.com/Goncalerta/proc-quote">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library to inline out-of-line mod items and resolve #[path = "..."]<br>
<a href="https://github.com/dpc/crev/issues/89">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/6">[Design]</a>
—
<a href="https://github.com/TedDriggs/syn-inline-mod">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library for parsing function signature without parsing function body<br>
<a href="https://github.com/dtolnay/syn/issues/467">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/16">[Design]</a>
—
<a href="https://github.com/taiki-e/syn-mid">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Derive macro for computing total memory occupied by a data structure<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/22">[Design]</a>
—
<a href="https://github.com/Aeledfyr/deepsize">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library to serialize and deserialize Syn syntax trees<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/25">[Design]</a>
—
<a href="https://github.com/taiki-e/syn-serde">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Testing tool for comparing output of macro against expected source code<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/28">[Design]</a>
—
<a href="https://github.com/eupn/macrotest">[Outcome]</a>
</td></tr></table>
</blockquote>

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Library + tool to list all source files of a crate<br>
<a href="https://github.com/dtolnay/request-for-implementation/issues/38">[Design]</a>
—
<a href="https://github.com/Areredify/srcfiles">[Outcome]</a>
</td></tr></table>
</blockquote>

<br>

<a name="visualization"></a>
# [:mountain\_cableway:&ensp;Visualization](#visualization)

**Completed ideas:**

<blockquote>
<table><tr><td><ul><li></li></ul></td><td>
Minimal API for generating color scheme for a chart that needs <i>n</i>
colors<br>
<a href="https://github.com/dtolnay/cargo-tally/issues/10">[Origin]</a>
—
<a href="https://github.com/dtolnay/request-for-implementation/issues/12">[Design]</a>
—
<a href="https://github.com/BrandtM/colourado">[Outcome]</a>
</td></tr></table>
</blockquote>

<br>

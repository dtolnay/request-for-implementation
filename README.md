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

# De/serialization

- [ ] A `dtd` macro that you could point at an [XML DTD file] and have it
  generate struct definitions for you<br>
  [\[Origin\]][dtd-origin] -- [\[Design\]][dtd-design]

[XML DTD file]: https://en.wikipedia.org/wiki/Document_type_definition
[dtd-origin]: https://twitter.com/chriskrycho/status/1085537088647249920
[dtd-design]: https://github.com/dtolnay/request-for-implementation/issues/2

- [ ] Derive macros to serialize and deserialize struct as an array of
  values<br>
  [\[Origin\]][serde-tuple-origin] -- [\[Design\]][serde-tuple-design]

[serde-tuple-origin]: https://github.com/serde-rs/serde/issues/637
[serde-tuple-design]: https://github.com/dtolnay/request-for-implementation/issues/3

- [ ] Derive macro to derive Default from Serde default attributes<br>
  [\[Origin\]][default-serde-origin] -- [\[Design\]][default-serde-design]

[default-serde-origin]: https://github.com/serde-rs/serde/issues/1416
[default-serde-design]: https://github.com/dtolnay/request-for-implementation/issues/4

<br>

# Procedural macros, Syn

- [ ] Query syntax and extractor for syntax tree elements<br>
  [\[Origin\]][rustq-origin] -- [\[Design\]][rustq-design]

[rustq-origin]: https://github.com/dtolnay/cargo-expand/issues/8
[rustq-design]: https://github.com/dtolnay/request-for-implementation/issues/1

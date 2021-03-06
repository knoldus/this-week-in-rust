Title: This Week in Rust 279
Number: 279
Date: 2019-03-26
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

[GNOME Google Summer of Code](https://twitter.com/sdroege_/status/1109135842793148419): couple of Rust-related ideas lined up for this year's GSOC. From low-level libraries like Gstreamer, and Librsvg, to system services, to desktop applications. More details can be found by searching [this wiki page](https://wiki.gnome.org/Outreach/SummerOfCode/2019/Ideas)


# Crate of the Week

This week's crate is [safety-guard](https://gitlab.com/tdiekmann/safety-guard), a crate providing a `#[safety]` attribute that generates both a doc entry and debug assertion. Thanks to [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/506) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Rust and WebAssembly WG: Let's build Gloo together](https://rustwasm.github.io/2019/03/12/lets-build-gloo-together.html).
* [gfx-rs: Call for participation](https://users.rust-lang.org/t/gfx-rs-call-for-participation/26410).
- [grpc-rs: Add support for well-known types](https://github.com/pingcap/grpc-rs/issues/276)
- [TiKV: Flush logs on fatal errors](https://github.com/tikv/tikv/issues/4328)
- [TiKV: Disable test suites that contain no tests](https://github.com/tikv/tikv/issues/4391)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

169 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-03-18..2019-03-25

* [Move libtest out of rust-lang/rust](https://github.com/rust-lang/rust/pull/57842)
* [Introduce assembly tests suite](https://github.com/rust-lang/rust/pull/58791)
* [syntax: Better recovery for `$ty::AssocItem` and `ty!()::AssocItem`](https://github.com/rust-lang/rust/pull/59058)
* [MIR optimization: Run branch cleanup after copy propagation](https://github.com/rust-lang/rust/pull/59290)
* [Do not complain about non-existing fields after parse recovery](https://github.com/rust-lang/rust/pull/59266)
* [Make meta-item API compatible with `LocalInternedString::get` soundness fix](https://github.com/rust-lang/rust/pull/59256)
* [Use a valid name for graphviz graphs](https://github.com/rust-lang/rust/pull/59251)
* [When moving out of a for loop head, suggest borrowing it](https://github.com/rust-lang/rust/pull/59195)
* [When encountering `||{}()`, suggest the likely intended `(||{})()`](https://github.com/rust-lang/rust/pull/59035)
* [Point at coercion reason for `if` expressions without else clause if caused by return type](https://github.com/rust-lang/rust/pull/58981)
* [Elide object safety errors on non-existent trait function](https://github.com/rust-lang/rust/pull/58929)
* [Unify `OsString`/`OsStr` for byte-based implementations](https://github.com/rust-lang/rust/pull/58953)
* [Add provided methods `Seek::`{`stream_len`, `stream_position`}](https://github.com/rust-lang/rust/pull/58422)
* [Add `todo!()` macro](https://github.com/rust-lang/rust/pull/56348)
* [Implement `ExactSizeIterator` for `ToLowercase` and `ToUppercase`](https://github.com/rust-lang/rust/pull/58778)
* [Make `Option<ThreadId>` no larger than `ThreadId` with `NonZeroU64`](https://github.com/rust-lang/rust/pull/59291)
* [Stabilize `refcell_map_split` feature](https://github.com/rust-lang/rust/pull/59280)
* [Add const generics to rustdoc](https://github.com/rust-lang/rust/pull/59170)
* [crates.io: Allow download counts to fail to be updated](https://github.com/rust-lang/crates.io/pull/1675)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: merge] [Transparent Unions and Enums](https://github.com/rust-lang/rfcs/pull/2645).
* [disposition: merge] [Stabilize the alloc crate](https://github.com/rust-lang/rfcs/pull/2480).
* [disposition: postpone] [Initial pipeline rfc](https://github.com/rust-lang/rfcs/pull/2656).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Add provided methods `Seek::{stream_len, stream_position}`](https://github.com/rust-lang/rust/pull/58422).
* [disposition: merge] [Tracking issue for {f32, f64}::copysign](https://github.com/rust-lang/rust/issues/58046).

## New RFCs

* [`std` Aware Cargo](https://github.com/rust-lang/rfcs/pull/2663).

# Upcoming Events

### Online

* [Mar 27. Rust Community Team Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).

### Africa

* [Mar 30. Nairobi, KE - Rust Nairobi Meetup: Projects Showcase](https://www.meetup.com/Rust-Nairobi/events/259650701/).

### Asia Pacific

* [Mar 25. Melbourne, AU - Rust Melbourne Meetup](https://www.meetup.com/Rust-Melbourne/events/259230502/).
* [Mar 25. Auckland, NZ - Rust AKL Meetup](https://www.meetup.com/rust-akl/events/259480499/).
* [Mar 25. Tokyo, JP - Tokyo Rust Meetup](https://rust.connpass.com/event/122377/).
* [Mar 29. Noida, IN - Fearless Concurrency in Rust - Knoldus Meetup](https://www.meetup.com/Reactive-Application-Programmers-in-Delhi-NCR/events/259722745/).
* [Apr 20. Beijing, CN - RustCon Asia](https://rustcon.asia/)

### Europe

* [Mar 21. Kharkiv, UA -  PeerLab Kharkiv #Rust](https://dou.ua/calendar/25951/).
* [Mar 21. Grenoble, FR - Rust Meetup - FLOSS Grenoble](https://www.meetup.com/FLOSS-Grenoble/events/259118704/).
* [Mar 21. Torino, IT - Turin Rust Meetup](https://www.meetup.com/Mozilla-Torino/events/ktqcpqyzfblc/).
* [Mar 26. Berlin, DE - Rust and Tell Berlin](https://www.meetup.com/Rust-Berlin/events/szgnqqyzfbjc/).
* [Mar 28. Copenhagen, DK - Copenhagen Rust Hack Night #14](https://cph.rs/).
* [Mar 28. Toulouse, FR - Rust Toulouse meetup](https://www.meetup.com/fr-FR/Toulouse-Rust-Meetup/events/259589986/).
* [Apr  3. Sandown, ZA - Johannesburg meetup](https://www.meetup.com/Johannesburg-Rust-Meetup/events/gpxrtqyzgbfb/).
* [Apr  3. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/rjgkhqyzgbfb/).
* [Apr 04. Wroclaw, PL - Rust Wroclaw Meetup](https://www.meetup.com/Rust-Wroclaw/events/259511136/).
* [Jun 28-29. Firenze, IT - RustLab](https://www.rustlab.it/).

### North America

* [Mar 25. Durham, US - Triangle Rustaceans](https://www.meetup.com/triangle-rustaceans/events/mfglwpyzfbhc/).
* [Mar 27. Chicago, US - Chicago Rust Meetup - Futures in Haskell and Rust](https://www.meetup.com/Chicago-Rust-Meetup/events/259343384).
* [Mar 27. Ann Arbor, US - Ann Arbor Rust Meetup](https://www.meetup.com/Ann-Arbor-Rust-Meetup/events/cgsskqyzfbkc/).
* [Mar 27. Mesa, US - Phoenix Rust: Scientific Computing](https://www.meetup.com/Desert-Rustaceans/events/259615926/).
* [Apr  3. Indianapolis, US - Indy.rs](https://www.meetup.com/indyrs/events/246726699/).
* [Apr  3. Atlanta, US - Rust Atlanta Meetup](https://www.meetup.com/Rust-ATL/events/lgtvsqyzgbfb/).
* [Apr  3. Vancouver, CA - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/gqbksqyzgbfb/).

### South America

* [Mar 29. Montevideo, UY - Rust Latam @ Montevideo, Uruguay](https://rustlatam.org/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Database Engineer Developer at Parity, Berlin, DE](https://www.parity.io/jobs/#berlin-database-engine-developer).
* [Rust Software Consultant at Knoldus, Noida, IN](https://www.knoldus.com/careers/rust-software-consultant.knol).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> all the ergonomic improvements in rust 2018 are really messing up my book that consists entirely of running face-first into compiler errors so i can explain concepts.

– Alexis Beingessner, author of “Learning Rust With Entirely Too Many Linked Lists”

Thanks to [icefoxen](https://users.rust-lang.org/t/twir-quote-of-the-week/328/631) for the suggestion!

[Please submit your quotes for next week](http://users.rust-lang.org/t/twir-quote-of-the-week/328)!

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [Flavsditz](https://github.com/Flavsditz).*

<small>[Discuss on r/rust]().</small>

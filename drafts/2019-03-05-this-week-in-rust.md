Title: This Week in Rust 276
Number: 276
Date: 2019-03-05
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

# Crate of the Week

This week's crate is [shellfn](https://crates.io/crates/shellfn), a proc macro to easily and safely use shell scripts in Rust. Thanks to [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/490) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [RustConf CfP is now open](https://cfp.rustconf.com/events/rustconf-2019).
* [RustFest is searching for local teams to apply for the next events](https://blog.rustfest.eu/call-for-teams).
* [Rust: Add LLVM atomic memcpy intrinsics, expose in core/std](https://github.com/rust-lang/rust/issues/58599).
* [TiKV: support ALLOW_INVALID_DATES in coprocessor](https://github.com/tikv/tikv/issues/4100).
* [TiKV: Use breakpad + symbolic to generate and interpret minidump-format core dumps](https://github.com/tikv/tikv/issues/4202).
* [TiKV: Make git dependency revisions explicit in Cargo.toml](https://github.com/tikv/tikv/issues/4283).
* [LSD: Looking for maintainers](https://github.com/Peltoche/lsd/issues/131).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

245 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-02-18..2019-02-25

* [Add an unstable option to build proc macros for both the host and the target](https://github.com/rust-lang/cargo/pull/6547)
* [Avoid ICE when region sneaks into impl trait](https://github.com/rust-lang/rust/pull/58649)
* [Add const generics to the HIR](https://github.com/rust-lang/rust/pull/58503)
* [Improve parsing diagnostic for negative supertrait bounds](https://github.com/rust-lang/rust/pull/57364)
* [Optimise `vec![false; N]` to zero-alloc](https://github.com/rust-lang/rust/pull/58628)
* [Add expected/provided byte alignments to validation error message](https://github.com/rust-lang/rust/pull/58658)
* [Remove `LazyTokenStream`](https://github.com/rust-lang/rust/pull/58476)
* [Add better error message for partial move](https://github.com/rust-lang/rust/pull/58199)
* [Suggest removing parentheses surrounding lifetimes](https://github.com/rust-lang/rust/pull/58198)
* [Use normal mutable borrows in matches](https://github.com/rust-lang/rust/pull/57609)
* [Monomorphize less code in `fs::`{`read`, `write`}](https://github.com/rust-lang/rust/pull/58530)
* [Make overflowing and wrapping negation const](https://github.com/rust-lang/rust/pull/58044)
* [Fix overlapping references in BTree](https://github.com/rust-lang/rust/pull/58431)
* [Relax some Ord bounds on BinaryHeap<T>](https://github.com/rust-lang/rust/pull/58421)
* [Relax some Hash bounds on HashMap<K, V, S> and HashSet<T, S>](https://github.com/rust-lang/rust/pull/58370)
* [Turn duration consts into associated consts](https://github.com/rust-lang/rust/pull/58595)
* [`RangeInclusive` internal iteration performance improvement](https://github.com/rust-lang/rust/pull/58122)
* [Override `VecDeque::try_rfold`, also update iterator](https://github.com/rust-lang/rust/pull/58064)
* [Stabilize `TryFrom` and `TryInto` with a `convert::Infallible` empty enum](https://github.com/rust-lang/rust/pull/58302)
* [Stabilize `iter::successors` and `iter::from_fn`](https://github.com/rust-lang/rust/pull/58576)
* [Destabilize fixed-width const defined atomic integers](https://github.com/rust-lang/rust/pull/58616)
* [Deprecate the unstable `Vec::resize_default`](https://github.com/rust-lang/rust/pull/57656)
* [Modify doctest's auto-`fn main()` to allow `Result`s](https://github.com/rust-lang/rust/pull/56470)
* [crates.io: Stop logging the referer header](https://github.com/rust-lang/crates.io/pull/1636)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC 2627: `#[link(kind="raw-dylib")]`](https://github.com/rust-lang/rfcs/pull/2627).
* [RFC 2532: Associated type defaults](https://github.com/rust-lang/rfcs/pull/2532).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

*No RFCs are currently in final comment period.*

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Add FromStr impl for NonZero types](https://github.com/rust-lang/rust/pull/58717).
* [disposition: merge] [Cosmetic changes to compiler comments and docs](https://github.com/rust-lang/rust/issues/58619).

## New RFCs

* [Initial pipeline rfc](https://github.com/rust-lang/rfcs/pull/2656).
* [Add Destructuring assignment](https://github.com/rust-lang/rfcs/pull/2649).

# Upcoming Events

### Online

* [Mar  6. Rust Community Team Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).
* [Mar 11. Rust Community Content Subteam Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).
* [Mar 13. Rust Events Team Meeting on Telegram](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).
* [Mar 20. Rust Community Team Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).

### Asia Pacific

* [Mar  6. Selangor, MY - Rust Malaysia Meetup Kuala Lumpur](https://www.facebook.com/events/1128655260646848/).

### Europe

* [Mar  6. Sandown, ZA - Johannesburg meetup](https://www.meetup.com/Johannesburg-Rust-Meetup).
* [Mar  6. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/rjgkhqyzfbjb/).
* [Mar 11. Stockholm, SE - Rust Meetup Stockholm First one for 2019](https://www.meetup.com/ruststhlm/events/259387426/).
* [Mar 14. Brno, CZ - Rust Brno Meetup at Masaryk University](https://rust-brno.github.io/)
* [Mar 14. Göteborg, SE - Rust Gothenburg](https://www.meetup.com/rustgbg/events/259386306/).
* [Mar 19. Nijmegen, NL - Rust Nijmegen: Rust for the (Inter)Net - API's, HTTP/3 and Tide](https://www.meetup.com/Rust-Nijmegen/events/258758167).
* [Mar 19. Paris, FR - Paris - Rust Paris](http://www.meetup.com/Rust-Paris).
* [Mar 20. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/find/events/?allMeetups=false&keywords=Rust+Hack+and+Learn+OpenTechSchool&radius=25&userFreeform=Berlin%2C+Germany&mcName=Berlin%2C+DE&eventFilter=all).

### North America

* [Mar  6. Indianapolis, US - Indy.rs](https://www.meetup.com/indyrs/events/mffbtpyzfbjb/).
* [Mar  6. Atlanta, US - Rust Atlanta Meetup](https://www.meetup.com/Rust-ATL/events/cbcmbqyzfbjb/).
* [Mar  6. Vancouver, CN - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/hkllqqyzfbjb/).
* [Mar  9. 200 University Ave W, Waterloo, CN - Workshop: Introduction to Game Development in Rust!](https://www.meetup.com/Rust-KW/events/259335419/).
* [Mar 11. Seattle, US - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/nzfspqyzfbpb/).
* [Mar 13. Ciudad de México, MX - Study group RustMX](https://www.meetup.com/Rust-MX/events/259473143/).
* [Mar 14. Columbus, US - Columbus Rust Society](https://www.meetup.com/columbus-rs/events/dbcfrpyzfbsb/).
* [Mar 14. Utah, US - Utah Rust monthly meetup](https://www.meetup.com/utahrust/events/258703993/).
* [Mar 14. San Diego, US - San Diego Rust](http://meetu.ps/c/2vF0G/4DXV4/a).
* [Mar 20. Vancouver, CN - Vancouver Rust meetup](https://www.meetup.com/Vancouver-Rust/events/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Software Engineer at TenX, Singapore](https://tenx.workable.com/jobs/689264).
* [Software Engineer - Blockchain at TenX, Sydney, AU](https://tenx.workable.com/jobs/689268).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

Sadly, no quotes were nominated this week.

[Please submit your quotes for next week](http://users.rust-lang.org/t/twir-quote-of-the-week/328)!

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [Flavsditz](https://github.com/Flavsditz).*

<small>[Discuss on r/rust]().</small>
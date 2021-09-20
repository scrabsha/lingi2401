# Open Source Contribution Project
*Author:* Sasha Pourcelot

*NOMA:* 26212100

*Year:* 2021

*Selected project:* [The Rust Compiler](https://github.com/rust-lang/rust)

# Project research and selection

I discovered the Rust Programming Language when I started University and try
to participate to its development. I have already done a few contributions
([1], [2], [3]) which improve the error messages emitted during
parsing in very specific situations.

[1]: https://github.com/rust-lang/rust/pull/75779
[2]: https://github.com/rust-lang/rust/pull/76160
[3]: https://github.com/rust-lang/rust/pull/88546

As I love this language and the community that formed around it, I'd like to
contribute to its development again. I think [issue #27300][4] is a good
candidate. 

[4]: https://github.com/rust-lang/rust/issues/27300

# Issue description

This issue points out that the closures written with the Ruby syntax are
syntatically valid in Rust, but are not parsed the correct way, which causes
a very weird error messsage during the type-checking process.

# First contact related to the issue

*Brief note*: part of the Rust developpment discussions happen on Zulip. It
is necessary to log on the platform in order to see messages. Any GitHub
account can be used to do so.

I made my first contact with the Rust developpment team when I claimed issue
[#88065]. I was then invited to join the Rust Developpment Zulip chat in order
to discuss with other developpers. Once I [joined][scrabsha_joins_zulip] the
chat, [Esteban Küber gave me a brief overview][ekuber_overview] of the fix, and
[suggested][ekuber_suggests_ruby_style] me to fix [#27300] as well. After a few
weeks of developpment, [my fix][#88546] for [#88065] is merged in the compiler
(it can even be tested [on the playground][88065-playground]).

[#88065]: https://github.com/rust-lang/rust/issues/88065
[scrabsha_joins_zulip]: https://rust-lang.zulipchat.com/#narrow/stream/122652-new-members/topic/First.20non-trivial.20contribution/near/249564563
[ekuber_overview]: https://rust-lang.zulipchat.com/#narrow/stream/122652-new-members/topic/First.20non-trivial.20contribution/near/249567668
[#27300]: https://github.com/rust-lang/rust/issues/27300
[ekuber_suggests_ruby_style]: https://github.com/rust-lang/rust/issues/88065#issuecomment-899358405
[#88546]: https://github.com/rust-lang/rust/pull/88546
[88065-playground]: https://play.rust-lang.org/?version=nightly&mode=debug&edition=2018&gist=4f0041a6ecc12a9bbf9fc5ffeb3e9be6

Now that [#88065] is fixed, I have plenty of time to work on [#27300]. On
september 20, I described [an idea of fix][scrabsha_tries_to_fix_27300] on
Zulip.

[scrabsha_tries_to_fix_27300]: https://rust-lang.zulipchat.com/#narrow/stream/147480-t-compiler.2Fwg-diagnostics/topic/Parse.20closure.20missing.20braces.20around.20body.20.2388065/near/254020404
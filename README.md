# xchatnickcolor

A modified version of irssi nick-colouring script `xchatnickcolor.pl`. Makes the
following improvements:

* Nick colours now always match their equivalents in xchat
* No longer remembers nick colours across nickchanges
* Uses %K (dark grey) instead of %b (blue) for angle brackets around nicks

## History

In 2002, the original `xchatnickcolor.pl` added xchat-style nick colouring to
irssi. Each user nick has a colour calculated from the letters in the nick, so
that any given nick will always have the same name.

However, the colours calculated by `xchatnickcolor.pl` didn't always match the
colours calculated by xchat. This new version fixes that. Now, anyone whose nick
is red in xchat will be red in irssi, and so on.

This version also disables the feature to temporarily retain a user's colour
across nick changes. It was inconsistent and broke compatibility with xchat. You
can uncomment the last line to turn it back on.

## Other versions

The irssi website now has a script called `nickcolor.pl`, an updated version of
the original `xchatnickcolor.pl` which supports custom colour sets. If you're
using that script instead of this one, and just want xchat-compatible colours,
the following command 

`/set nickcolor_colors 19 20 22 23 25 26 27 28 29`

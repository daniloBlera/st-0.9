# A fork of ST 0.9 with my configs

Version forked: [0.9](https://dl.suckless.org/st/st-0.9.tar.gz)

## Patches applied

* iso 14755 ([st-iso14755-0.8.5.diff][iso])
* scrollback ([st-scrollback-ringbuffer-0.8.5.diff][scrollback])
* ligatures ([st-ligatures-scrollback-ringbuffer-0.9][ligatures])
* anysize ([st-expected-anysize-0.9.diff][anysize])
* xresources ([st-xresources-20200604-9ba7ecf.diff][xresources])

[iso]: https://st.suckless.org/patches/iso14755/st-iso14755-0.8.5.diff
[scrollback]: https://st.suckless.org/patches/scrollback/st-scrollback-ringbuffer-0.8.5.diff
[ligatures]: https://st.suckless.org/patches/ligatures/0.9/st-ligatures-scrollback-ringbuffer-20230105-0.9.diff
[anysize]: https://st.suckless.org/patches/anysize/st-expected-anysize-0.9.diff
[xresources]: https://st.suckless.org/patches/xresources/st-xresources-20200604-9ba7ecf.diff

st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

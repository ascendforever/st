# st


This is a fork of suckless `st` with a few patches and custom configurations applied.

`st` is a simple terminal emulator for X which sucks less.

##### Patches
- anysize
- autocomplete
- scrollback-reflow-standalone-extended
- undercurl
- workingdir
- xresources

##### Other changes
- Alternate colorscheme
- Autocomplete modkey: Alt
- Default font: Inconsolataa





## Install

Debian and Fedora packages are available.
See [AscendForever/repos](https://ascendforever.com/repos)
    [[secure]](https://secure.ascendforever.com/repos)
    [[tor]](http://zuh3vfagsxufncxiyhrsu4wbcihjdexzvsvm2zoxtypiqjh7nvtdkkqd.onion/repos)
    [[i2p]](http://xryyir2gvnjhdxlsjx2ajdqps4p3yxh5tczboumrizagd4tavwcq.b32.i2p/repos)
    for instructions.





## Upstream readme

```markdown
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
```

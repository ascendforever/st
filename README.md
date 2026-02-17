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





# Install



### Debian package
Debian packages are available for stable and oldstable releases.


#### Install the signing key
Clearnet:
```bash
curl https://deb.ascendforever.com/ascendforever.gpg | sudo tee /usr/share/keyrings/ascendforever.gpg >/dev/null
```
Or onion:
```bash
curl http://csjkrevghycpr6b266bk2hrgfotoxsz7xbyfk6rkk63fxlbkbes7b7qd.onion | sudo tee /usr/share/keyrings/ascendforever.gpg >/dev/null
```


#### Add repository
Change `trixie` -> `bookworm` if needed.

Clearnet:
```bash
printf 'deb [signed-by=/usr/share/keyrings/ascendforever.gpg] https://deb.ascendforever.com %s main' trixie | sudo tee /etc/apt/sources.list.d/ascendforever.list
```
Or onion:
```bash
printf 'deb [signed-by=/usr/share/keyrings/ascendforever.gpg] tor+http://csjkrevghycpr6b266bk2hrgfotoxsz7xbyfk6rkk63fxlbkbes7b7qd.onion %s main' trixie | sudo tee /etc/apt/sources.list.d/ascendforever.list
```


#### Install
```bash
sudo apt install -y st-af
```





## Original readme
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

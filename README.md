# nethack-3.6.0-for-minix3
This gives you the X11 version and it need X running <br />
<br />
From the root directory of nethack 3.6.0 as normal user execute x11 or tty patch: <br />
For x11: <br />
$ patch -p0 -i mypatchx11.diff <br />
or <br />
For tty: <br />
$ patch -p0 -i mypatchtty.diff <br />
<br />
$ cd sys/unix <br />
$ ./setup.sh hints/unix <br />
$ cd ../.. <br />
1-25-2020 the current nethack you should run $ make fetch-Lua at this moment.  cd lib/lua-*/src.  Replace * with the version there.  Edit Makefile with vi and change gcc to clang the rest of the commands should work. <br />
$ make <br />
$ make install <br />
$ cd <br />
<br />
You will need to execute every time if you don't add to your path: <br />
$ export PATH=/home/$USER/games:$PATH <br />
<br />
Then execute: <br />
$ nethack <br />

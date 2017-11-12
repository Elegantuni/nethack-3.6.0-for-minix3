# nethack-3.6.0-for-minix3
This gives you the X11 version and it need X running <br />
<br />
From the root directory of nethack 3.6.0 execute: <br />
patch -p0 -i mypatch.diff <br />
cd sys/unix <br />
./setup.sh hints/unix <br />
cd ../.. <br />
make <br />
make install <br />
cd <br />
<br />
You will need to execute every time if you don't add to your path: <br />
export PATH=/home/$USER/games <br />
<br />
Then execute: <br />
nethack <br />

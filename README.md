# nethack-3.6.0-for-minix3
This gives you the X11 version and it need X running

From the root directory of nethack 3.6.0 execute:
patch -p0 -i mypatch.diff
cd sys/unix
./setup.sh hints/unix
cd ../..
make
make install
cd

You will need to execute every time if you don't add to your path:
export PATH=/home/$USER/games

Then execute:
nethack

# Pepper/Nao Programming Tools on Ubuntu Desktop Dockerfile

This unoffical Docker container contains necessary tools to program Softbank's Pepper and Nao robots on a Linux environment. 

It has been tested only on Pepper robot. But, it will most probably work on Nao as well. Please let me know, if you run it.

It contains Ubuntu 16.04 desktop and a VNC server. You just need to connect to it by using a VNC client.

# How to run

`docker run -p 5901:5901 ocihangir/pepper-on-ubuntu-desktop`

and then connect to:

`vnc://<host>:5901` via VNC client.

The VNC password is `password`.

# Running tools

You can access Softbank Choregraphe Suite in the programming section of Ubuntu dashboard.

To access Python library, in a terminal window:

`python`

>>> import naoqi

# Choregraphe Suite public license key

Somehow during installation, Choregraphe Suite cannot check installation key. You can provide it during first run. 

Key : 654e-4564-153c-6518-2f44-7562-206e-4c60-5f47-5f45
(Obtained from : https://developer.softbankrobotics.com/us-en/downloads/pepper )

# Pepper documentation

Naoqi : http://doc.aldebaran.com/2-5/naoqi/index.html

Pepper : http://doc.aldebaran.com/2-5/home_pepper.html

Note : The parts related to VNC was taken from https://github.com/queeno/docker-ubuntu-desktop/
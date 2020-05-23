==========
obs-gphoto
==========

Forked from `https://github.com/dunkelstern/obs-gphoto`, which was forked from
`https://github.com/Atterratio/obs-gphoto.git`. Not sure if the upstream is still
active.

------
v0.4.0
------

MODULES
=======
gPhoto live preview capture
---------------------------
   Allows capture cameras preview like video.

Timelapse photo capture
-----------------------
   Allows capture photo with some intervals(if interval set to 0 work only manual capture) or manual with hotkey and camera capture button, to show work in progress on good picture quality, or to compile timelapse video in future.

REQUIREMENTS
============

* *obs-studio*
* *libgphoto >= 2.5.10*
* *libjpeg-turbo* (probably already installed on your distribution)
* *libudev(optional)*

INSTALLATION
============

For ArchLinux:
--------------

Use the included PKGBUILD


For installation from source:
=============================

Fedora: 
-------
Install requirements: :code:`dnf install libgphoto2-devel obs-studio-devel libjpeg-devel systemd-devel`

General:
--------
* :code:`git clone https://github.com/dunkelstern/obs-gphoto`
* :code:`cd obs-gphoto`
* :code:`cmake . -DSYSTEM_INSTALL=0` for local installation or :code:`cmake . -DSYSTEM_INSTALL=1` for system installation
* :code:`make`
* :code:`make install`

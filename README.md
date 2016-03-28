Adapta
=========
<img src="img/Button.gif" alt="Button" align="right" />
An adaptive Gtk+ theme based on Material Design Guidelines.
Lots of elements are forked from Flat-Plat: https://github.com/nana-4/Flat-Plat

Elements
--------
![Materials](img/Materials.png)

Required Components
-------------------
Adapta supports Gtk+ 3.20.x (and 3.18.x)

* Gtk+-3.0 >= 3.20 (or 3.18.4)
* Gtk+-2.0 >= 2.24.30 (or 2.24.29)
* gtk2-engines-pixbuf >= 2.24.30 (or 2.24.29)

Supported Desktop Environments
------------------------------
* GNOME 3.20 (or 3.18)
  * gnome-shell >= 3.19.92 (or 3.18.4)
  * mutter >= 3.19.92 (or 3.18.4)
* GNOME-Flashback 3.18.x
* budgie-desktop 10.2.x
* Unity7 7.4.0
* Cinnamon 2.8.x

Unity and Cinnamon are under W.I.P state.

Unsupported Gtk+ Based Desktops
-------------------------------
* Mate
* XFce4
* Pantheon

Installation
------------
1. Check `autoconf`, `automake` and `pkg-config` (`pkgconfig`) are installed.
2. Build and install system-wide:
   ```
   ./autogen.sh
   make
   sudo make install
   ```
   * Default prefix is `/usr`
   * `make` actually does nothing (for future release)
   * `sudo make install` installs multiple versioned themes,
     and Gtk+ automatically selects proper versioned one when running.

3. Run `gsettings set org.gnome.desktop.interface gtk-theme 'Adapta'` to enable the theme.
   (`gnome-tweak-tool` can NOT support multiple versioned theme?)

Work in Progress
----------------
* Conversion to Gtk+ 3.20 or git master
* Cinnamon 2.8 desktop integration

TODO
----

Public License
--------------
* License: GPLv2

Special Thanks to
--------------
Nana-4, the developer of Flat-Plat.

I built this bundle so I could use Michael Schwern's Class::DBI
package on Win32 systems. ActiveState has not published PPM-installable
bundles for these modules, so I built them myself. It wasn't too
hard once I figured out the incantations and after many chickens.

WARNING: This bundle has NOT been in Schwern's pants.

The PPM bundles in this ZIP file are as follows:
  Class-WhiteHole-0.03
  Class-Fields-0.10
  Class-Data-Inheritable-0.02
  Carp-Assert-0.11
  Class-Accessor-0.13
  Ima-DBI-0.23
  Class-DBI-0.15

You should build them in that order.
To build them, change directories into the appropriate directory.
Edit the .ppd file with notepad.exe or your favorite text editor.
Replace the path "D:\SRC\Win95\Perl" in the <CODEBASE HREF=""> tag
with whatever directory you unpacked this in.
Install the package with PPM using the command:
  ppm install --location=. <ppd basename>
where <ppd basename> is the basename of the ppd file in this directory.
e.g. in Class-DBI-0.15, you would type:
  ppm install --location=. Class-DBI

That should be all.
Note, these ppd files have no author (Michael Schwern) or descriptions
in them.

Good Luck.
Michael King (mike808@users.sourceforge.com)

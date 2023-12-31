OpenGFX+ Landscape Minus
------------------

This version: OpenGFX+ Landscape Minus v7140 (178d7491052b)

Contents:

1 About
2 Usage
  2.1 Parameters
  2.2 Incompatibilities with other NewGRF
3 Contributing
  3.1 Translations
  3.2 Sprites and code
4 License
5 Credits



-------
1 About
-------

OpenGFX+ Landscape Minus is a stripped down version of OpenGFX+ Landscape 
to use with other landscape basesets or GRFs. It keeps the configurable
snowline and provides a few selected NewObjects to populate a landscape.

Minimum required OpenTTD version is 1.2.0 or r22723.
Some features require OpenTTD version 1.4.0 or r25230.

Name of this Repo:  OpenGFX+ Landscape Minus v7140 (178d7491052b)
Repository version: 7140
GRF_ID:             
MD5 sum:            {{GRF_MD5}}



-------
2 Usage
-------

Features of this NewGRF:

Variable, configurable snowline:
	Available for arctic and alpine landscape. You can set the snow height
	for mid January and mid June respectively. Snow will change in a
	sinoidal pattern between those two dates

NewObjects:
	* Wind turbin from 1985 onwards. They cannot be placed adjacent to
	  eachother
	* Company fenced land. Plain ground tiles or ground tiles with a fir
	  tree, surrounded by a fence. [OpenTTD 1.4.0 (r25230) recommended]
	* Communication tower from 1950 onwards.
	* Light house from 1492 onward

Rock instead of communication tower:
	For early scenarios communication towers may look out-of-place. Use
	this NewGRF parameter to replace it by a rock.

2.1 Parameters
--------------
* Transmitter replaced by rocks
	yes: Replace the communication transmitter by a rock. Suitable for
	     scenarios which play at an early time
	no:  No change. This is the default.
* Snow line mid January
	0 .. 16 (16 = nowhere) given in tile heights.
	default: 4
	If you play with more height levels, the steps are 1/16 of the maximum
	allowed height
* Snow line mid July
	0 .. 16 (16 = nowhere) given in tile heights
	default: 8
	If you play with more height levels, the steps are 1/16 of the maximum
	allowed height

2.2 Incompatibilities with other NewGRFs
----------------------------------------

- Canadian Station Set replaces or removes the default fences. This alters
    in the same way the fences of the fenced land
- SwedishRails allows to alter the default fences. This alters the fences
    of the fenced land in the same way.



--------------
3 Contributing
--------------

3.1 Translations
----------------

Additions of new languages or updates to existing translations are always
welcome.

Translations are managed by the DevZone's central NewGRF translations
service which allows you to translate the NewGRFs conveniently from
your web browser. It's found at:

http://translator.openttdcoop.org

You'll need to login there with your account from the #openttdcoop
DevZone (http://dev.openttdcoop.org) Simply register and apply as
translator for the language of your choice)

If you want to translate offline, obtain the language file from the
repository and use the english one as the base language. In those cases
post updates or new translations as an issue in the project's issue
tracker at http://dev.openttdcoop.org/projects/ogfx-landscape or in the
forum thread at tt-forums: http://www.tt-forums.net/viewtopic.php?f=26&t=52396


3.2 Sprites and code
--------------------

The source code can be obtained from the #openttdcoop DevZone at
http://dev.openttdcoop.org/projects/ogfx-landscape
or via mercurial checkout
hg clone http://hg.openttdcoop.org/ogfx-landscape

Requirements for running this Makefile successfully:
	NML r2074 or later
	gimp
	gcc
	make
	mercurial (recommended)
	python (recommended)
	tar
If you want to create a compressed bundle of the grf, you'll need additionally
	zip
	bzip2
	unix2dos (optional)
Windows only:
On Windows systems this means that you'll need to install MinGW and MSys
in order to obtain a posix compatible environment. Then the makefile can
be called the very same way as it is on linux and mac systems.
MinGW/MSys contain the above mentioned programmes and can be obtained from
http://www.mingw.org/ That site also features an excellent walk-through of
how to install it.



---------
4 License
---------

OpenGFX+ Landscape was written by Ingo von Borstel (aka planetmaker) and is
free to use for anyone under the terms of the GNU Pulic License v2 or
higher. See license.txt for details.

This program is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License version 2 (or, at your
discretion, any later version) as published by the Free Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the
Free Software Foundation, Inc.
1 Franklin Street, Fifth Floor
Boston, MA 02110-1301
USA.



---------
5 Credits
---------

Authors:
    Lead programmer:            Ingo von Borstel (aka planetmaker)
    General:                    Alberth
Graphics:
    Lead graphics artist:       Zephyris

    Canal dikes:                Zephyris, planetmaker
    Desert transition tiles:    planetmaker
    Foundations (gray stone):   Froix
    Foundations (bricks):       Froix
    Foundations (mossy stone):  Froix
    Gold mine (temperate):      Zephyris, planetmaker
    Maglev (temperate):         Zephyris, 2006TTD
    no grid roads:              Zephyris, planetmaker
    no grid rail tracks:        Zephyris, planetmaker
    Oil derrik ground tile:     Zephyris, planetmaker
    Plantation foundations:     Zephyris, planetmaker
    River and canal water:      Leppka, Zephyris, planetmaker
    River borders:              planetmaker, Zephyris
    Road tunnels:               V453000
    Rocky land:                 planetmaker, Zephyris
    Sea shores:                 planetmaker
    Transmitter to rock:        kamnet
    Wind powerplant:            Zephyris, andythenorth (animation stages)
    Transmitter:                Mr. X
Translations:
    Catalan:                    juanjo
    Croatian:                   Voyager1
    Dutch:                      Alberth
    English (US)                Supercheese
    Finnish:                    Juzza1
    French:                     arikover
    German:                     planetmaker, Jogio
    Hungarian:                  zaza, molace
    Indonesian:                 UseYourIllusion, Yoursnotmine
    Italian:                    Voyager1
    Korean:                     kevin, Telk
    Latin:                      Supercheese
    Russian:                    akasoft, George
    Scotish Gaelic:             GunChleoc
    Spanish:                    SilverSurferZzZ

Special thanks to
* Ammler and ^Spike^ for maintaining the DevZone where this repository is
  hosted.
* Alberth and PaulC for their extensive and detailed feedback
* frosch, Rubidium, Terkhen, V453000 and Yexo for their valuable input in form
  of advice and patches to this project.

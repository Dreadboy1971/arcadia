-----------------------------------------------------------------------

Dread's QuickMESS Launcher v4.64b (DOS)

Frequently Asked Questions (Mini FAQ)

-----------------------------------------------------------------------

Q: How do I run the program from DOS?

A: Just type "QS" while in your emulator directory (i.e. C:\MESS) and 
press the enter key.

-----------------------------------------------------------------------

Q: How do I run the program from Windows?

A: The program is installed in a common directory defined by the PATH 
statement in your AUTOEXEC.BAT file.  Typically, C:\QMLAUNCH.  You do 
not have to place or copy the program files in the same directory as 
MESS or any other emulator such is the case with other front-ends.  
This gives the user a single location to update the front-end.  All 
QuickMESS program files, and other files such as README's and docs will 
be located here.

Just Right-click the directory you want to start QuickMESS in and click 
"QuickMESS Here...". Simply double-click the QS.REG file to add a 
"right-click" function for directories/folders if you did not choose 
this option when installing.

-----------------------------------------------------------------------

Revision History:

-----------------------------------------------------------------------

April 27, 2000

- First Public Release! - Version 4.64b  (Taken From QuickMAME 4.xx)

New Features:

- Added an option for customizable "No Preview Available" image now.  
The default image no longer has to be used.  Just add a NOPIC.PCX file 
to your emulator directory.  QuickMESS will use look for this first 
before the default built-in image.  See QSMANUAL.DOC (MS Word 97 
format) for more info.

- Automatic checking of emulator executable.  Some people try to run QS 
directly from its directory instead of running it from their emulator 
directory as per the instructions.  I get a zillion e-mails about this.  
Basically, the program is installed in one location but can be run from 
any location to accommodate single location upgrades and keep the byte 
count lower.  Many people fail to understand this and run QS directly 
from its home directory.  This is not the way to do it.

Via the PATH statement, the program must be run in your emulator 
directory (i.e. C:\MESS) even though QS itself is not in this 
directory.  Of course, it will NOT be in C:\QMLAUNCH so the program 
will now report that you are using it incorrectly and will suggest you 
read the documentation like every good Samaritan should.  There is also 
an "ignore" option if it is desirable to disable this for expert mode, 
or special cases where there is no EXE argument for instances like 
calling other batch files, etc.  =)

-----------------------------------------------------------------------

-January 22, 2000

- Updated to 4.63b

Help:

- I still need some PNG code if anyone would like to help me out.  All 
my code's in 16-bit MS QuickBasic 4.5 & MASM 6.1 assembly.  All the 
C/C++ code for decoding PNG's is useless to me.  Can anyone build me an 
MS-compatible 16-bit language library (i.e. PNG.LIB & PNG.QLB) for 
QuickBasic?  Or even convert the C code to generic BASIC or assembly?  
PCX's ok for now, since all the other emulators still capture screen 
shots in PCX flavor, but it would be nice to be able to import both PCX 
& PNG since QuickMAME is mostly used for MAME.  =)

New Features:

- QMMANUAL.DOC updated accordingly.  FAQ section updated in manual and 
added to web site.

Bug Fixes:

- Mostly cosmetic & internal functionality changes.

- Automatic checking of non-existing files eliminating the risk of 
having to manually edit the QM.INI file.

- Eliminated extraneous database reloading.  Now the program only 
reloads only if files are changed, etc.  It's a big time saver when you 
have  2000 ROMs or so.

- Added warning message in PCX preview window about unsupported PCX 
files when loaded.  They will not be displayed all "goobly-gooped" now, 
instead the message will appear.

-----------------------------------------------------------------------

October 4, 1999

- Updated to 4.61b

New Features:

- Smooth Scroll added.  Some people using a previous version may not 
like this new feature.  It allows smooth scrolling of the game list 
with up/down and pgup/pgdn.  It just makes the text a little nicer 
looking.  By default it is enabled.  You can disable or adjust the 
settings under the "Effects" menu.  If you're running a slower system 
you will probably want to disable this feature.

-----------------------------------------------------------------------

August 12, 1999

- Updated to 4.60b

New Features:

- Password security.  Disables guest users from exiting the front-end 
or accessing the control panel.  This one's a request from "Borgdude".  
I guess he doesn't want his buddies bailing out of the menu and into 
trouble.  "Resistance is futile...", I guess.  Just click on the 
"Password" button to enabled this feature.  Press "ENTER" to disable 
the password.  Of course, the password is stored in the QM.INI file 
(for now) if anyone knows a thing or two about editing INI files.  Pro: 
You can delete it if you forget what it was.  Con: Anyone can look at 
it by simply opening the INI file and taking a peek.  If anyone wants 
to submit some encryption/decryption code I could scramble it.  Until 
then, it's just a low-security measure.  Maximum of 8 ASCII characters 
ranging from 32 (Space Bar) to 126 (Tilde "~").  It is NOT case-
sensitive so don't worry about where the CAPS LOCK is set.

-----------------------------------------------------------------------

July 21, 1999

- Updated to 4.54b

Bug Fixes:

- Sorry.  I forgot to include one of the most important files in the 
version 4.53 installation, QM.BAT.  This is now included in 4.54.

- Installation now prevents overwriting of QM.BAT & QM.PIF files, in 
the event that the user has customized them.

-----------------------------------------------------------------------

July 20, 1999

- Updated to 4.53b

Bug Fixes:

- Fixed another "Auto Name Resolve" bug.  The program would only ever 
execute "MAME -LISTFULL > LISTFULL.TXT" even if a user had AMAME, 
PMAME, KBMAME, etc.  This is now corrected to use whatever MAME program 
name is specified under the "Paths Options".  Geez, I hate bugs.

New Features:

- Modified the installation program to search for alternate QuickMAME 
path other than C:\QMLAUNCH.  The user no longer has to manually define 
the path if they choose something other than the C:\QMLAUNCH default 
directory.

-----------------------------------------------------------------------

July 18, 1999

- Updated to 4.52b

Bug Fixes:

- Auto Name Resolve function: Duplication entries eliminated.  When two 
ROMs with the same prefix were found (i.e. CIRCUS & CIRCUSC) both would 
refer to CIRCUS instead of "Circus" & "Circus Charlie" because it was 
the first match in the list.  This is now corrected to verify it is the 
proper ROM name.  Sorry about the problem.

New features included in this release:

- QuickMAME manual split into two files.  Instead of the legacy 
QMREADME.TXT file being the whole manual, I've split it into two files.  
QMREADME.TXT is now just a "What's New" file with chronological notes 
on updates.  QMMANUAL.DOC is the new manual containing lots of examples 
and snapshots of QuickMAME and its associated dialog windows and 
settings.  QMMANUAL.DOC is in Word 97 format.  If you require another 
format please e-mail me with your request.  Dreadboy@hotmail.com

- You can now take BMP (Windows Bitmap) snapshots of the front-end 
itself.  Outputs a 640x480 8-bit (256 color) BMP with the filename 
QMxxxxxx.BMP.  Use the F12 key to "snap" these screen shots.

-----------------------------------------------------------------------

July 5, 1999

- Updated to 4.51b

Help:

- I still need some code to decode PNG file LZW chunks.  Even a small-
sized little utility like a PNG2PCX.EXE program would be great.  That 
way I could shell from the program to create a temporary PCX file that 
QuickMAME can read.  That way PNG files can still be left on the system 
without having to convert them all to PCX.  Can anybody help with this 
one?

- I can't get 368x256 to work with TWEAK on my arcade monitor since 
MAME's 0.35RC1 release.  I keep reading "refer to VGATWEAK.TXT for more 
info" in MAME's README.TXT file, but unfortunately they haven't 
distributed that file with the source or the binary since April 1, 
1999.  So I'm still stuck with the old one which only had support and 
examples up to the 256x256 mode.  Nothing over 300 pixels horizontally.  
I can't find an update to the file anywhere, and no one seems to know 
the author's URL.  OK, I'm done whining now.  |c8

Bug Fixes:

- None that I know of.  I probably just created a bunch more.  Was 
tired while I was working on it.  Cursing the "TWEAK" switch all the 
way.

New features included in this release:

- Should be in line with the official binary release of MAME 0.35 
Final.  The Control Panel now sports an option to replace the old 
"DOUBLE/NODOUBLE" switches with "STRETCH/NOSTRETCH". I've managed to 
get about 99% of the games to display satisfactory with that bugger-of-
a-switch, TWEAK.  At first it really messed up my arcade monitor, 
because it is a fixed-frequency monitor, meaning that none of the modes 
can be scaled.  The approximate resolution of an NTSC CRT is about 
720x525, so I used to try and spank all my screen modes to fit into 
either 640x480, 320x240, or 320x200.  It all worked quite well until 
MAME introduced the TWEAK/NOTWEAK stuff.  The DOUBLE switch no longer 
worked to force MSPACMAN into a 640x480 screen instead of a doubled 
800x600 (which my video card won't do because of the fixed-freq monitor 
thing so the edges of the maze would always be cropped or the maze was 
way off-center and cropped, or whatever.)  The STRETCH switch doesn't 
work the same way as the DOUBLE switch used to - It gets stretched 
vertically, but not horizontally, and not for all games and/or screen 
modes.  Arghh!  Got it working finally after fiddling around with the 
MAME.CFG [TWEAK] frequencies for what seemed an eternity of "Hit n' 
miss".  Got every mode working except for 368x256.  Can't get it for 
the life of me.  But then the only games that seem to use this strange 
resolution are the "Lode Runner" arcade series, which really suck 
anyway compared to the original Lode Runner game so I ain't too worried 
'bout it.  OK, go nuts.

-----------------------------------------------------------------------

June 20, 1999

- Updated to 4.50b

Bug Fixes:

- Previously, a sound card type needed to be identified to pass 
SOUNDRATE and SOUNDBITS switches to MAME.  If "Default" was selected 
these switches would NOT be passed.  This is now corrected to pass them 
regardless of whether a sound card is specified or not.

New features included in this release:

- AUTOMATIC ROM NAME RESOLUTION!  Yes!  It's about time.  Prior to this 
version, only the 8-character ROM prefix name (i.e. "YARD" vs. "10-Yard 
Fight") was added to the database forcing the user to rename each ROM-
set.  This is no longer an issue.  QuickMAME now uses your latest 
version of MAME to resolve the proper names from the ROM names.  It 
does this by issuing the command "MAME -LISTFULL > LISTFULL.TXT" to 
DOS, then restarting, and then automatically resolving the names 
anytime new ROMs are found.  I was really getting sick of renaming all 
these new ROMs which I had no idea what their proper names were.  I 
would have to start each one in order to "get" the name to type into 
QuickMAME.  Much better, man.  Please keep in mind: This feature is 
only intended for use with MAME and not with other emulators such as 
Bloodlust emulators.  MAME is required to produce the list.  The exact 
program name is derived from the "Path" configuration within the 
program to determine whether you are using MAME, PMAME, AMAME, etc.  
For other emulators you still have to type in the name you desire for 
the ROM-set.  (i.e. System16, Callus, etc.)
 
- New "Tweak" field added to database for the new TWEAK/NOTWEAK switch 
in MAME 0.35RC1 to support tweaked video modes.  For more information 
on this new feature, please view the README.TXT file included with your 
latest release of MAME.

- Although the DOUBLE/NODOUBLE switch no longer works with MAME 
0.35RC1, I have left that field in there for two reasons...  1) For 
downward database compatibility.  2) Still required for previous 
versions of MAME prior to 0.35RC1 if that switch is at all used.

-----------------------------------------------------------------------

May 28, 1999

- Updated to 4.42b

Bug Fixes From v4.41b:

- Reconfigured "Reset All Defaults" field to actually work again.  
Sorry about that, I guess it hasn't been working for some time now.  I 
have always just deleted the QM.INI file manually to reset it I guess.  
It's working now.

New features included in this release:

- As per request from "Johnny" from Oslo, Norway, I have added an 
option to "attach" a single space character on the scroll list 
description as a "Leading Space" and/or a "Trailing Space".  And YES, 
Johnny, you're right --- it does look better.  You can find these new 
options under the "Effects" window.  By default, these variables are 
set to false so you have to enable them yourself if you prefer them.

- A couple of other minor window description changes that aren't really 
worth mentioning.

-----------------------------------------------------------------------

May 27, 1999

- Updated to 4.41b

HELP!

- The MAME team went and switched screen capturing to the PNG (Portable 
Network Graphics) format from PCX.  I spent weeks working on assembly 
code to "de-ice" multiple color-depth PCX files.  Now they've gone and 
changed it, even though all the other DOS emulators still use PCX 
previews as well!  Argghhh!  Although it's not a huge hassle to convert 
all the PNG's to PCX files for previewing, it would be nice to natively 
support PNG graphics files as well.  

- I don't have a whole lot of time to spend on it anymore, but I would 
appreciate any ASM code (or BASIC code that I can convert to ASM 
myself) that decodes PNG files.  I realize they are much smaller in 
size, are LZW compressed, and cover more color depth than GIF's.  I 
just wish I knew it was coming.  What a drag!

New features included in this release:

- Getting too many ROMS!  Had to re-optimize loading and resorting 
routines.  Load now takes less than 1 second for 750 entries.  Resort 
now takes about 5 seconds for 750 entries.  (Times derived from an 
Intel Pentium 200MHz non-MMX CPU PC)

-----------------------------------------------------------------------

May 22, 1999

- Updated to 4.40b

Bug Fixes From v4.20b:

- Mouse emulation & VESA bank conflicts eliminated - FOR REAL THIS 
TIME.  VESA Read/Write window corruption has been tested on 6 different 
manufacturer's video cards with total success this time rather than 
just with ATI cards.  Emulated mouse cursor now works properly without 
corrupting the dialog window's background - FOR REAL AS WELL.

- Edit bug that would return to the Control Panel after changing a game 
description and would not refresh the list.  Fixed now, should work the 
same as in every other version so far.

New features included in this release:

- Point and click definitions for window positions and sizes.  This one 
really bugged me for a while now.  I hated punching in coordinates 
blindly in a "Hit & Miss" fashion.  Not very sophisticated.  Works very 
well now.  Use the "Set." buttons under "Custom" settings.

- Here's a good one --- A "Quit" button so you can exit the front-end 
with the click of a mouse button rather than having to press the ESC 
key to bail.  Of course, ESC still works as well for backward 
compatibility.

- Last one:  Switched Control Panel access from the left mouse button 
to the right since I'm thinking I'm gonna do something with the left 
button in the future here.  Of course, the TAB key still accesses the 
Control Panel as well for downward compatibility.

-----------------------------------------------------------------------

April 13, 1999

- Updated to 4.20b

New features included in this release:

- Preview "fade in" enable/disable - Allows instant display of PCX 
preview screen.

- Preview "delay" enable/disable - Shows all PCX previews while 
scrolling through the menu.  If you experience performance loss with 
this option then disable it.  If the keyboard buffer is "filling up" 
too quickly then choose "Force Keystroke Break" from the "System 
Options" dialog window.

- Font text shadow for better contrast against background.  If you are 
using a Pentium 133 or less and suffer from performance degradation 
using this option then disable it from the control panel.

- Database record counter enable/disable.  This option is used for 
those who don't want statistical clutter on the screen.  To disable the 
default screen caption, "Dread's QuickMAME Launcher" just use a blank 
entry in the "System Options" menu.

-----------------------------------------------------------------------

April 10, 1999

- Updated to 4.12b

Bug Fixes From v4.11b:

- Mouse emulation & VESA bank conflicts eliminated.  Emulated mouse 
cursor now works properly without corrupting the dialog window's 
background.

- The Control Panel layout order is more logical than it was, 
previously.

New features included in this release:

- Text cursor & mouse cursors both "glow" now.

-----------------------------------------------------------------------

April 9, 1999

- Updated to 4.11b

New features included in this release:

- Mouse cursor emulation support for Windows & DOS.  Still requires a 
valid DOS or Windows mouse driver.  I finally figured out that the 
"VESA change bank" call requires the value "1" in the BL register for 
the read page.  I had always had it set for "0" instead (which is write 
only on some video cards) because no documentation I've ever read on 
VESA calls makes mention of this except for the fact that it "must be 
zero."  I just took a "shot in the dark" and it panned out.  Go nuts.

-----------------------------------------------------------------------

April 8, 1999

- Updated to 4.10b

Code still needed:

- Forcing a VESA mouse pointer manually under Windows 9x.  I can't seem 
to read the screen graphics in any VESA bank above 0 even after 
switching with ATI, STB, and a handful of other video cards.  It  
destroys the background if the pointer is in VESA banks higher than 0.  
HELP!  If you feel you really need a mouse pointer then run in pure DOS 
mode with a VESA compliant DOS mouse driver.

Bug Fixes From v4.00b:

- Screen doesn't flicker anymore when palette fades occur.  Thanks to 
Darren H. for the "Wait for Vertical Refresh" code.  Muchly 
appreciated.

- Crashing & illegal operations under Win9x on some PC's although it 
works fine under pure DOS.  This should now be fixed.  I've "alpha" 
tested it on a few machines that were previously problematic with 
success.  If anyone still has problems, please e-mail me.

- Removed "keystroke speed and delay" options from the "System Options" 
dialog box.  The system would keep these values after exiting the 
program.  There is no way to read the original values so I "ex-ed" it 
because it was annoying.

- Automatic joystick/gamepad enumeration on load.  This means that you 
do not have to specify whether a joystick is connected and/or how many 
are connected.

New features included in this release:

- Native joystick/gamepad menu support.  (See "Joystick Support".)

- Menu keystroke ignore has been added.  This feature is useful if you 
want to use a joystick or gamepad to launch and scroll through the menu 
and you are also using JOYEMU.  This disables "double key presses" when 
JOYEMU is running but allows the user to still press "ESC", "TAB", or 
click a mouse button to quit or to access the control panel.  Joystick 
scrolling is much smoother than the keyboard.

-----------------------------------------------------------------------

February 16, 1999

- Updated to v4.00b

New features included in this release:  (This is lots!!!)

- Completely rewritten GUI (graphical user interface).

- GUI Includes:  640x480 256-Color GUI, 23 built-in fonts and custom 
font ability, background WAV sound (built-in or custom), PCX preview 
ability for every game, and a customizable background.

- Much faster ROM checking, loading, and resorting engine.

- Completely downwardly compatible with QuickMAME 3.xx

- See the "QM Explained" section for more details.

-----------------------------------------------------------------------

January 02, 1999

- Updated to v3.71

Bug Fixes From v3.70:

- Keyboard interrupt problems when launching under Windows 95/98 on 
first run.

- Glitch in edit window with categorization filter enabled.  The item 
would not be displayed on the main menu after changes.

New Features included in this release:

- New "Sports" category to find only sports-related titles.

- Can now disable automatic sorting after editing a game description.  
Handy when you're renaming quite a few ROM names at once.  This way you 
don't have to wait every time while the database is re-sorted, you can 
just simply choose "Re-sort Database" under the "System Options" dialog 
window.

-----------------------------------------------------------------------

November 11, 1998

- Updated to v3.70.

Bug Fixes From v3.70:

- "QuickList" filtering problem


Bug Fixes From v3.61:

- Program couldn't find the QMREADME.TXT help file if the "A - ARCHIVE" 
attribute was set to false.  This is now corrected.

New Features included in this release:

- More database fields added to allow a "Quick List" of all entries, 2 
Player VS entries, and My Favorites entries on the main window.

- Optional resorting dialog window added.  If the program detects new 
entries it will now prompt to either resort now or later upon startup.  
You can always resort manually later by choosing the option from the 
System dialog window.

- Faster resorting engine.  Still using the same A-Z low order search 
method, but now it copies the entries to another temporary database 
while it sorts.  Much quicker now.

- Custom main window title.  You can name it whatever you want now, 
instead of the default "Dread's QuickMAME Launcher 3.xx".  A good 
choice is the name of the emulator within that directory.

-----------------------------------------------------------------------

November 08, 1998

- Updated to v3.61.

Bug Fixes From v3.60:

- Eliminated unnecessary database resorting and loading procedures 
because they were running every time whether or not they needed to due 
to modifications made to the database.  Now it only runs these when 
necessary to do so.  Speeds it up quite a bit if you're editing a lot 
of entries.

- A bug that caused garbage entries in the main window scroll box 
when>~500 entries were found.  Now supports ~1000 entries.  I did try 
another method that actually uses the disk instead of memory to hold 
the values for the scroll box since it had support for an infinite 
number of entries, but it degraded the speed so I gave up huge listings 
for speed.  Besides, is anyone really gonna have more than 1000 ROMS?  
Maybe one day, I guess, but about 1/3 are all cloned ROM's for MAME 
anyway.

New Features included in this release:

- Idiot-proof Installation program added in archive to make life much 
easier.

- Faster database "loading / new ROM comparison" procedure.  It's now 
about 3-4 times faster loading than before.

- More database fields added.  Now allows the following switches to be 
defined for MAME:

  -RES
  -DOUBLE / -NODOUBLE
  -FRAMERATE
  -SR
  -SB

-----------------------------------------------------------------------

November 05, 1998

- Updated to v3.60.

Bugs Fixed from v3.51:

- Some anti-virus programs like Dr. Solomon's and AVP were reporting a 
"possible MUST DIE Trojan" in QM.COM.  These virus scanners were 
finding a string labeled "COMEXE" in the program and therefore 
misreporting the situation.  Of course, this string was used in the 
code to indicate an executable file "search pattern."  Nevertheless, 
some people were on edge over this, so after receiving a few complaints 
the program has been recompiled so it no longer gets misreported by 
these AV programs.  My apologies for the virus scare.

- Database description truncation problem fixed when using ROM file 
extensions with less than 3 characters for a file extension.  Thanks to 
"Peter M." for finding this after trying Virtual GameBoy ROM 
extensions.  (*.GB file types.)

- Better error trapping handler added.

New Features included in this release:

- Automatic database upgrade to add some new expansion fields/options.

- A new "Force Resolution" option for individual entries with the click 
of a mouse.  (Or via keyboard, of course.)  Includes a custom 
resolution field, as well.

- Reset to default option for settings.

- Delete database option to reinitialize entries.

- Re-sort database on demand option.

- Pause before returning to program option.

-----------------------------------------------------------------------

November 02, 1998

- Added more examples for using QM with other emulators.

-----------------------------------------------------------------------

October 20, 1998

- Changed the sort engine from "swap" to straight A-Z linear sorting.  
Had problems when more than ~150 files needed to be sorted.  Very 
sloooooow, previously.  Now it's quite zippy, and I can now predict a 
"percentage complete" ratio for animation.

- The "Pacman" loading & resorting windows now have a little more text 
animation with a ghost-monster running around too.

- Fixed a bug regarding resorting.  It opened the database twice 
without closing the first instance.  Caused blank entries in the 
database that made it loop endlessly, or at least until an error 
occurred after running out of memory, etc.

- Button color & screen row custom configuration added.

- Longer executable statement added to allow "prefix" switches instead 
of just "suffix" switches with the "Universal Switches" field.  (e.g. 
RETRO -G)

-----------------------------------------------------------------------

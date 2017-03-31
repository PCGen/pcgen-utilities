-- To Use Prettylst --

Hi, this is a basic text help read me file [your quickstart guide for a general setup and to get you using the program as intended]. For the advanced instructions please refer to the 'prettylst.pl.html' file. That has a basic install guide, the perl commands used for PCGen and an internal changelog.



WINDOWS INSTRUCTIONS:

You must have Perl on your machine or you will need to install it.

I recommend Active State Perl which can be found:

  http://www.activestate.com/store/activeperl/

After Installation you will need to load the Perl Package Manager (PPM) either in the start menu or using the RUN command.
  You will need to install the "Readonly" module.
  Type in the Search Bar 'READONLY' and then mark it for install... After that is installed you're set to go.


--- BAT File Help ---

Helpful Notes for PL - using a Bat File:
NOTE: This will assume default 'pl' folder is root of C:\

Make two folders within the 'pl' folder called 'test' and 'checked'

Place the pcc and lst files you wish to check in your test folder and then run your bat file.

Here is a sample Bat file:

#
perl prettylst.pl -i=c:\pl\test -o=c:\pl\checked -x -nw -e=error.txt
#

This will run prettylst on the file(s) and folder(s) placed in C:\pl\test, then place any corrected files in the 'checked' folder and give you a txt file called "error.txt" with what the program found -lots of false positives so be careful.

NOTE: For a complete list of commands refer to the prettylst.pl.html file.

###
Here is a modified form - USE AT OWN RISK

#
perl prettylst.pl -i=d:\pcgen\pcgen_dev\Trunk\pcgen\data -o=c:\pl\checked -x -nw -e=error.txt
#

This would run prettylst on the entire data folder in the trunk... Don't use unless you know what you are doing and have a lot of memory to spare.
This is just an example of how you can customise your bat file. NOTE:You would actually have to setup a folder in a D:\ for this to work.

Additional useful command line switches:
  -c=pcgen5120	will convert many older tags to PCGen version 5.12.0
  -wl=notice	will display only the more serious error messages.


Good Luck and Happy coding.

If you need further assistance, please ask on the PCGen Y! group [http://games.groups.yahoo.com/group/pcgen/] with [PL] in the subject line. Thanks.

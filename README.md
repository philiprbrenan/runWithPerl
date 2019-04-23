# runWithPerl
## Run with Perl - a simple development environment for Xml and Perl using Geany.

Integrated development environment for the Geany editor at:

  https://www.geany.org/Download/Releases

To compile or run Bash, C, Perl, Javascript programs or validate Xml without
leaving the editor, enter the following on lines 1-2 of the dialog box reached
by selecting the Geany menu actions:

 "Build"=>"Set Build Commands"

Commands to enter into the dialog box:

  runWithPerl "%f"
  runWithPerl --run "%f"

Place this script in your:

  ./local/bin/

folder and run it once with no arguments to make itself executable:

  perl ./local/bin/runWithPerl

There-after pushing the right key in Geany or using the "Build" menu will cause
the code you are editing to be compiled or run.

To validate Xml you will need to have xmllint installed:

  sudo apt-get install libxml2-utils

To validate with Dita OT update the value of sub xmlCatalog below with a
catalog from:

  https://www.dita-ot.org/


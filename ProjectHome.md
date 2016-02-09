This project hosts and supports additional plugins for SAPlink.
Check the main project [SAPlink](http://code.google.com/p/saplink/) for more details.

Current Plugins within this repository include

**[Transactions](http://code.google.com/p/saplink-plugins-ksq/downloads/list)**

**[Report Variants](http://code.google.com/p/saplink-plugins-ksq/downloads/list)**

Following guidelines need to be followed if you would like to export variants using this Plug in along with the current releases of the ZSAPLINK main program.
  * For exporting a slinkee (Slinkee Tab of the selection screen)
    1. Increase the length of the Object from 40 to 120 in the selection screen
    1. The object type is 'VARI' which ZSAPLink automatically detects and the object name is a concatenation of Program name and Variant name preserving the spaces.(RESPECTING BLANKS addtion for CONCATENATE statement)
  * For exporting variants in a transport (Nugget Tab of the selection screen)
    1. You need to modify the Select query from E071 to include additonal where clause as 'OR PGMID = 'LIMU''
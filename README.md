# ripdisc
The ripdisc bash script creates a backup of a DVD in .iso format.

# Author:
Geno Nullfree

# Description:
This script will rip a 1:1 backup iso of a dvd video. It will first try to use the dvdbackup utility, and if that fails (some discs do, some discs dont, I believe this is encryption related) it will attempt to do a dd on the disc.

# Dependencies: 
dvdbackup dvd+rw-tools lsdvd libdvdcss pgrep



# Usage:
ripdisc [options]

-n "title"        Specify output .iso filename (Use quotation marks or escape spaces)
 
-t /path/to/tmpdir    Temp directory (Leave off trailing /)
 
-o /path/to/outdir    Output directory (Leave off trailing /)

-d <dvd device name>  DVD drive name (Only put sr#, not /dev/sr#. Replace # with drive number.)

If you have multiple disc drives and you wish to use multiple at the same time, change /dev/sr0 to which dvd drive it is (i.e. 0, 1, 2, etc.)
 
# Lessons Learned:
How to use a case/switch statement
How to check a DVD's title
How to check a DVD's size
How to overwrite an echo line
How to monitor a child pid
How to catch a ctrl-c hit
How to shift the command line arguments

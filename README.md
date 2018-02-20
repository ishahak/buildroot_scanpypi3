# buildroot_scanpypi

This is a porting of buildroot's scanpypi for Python 3, so that Python3 packages from PyPI can be easily installed into a buildroot file system.

see discussion here:
https://stackoverflow.com/questions/48867457/adding-python3-packages-to-buildroot

**Usage:**
1. Copy scanpypi3 into &lt;buildroot&gt;/support/scripts
2. Use it to install packages
  
**Example:**
* ./support/scripts/scanpypi3 websocket-server -o package

For licensing issues please refer directly to https://buildroot.org

**Important Note:** 

Although I didn't see anything about it in the docs, it seems that in order to have the new package appear in the menu for external Python packages (Target packages -> interpreter languages -> External Python modules), the file package/Config.in should be added with an appropriate line. A rumor for this is appearing here: http://www.armadeus.org/wiki/index.php?title=Buildroot_Packages

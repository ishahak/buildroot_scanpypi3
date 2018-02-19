# buildroot_scanpypi

This is a porting of buildroot's scanpypi for Python 3, so that Python3 packages from PyPI can be easily installed into a buildroot file system.

Usage:
1. Copy scanpypi3 into &lt;buildroot&gt;/support/scripts
2. Use it to install packages
  
Example:
* ./support/scripts/scanpypi3 websocket-server -o package

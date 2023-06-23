ACS TOOL Rebuild

Given that the original u-boot repository is quite old, it still uses python2 tools.
This script is meant to patch a failure during the compilation

Instructions:

Makefile.fip.mk:33

Substitute this line:
python2 $(CURDIR)/fip/acs_tool.pyc

for:
python $(CURDIR)/fip/acs_tool.py 


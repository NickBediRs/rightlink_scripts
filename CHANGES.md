Changelog for the RightLink10 Base ServerTemplate
=================================================

10.1.2
------
- Make collectd.sh throw errors on broken configs.

10.1.rc1
--------
- Changes to use RightScale TSS for monitoring:
  - Modified collectd config to use write_http plugin to route monitoring traffic through RightLink.
  - Removed usage of forward ported collectd 4 and RightScale Software repo.
  - Renamed setup_software_repo.sh to security_updates.sh.
- Fixed syntax errors in wait-for-eip.sh

10.1.rc0
--------
- Modified wait-for-eip.sh to reflect variable name changes
- Update scripts to use sudo as RightLink now runs as the rightlink user and not as root

10.0.rc4
--------
- Fixing of rs_push script to find the right audit entry again (html parsing breakage)
- Adding test-script back into rll cookbook to support the rightlinklite regression tests

10.0.3
------
- Reorg of rll cookbook scripts to break out the init script into multiple pieces
- Addition of automatic upgrades

10.0.rc0 .. 10.0.rc2
--------------------
- Dark ages... First version of the rll "cookbook" and the rs_push/rs_make_st scripts

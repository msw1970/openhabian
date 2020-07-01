This is the new announcement page that will pop up whenever you start
`openhabian-config` and the developers have significant news they would like to
share with you.

Hit tab to unselect the buttons and scroll through the text using UP/DOWN or
PGUP/PGDN.

All announcements will be stored in /opt/openhabian/docs/NEWSLOG.md for you to
lookup.

## June 17, 2020

### Removed support for PINE A64(+) and older Linux distributions
`openhabian-config` will now issue a warning if you start on unsupported
hardware or OS releases. See [README](README.md) for supported HW and OS.

In short, PINE A64 is no longer supported and OS releases other than the current
`stable` and the previous one are deprecated. Running on any of those may still
work or not.

The current and previous Debian / Raspberry Pi OS (previously called Raspbian)
releases are 10 ("buster") and 9 ("stretch"). Most current Ubuntu LTS releases
are 20.04 ("focal") and 18.04 ("bionic").

## June 10, 2020

### New parameters in `openhabian.conf`
See `/etc/openhabian.conf` for a number of new parameters such as the useful
`debugmode`, a fake hardware mode, the option to disable ipv6 and the ability to
update from a custom repository other than the `master` and `stable` branches.

In case you are not aware, there is a Debug Guide in the `docs/` directory.

### New Java options
Preparing for openHAB 3, new options for the JDK that runs openHAB are now
available:

-   Java Zulu 8 32-Bit OpenJDK (default on ARM based platforms)
-   Java Zulu 8 64-Bit OpenJDK (default on x86 based platforms)
-   Java Zulu 11 32-Bit OpenJDK
-   Java Zulu 11 64-Bit OpenJDK
-   AdoptOpenJDK 11 OpenJDK (potential replacement for Zulu)

openHAB 3 will be Java 11 only.  2.5.X is supposed to work on both, Java 8 and
Java 11. Running the current openHAB 2.X on Java 11 however has not been tested
on a wide scale. Please be aware that there is a small number of known issues in
this: v1 bindings may or may not work.

Please participate in beta testing to help create a smooth transition user
experience for all of us.

See [announcement thread](https://community.openhab.org/t/Java-testdrive/99827)
on the community forum.
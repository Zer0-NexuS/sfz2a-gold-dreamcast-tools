STREET FIGHTER ZERO 2 ALPHA — DREAMCAST DISC BUILDER
v1.4.3 RC P3

WHAT YOU NEED
- Windows 10 or 11 (64-bit), with at least 1 GB of free space.
- The matching modified sfz2ald.zip ROM for this release.
  The ROM is not included. Retail ROMs and older revisions will not work.

No separate Python installation, SDK or internet connection is needed
on Windows. Keep all included kit files together.

BUILD YOUR DISC IMAGE
1. Extract the entire injection kit ZIP into a normal folder.
   Do not run the builder from inside the ZIP.
2. Leave your ROM ZIP zipped. Do not extract it.
3. Drag your matching ROM ZIP onto BUILD_CDI.bat.
4. Wait until the window says SUCCESS. Do not close it while building.
5. Open the output folder. Your finished disc image is:
   SFZ2_Alpha_DC_v1.4.3_RC_Projectiles.cdi

Cold-boot this CDI in Flycast, or use your usual compatible Dreamcast
disc-burning setup. Avoid loading an old emulator save state when testing
the new image.

IF SOMETHING GOES WRONG
- ROM mismatch: you need the correct modified ROM revision. Renaming
  a different ROM ZIP will not fix it. Repacked ZIPs with matching ROM
  contents are accepted.
- A usage message appears: drag the ROM ZIP onto BUILD_CDI.bat instead
  of opening the BAT file by itself.
- Missing files or runtime: extract the entire kit again and keep its
  folders intact.
- An unrelated file already exists in output: move or rename that file,
  then try again. The builder protects it from being overwritten.
- For other errors, check the logs folder.

Your original ROM ZIP is left unchanged. The finished CDI is checked
against the release image before the builder reports success.

MAC / LINUX
Install Python 3.11 or later, then run from the extracted kit folder:
  bash BUILD_CDI.sh /path/to/sfz2ald.zip

See TESTING.txt in the kit for validation details.

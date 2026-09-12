# Tool Pocket Generator V62

V62 is based directly on the immediately preceding V61 build. This build applies the agreed V62 fixes after whole-workflow review:
- Remove Photo now clears the displayed photo canvas as well as the photo state; profile geometry is not altered.
- Export Profile JSON is downloaded using the V60-compatible application/octet-stream handling so iPad/iOS does not treat the JSON as an STL-viewer file. The JSON contents remain profile data and the STL download mechanism is retained.
- STL export restores the proven V60 pocket-cutter geometry architecture while preserving V61 functionality: the main cutter occupies Z=(tray thickness-pocket depth) through Z=tray thickness, and enabled finger reliefs use their actual crescent/semicircular modified profiles as part of the cutter geometry.
- V61's corrected finger-relief depth rule is retained: relief depth must be positive and no greater than tray thickness; it is not incorrectly limited by main pocket depth.
- The V61 physical-grid rectangle preservation/re-centering workflow and other working features are retained.

The exported STL is intentionally a solid positive pocket-cut volume. It is not a finished hollow tray by itself; it is intended for the established tray/base workflow in Bambu Studio.

Version labels, manifest cache and exported filenames are V62.

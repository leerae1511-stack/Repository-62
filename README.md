# Tool Pocket Generator V61

V61 is based directly on the immediately preceding V60 build. This build makes only the agreed, isolated changes:
- Saved Tools Section 2 is simplified: Load is retained and the normal Delete control is removed. Save tool creates a new record or updates the currently loaded record.
- The initial Length × Width entries and Detect tool outline workflow are unchanged.
- Set dimensions from physical grid now preserves the edited outline at its existing physical size and re-centres it in the newly measured reference rectangle; it does not scale, distort or delete profile points. Finger-relief locations are carried with the physical profile.
- Finger-relief depth is checked against tray thickness rather than incorrectly requiring it to be shallower than the main pocket.
- STL export now generates the positive pocket-cut volume used in the tray workflow. The main cleared profile is the cutter and each enabled finger relief is a stepped deeper extension of that cutter. No new wall-thickness parameter or tray-envelope assumption was introduced.
- Export Profile JSON remains a JSON download and is labelled as V61; the STL download mechanism itself is retained.
- Version labels, manifest cache and exported filenames are V61.

The existing profile detection, point editing, segment curve controls, grid workflow, saved profile data structure and other unrelated functions were not intentionally changed.

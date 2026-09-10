DIVE BUDDY ALERT BAND — PRESENTATION & CAD REV F
Concept by Rafael | September 2026

START HERE
Open DBA_Interactive.html, or visit:
https://buddhacoder.github.io/dive-buddy-alert-band/
This is the primary presentation, with working 3D, simulated screen views,
current dimensions and download links. The side depth meter is a scroll effect.

CURRENT FILES
DBA_Design_Package_RevF.pdf        18-page concept and engineering brief
DBA_Product_Overview_RevF.pptx     12 editable slides with presenter notes
DBA_Annotated_Views_RevF.pdf       Five current drawing / fit views
DBA_Package_RevF.zip              Complete current release with legacy references
slides.html                      Optional online slide / drawing viewer
presentation.html                Redirect to the main interactive presentation
cad/                             Regular STEP/STL assembly and 18 parts
cad/fit-variants/compact/         Compact CAD, drawings and design manifest
cad/fit-variants/cuff/            Cuff CAD, drawings and design manifest
drawings/                        Coordinated DBA-001 PDF/PNG, SVG line art
renders/                         Current render and screen images
design-data.json                 Regular source parameters and envelopes

FINISH AND SOUND REFINEMENT — 10 SEPTEMBER 2026
Corrosion resistance is a design requirement. Proposed exterior: silicone
strap, keeper and button, molded acetal buckle with nonmetal retention, and
polymer housing and window. No exposed steel pin or charging contacts are
specified. Material grades, latch strength, seal durability and long-term
saltwater performance remain unvalidated. All 54 part STL files retain the
same geometry; finish metadata, renders and linked documents are refreshed.

Underwater sound is optional and starts muted. The sound toggle enables an
original procedural water-and-bubble soundscape; settings include volume.
Scrolling deeper gently muffles the ambience. Hiding the page pauses sound;
resuming requires a click. This is presentation sound design, not a recording
of an actual dive or a reproduction of DBA device signals.

WHAT CHANGED
Four screen views: Buddy (bearing and relative depth), Map (both divers),
Dive (time/depth/motion) and Boat (horizontal reference distance/bearing).
Rev F proposes a separate boat-associated acoustic positioning reference,
plus pressure and heading sensing in each band. A single wrist transducer
alone still gives range, not direction. The external reference has a system
architecture illustration, not fabricated detailed hardware CAD.

The module is 54 x 38 x 19.5 mm, plus 2.2 mm button protrusion. Display active
area is 24 x 24 mm. The 18-part model has an adjustable overlapping silicone
tail, ten adjustment holes, a buckle envelope and a keeper. Compact, Regular
and Cuff reference diameters are 50, 62 and 78 mm (about 157, 195 and 245 mm
circular reference circumference). These are nominal layouts, not established
wearer ranges. Buckle engagement and actual retention remain undefined.

INTERACTION
The demo starts with two paired bands. Short presses would cycle views;
a one-second hold would call. The peer short-presses to acknowledge.
Web tabs and call buttons simulate those actions directly. Device receipt
and human response are distinct. Settings expose missing peer/reference
links and stale updates. Missing fixes remove arrows and map points.
Speeds are relative to the reference, not speed through water. Vertical
rate is separate from horizontal speed and is not decompression protection.

BOUNDARIES
All screen positions, headings, depth, time, rates and battery values are
simulated. Navigation requires additional sensing and reference equipment.
20 m direct range is a target. No navigation accuracy, operating depth,
runtime, supported wrist range or manufacturing readiness is established.
An aid to buddy procedures, never a safety or reunion guarantee. Not a
replacement for a dive computer; no ascent-limit or decompression model.
Inductive charging through the sealed cap; no band charging port. The module
remains removable from the strap and the physical button remains on top.
Original Rev A costs are historical desk estimates, ±30%; they do not price
Rev F navigation hardware or the acoustic reference. No procurement or
physical hardware test program is part of this presentation project.

REGENERATION
Geometry authority: dba_cad.py named parameters. Install CadQuery in Python.
Run dba_cad.py for Regular, then with --size compact and --size cuff.
Then run render.py and drawing_sheet.py. Run presentation/build_fit.py,
presentation/embed_mesh.py and presentation/build.py to update diagrams,
all three base64 int16 mesh sets and the interactive site. Screen screenshots
and fit illustration PNG derive from the actual browser via capture_assets.cjs.
Run presentation/pdf.py and presentation/deck-build/build.mjs for documents.
Then build_hub.py, build.py and package_release.py in presentation/.
Render scripts use VTK, NumPy, numpy-stl and Matplotlib. Documents use
ReportLab/svglib. Slides use the supplied artifact-tool presentation runtime.
Never hand-edit STEP or STL files. Regenerate all dependent artifacts.

VERSION AUTHORITY
Current presentation, drawings and CAD are Rev F. Earlier PDFs and the
original Rev A package in legacy/ are historical references. Published diver
reviews and technical references are documented in the Rev F brief; they are
not interviews or validation of DBA hardware.

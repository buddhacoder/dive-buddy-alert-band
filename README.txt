DIVE BUDDY ALERT BAND — PRESENTATION REV G / CAD REV F
Concept by Rafael | September 2026
Prepared for Rafael
Presentation strategy, design & production by The AI Doc

START HERE
Open DBA_Interactive.html, or visit:
https://buddhacoder.github.io/dive-buddy-alert-band/
This is the primary presentation, with working 3D, simulated screen views,
current dimensions and download links. The side depth meter is a scroll effect.

MOBILE PRESENTATION — 10 SEPTEMBER 2026
The phone opening puts the rotatable band directly beneath the product name.
Model controls sit below the model, with touch-sized buttons and selectors.
Menu opens section links; sound and depth controls use a reserved side margin.
Swipe sideways on the band to rotate; swipe vertically to scroll the page.
Download labels use plain language. Product specifications and the current
PDF, slides, drawings, geometry and recorded audio are unchanged.

CURRENT FILES
DBA_Partner_Brief_RevG.pdf         One-page development-partner brief
DBA_Design_Package_RevG.pdf        25-page concept and engineering brief
DBA_Product_Overview_RevG.pptx     14 editable slides with presenter notes
DBA_Annotated_Views_RevF.pdf       Five current drawing / fit views
DBA_Package_RevG.zip              Complete current release with legacy references
slides.html                      Optional online slide / drawing viewer
presentation.html                Redirect to the main interactive presentation
cad/                             Regular STEP/STL assembly and 18 parts
cad/fit-variants/compact/         Compact CAD, drawings and design manifest
cad/fit-variants/cuff/            Cuff CAD, drawings and design manifest
drawings/                        Coordinated DBA-001 PDF/PNG, SVG line art
renders/                         Current render and screen images
design-data.json                 Regular source parameters and envelopes

PRODUCT-DEVELOPMENT BRIEF — 10 SEPTEMBER 2026
The opening now introduces the complete system and the proposed first market:
operator-managed recreational boat dives. Operator and diver responsibilities,
reference-dependent capabilities and first-product priorities are explicit.
The full four-view demo remains available. Proposed priorities do not remove
features from the concept or claim that the system has been validated.

presentation/partner-brief.json is the shared source for customer, workflow,
capabilities, priorities, alternatives/evidence, feasibility decision criteria,
commercial inputs and the partner request. Rev G adds a one-page partner brief
and revises the 25-page engineering brief and 14-slide meeting presentation.
Slides 1–10 are the meeting narrative; slides 11–14 provide supporting detail.
Current price, margin, volume, development budget and launch date remain open.
The request is for feasibility and a scoped proposal, not a hardware program.
No company endorsement, interviews, purchase intent or performance is invented.
CAD, annotated Rev F views, physical-product renders and scuba audio remain
unchanged. Four screen captures now exclude the website sound/depth controls.

FINISH AND SOUND REFINEMENT — 10 SEPTEMBER 2026
Corrosion resistance is a design requirement. Proposed exterior: silicone
strap, keeper and button, molded acetal buckle with nonmetal retention, and
polymer housing and window. No exposed steel pin or charging contacts are
specified. Material grades, latch strength, seal durability and long-term
saltwater performance remain unvalidated. All 54 part STL files retain the
same geometry; finish metadata, renders and linked documents are refreshed.

Scuba ambience now uses a real underwater recording: Scuba_bubbles.mp3 by
sbvitug (Freesound, CC0). See audio/CREDITS.txt for source and editing notes.
Sound attempts to autoplay on arrival. If browser policy blocks it, an ordinary
tap, click or key press starts playback. Mute and volume choices are saved.
Sound pauses while hidden and resumes when visible if enabled and allowed.
Mild filtering follows scroll depth while retaining the bubbles. The recording
is embedded in the single HTML file and included in audio/ for regeneration.
This is presentation ambience, not the proposed device's acoustic signals.

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
To rebuild audio/scuba-loop.mp3, run presentation/prepare_audio.py (FFmpeg +
NumPy); presentation/build.py embeds the result into the standalone page.
Then build_hub.py, build.py and package_release.py in presentation/.
Render scripts use VTK, NumPy, numpy-stl and Matplotlib. Documents use
ReportLab/svglib. Slides use the supplied artifact-tool presentation runtime.
Never hand-edit STEP or STL files. Regenerate all dependent artifacts.

VERSION AUTHORITY
Current presentation is Rev G; drawings and CAD remain Rev F. Earlier PDFs and the
original Rev A package in legacy/ are historical references. Published diver
reviews and technical references are documented in the Rev G brief; they are
not interviews or validation of DBA hardware.

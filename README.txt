DIVE BUDDY ALERT BAND - PRESENTATION REV C - SEPTEMBER 2026
Concept by Rafael.

START HERE
DBA_Interactive.html            Interactive display/haptic concept and original CAD viewer
DBA_Product_Overview_RevC.pptx   Editable nine-slide product overview with presenter notes
DBA_Design_Package_RevC.pdf      Revised concept and engineering brief
DBA_Annotated_Views_RevB.pdf     Original geometry: annotated nominal drawing views

REV C DISPLAY CONCEPT
The proposed interface combines tactile alerts with a simple visual display.
It distinguishes a call being received by the device from a diver acknowledging it.
Fresh estimated distance is shown on both bands during ranging; the caller can use
optional distance cadence. Unavailable or stale measurements clear both distance
and trend. Pairing, battery, low battery and stop states are demonstrated.
Enlarged screen views and the 3D cap material are appearance/interface studies.
They do not establish physical screen size, readability, seal or mechanical fit.

MECHANICAL BASELINE
The original eleven-part CAD, meshes, renders and parametric source are unchanged.
They do not include the new display/window/electronics. Display integration requires
reconciling the existing coil/cap interference, button access and internal clearances.
The 38 x 28 x 11.5 mm housing is the original nominal envelope, not a validated
housing specification for the display variant. The annotated Rev B views describe
that same original geometry. The original DBA-001 drawing has unresolved discrepancies.

PERFORMANCE AND COST
20 m range remains a target. One wrist transducer and approximately 65 kHz two-way
time-of-flight provide distance, not bearing. There is no relative-heading or
depth-difference capability. A directional buddy-finding feature needs a separately
defined sensing/estimation architecture; a new screen alone does not supply it.
This is an aid to buddy procedures, never a safety guarantee or promise of reunion.
The original +/-30% desk costs and retail target cover the display-free baseline.
Display-variant cost, power, mass and runtime have not been estimated or established.
This remains a presentation package, not a hardware development or sourcing program.

CONTENTS
cad/, drawings/, renders/       Original reference STEP/STL/DXF/drawings/renders
presentation/                   Editable page, style, interaction and document sources
legacy/                         Original README; archive also includes Rev A and B PDFs
 dba_cad.py                     Original parametric CadQuery authority
 render.py / drawing_sheet.py  Original render and drawing generators

REBUILD
python presentation/build.py
PDF: python presentation/pdf.py (reportlab, svglib, Pillow; output/pdf/)
Copy the resulting Rev C brief beside the HTML.
PowerPoint: presentation/deck-build/build.mjs uses @oai/artifact-tool and the Codex
presentation runtime/finalizer. Paths and output receipt are local authoring settings.
The finished PPTX is editable independently of the authoring runtime.
python presentation/package_release.py (requires final PDF/PPTX beside HTML)
Serve this folder for download links. Three.js uses its existing public CDN.

GEOMETRY CHANGES
Edit dba_cad.py parameters, regenerate CAD, rerun render.py and drawing_sheet.py,
and re-embed meshes in the existing base64 int16 format. Never hand-edit STEP/STL.
The original scripts target /home/claude/out; adapt output paths before regeneration.

LIVE SITE
https://buddhacoder.github.io/dive-buddy-alert-band/

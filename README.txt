DIVE BUDDY ALERT BAND — PRESENTATION REV E / CAD REV D
Concept by Rafael.

SHARE THE FULL INTERACTIVE PRESENTATION
https://buddhacoder.github.io/dive-buddy-alert-band/

This is the primary presentation: the product story, two-diver demonstration,
rotatable 3D model, band flexibility illustration, fit notes, specifications and
downloads. The earlier presentation.html link now opens the same full experience.
The optional online slide viewer is at slides.html.

OPEN LOCALLY
DBA_Interactive.html              Full interactive presentation
DBA_Design_Package_RevE.pdf        Product story and engineering brief
DBA_Product_Overview_RevE.pptx     Editable presentation with presenter notes
DBA_Annotated_Views_RevD.pdf       Dimensioned views of the current CAD
slides.html                      Optional slide and drawing viewer

WEARABILITY
The silicone band is intended to stretch for hand passage and sit around a wrist
or suit cuff. Its circular CAD shape is relaxed. The electronics module is rigid
and removable. The current model is one reference size: 62 mm relaxed opening,
approximately 195 mm inner circumference, 24 mm band width and 4 mm radial wall.
No wrist/cuff size coverage, silicone grade, hardness, stretch force, recovery or
maximum extension has been established. The 3D flex and diagrams are illustrations,
not material simulations, size recommendations or rated extension.

GEOMETRY AND SCOPE
Presentation Rev E preserves the 14-part Rev D CAD and its encoded base meshes.
Housing: 44 x 32 x 17.5 mm, plus 2.2 mm button protrusion.
Overall assembly: 70 x 37 x 90.7 mm.
Display body: 16 x 18 x 2.5 mm. Window: 18 x 20 x 1.2 mm.
Active display area: 14 x 16 mm.
The hero flex view deforms only its displayed silicone mesh and returns exactly
to the relaxed source. Dimensioned views and exported CAD remain at rest.

One top button, a removable sealed module and inductive charging through the cap
remain deliberate choices. One approximately 65 kHz acoustic transducer provides
distance, not buddy bearing or relative orientation. 20 m is a range target.
The concept is an aid to buddy procedures, never a safety guarantee.
Rev A costs (+/-30%) and retail figures are historical display-free estimates.
Current display-variant cost, mass, runtime and real underwater performance remain
unestablished. The illustrative dive scenario is not a claimed founder experience
or customer testimonial. These files are not a manufacturing release.

REBUILD
Geometry changes begin in dba_cad.py, followed by render.py, drawing_sheet.py,
presentation/embed_mesh.py and presentation/drawings.py. Never hand-edit STEP/STL.
For presentation changes, maintain presentation/story.json and requirements.json.
Run presentation/build_fit.py, presentation/build.py, and presentation/pdf.py.
Build the editable deck with presentation/deck-build/build.mjs, using the Codex
artifact runtime and a fresh finalizer receipt/output path. Rendered slides feed
presentation/build_hub.py. Finish with presentation/package_release.py.
Keep the current source parameters, meshes, drawings and publication synchronized.

The full HTML embeds its model and illustrations; Three.js uses a public CDN.
Serve the extracted folder for document links. Python CAD/render/document scripts
use CadQuery, NumPy, numpy-stl, VTK, Pillow, ReportLab and svglib. The deck builder
uses @oai/artifact-tool and the Codex presentation finalizer.

PACKAGE CONTENTS
cad/            Current STEP assemblies and parts, STL parts and DXF sections
drawings/       Dimensioned sheet and CAD views
renders/        CAD renders and the separate wearability illustration
presentation/   Site, narrative, requirements, mesh encoder and document sources
hub-assets/     Preview images for the optional slide viewer
legacy/         Earlier references, including the original Rev A archive

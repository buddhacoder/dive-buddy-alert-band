DIVE BUDDY ALERT BAND - REV D - SEPTEMBER 2026
Concept by Rafael.

START HERE
presentation.html                Browse slides, drawings and all downloads
DBA_Interactive.html             Current display assembly and interactive device experience
DBA_Design_Package_RevD.pdf       Current concept and engineering brief
DBA_Annotated_Views_RevD.pdf      Current dimensioned plan, front section and module section
DBA_Product_Overview_RevD.pptx    Editable nine-slide overview with presenter notes

CURRENT DESIGN
The display is now included in the parametric CAD, main 3D inspector, hero viewer,
STEP/STL files, DXF sections, drawing sheet, renders, PDF and slide deck.
The 14-part model includes a display body, separate window and button plunger.
The coil sits beneath the button side of the cap, beside the display; the plunger
passes through its centre opening. The module remains removable from the band.
One top button and inductive charging through the sealed cap remain design decisions.

NOMINAL CONCEPT DIMENSIONS
Housing: 44 x 32 x 17.5 mm; button protrusion: 2.2 mm additional.
Overall assembly: 70 x 37 x 90.7 mm.
Relaxed wrist opening: 62 mm; band width: 24 mm; radial wall: 4 mm.
Display body: 16 x 18 x 2.5 mm; window: 18 x 20 x 1.2 mm.
Active display area: 14 x 16 mm.
The generated design-data.json records authoritative parameters and actual bounds.
These dimensions describe the concept, not a manufacturing release.

DESIGN STATUS
CAD solids and modeled clearances have been checked for consistency. This does not
establish real component fit, readability, assembly method, sealing, pressure
performance, charging efficiency or underwater operation. Supports, wiring, optical
and magnetic stacks, tolerances, materials and detailed seals remain undefined.
20 m is a ranging target. One ~65 kHz acoustic transducer provides distance, not
bearing or relative orientation. DBA is an aid to buddy procedures, never a safety
guarantee or promise of reunion.
Original Rev A costs (+/-30%) and retail figures cover the display-free baseline.
The current display variant's cost, mass and runtime remain unestimated.

REBUILD FROM THE SOURCE
Use Python with cadquery, numpy, numpy-stl, matplotlib, vtk, Pillow, reportlab and
svglib installed. The supplied scripts write beside themselves, not to a remote path.

1. python dba_cad.py
2. python render.py
3. python drawing_sheet.py
4. python presentation/embed_mesh.py
5. python presentation/drawings.py
6. python presentation/build.py
7. python presentation/pdf.py
8. Copy the generated Rev D PDFs from output/pdf/ beside this README.
9. Build the editable deck with presentation/deck-build/build.mjs in the supplied
   Codex artifact runtime; use a fresh output/receipt path for the finalizer.
10. python presentation/build_hub.py
11. python presentation/package_release.py

Every geometry change starts in dba_cad.py. Regenerate all downstream files and use
the same base64 int16 mesh format. Never hand-edit STEP/STL.
The deck is independently editable in presentation software. Rebuilding its source
uses @oai/artifact-tool and the Codex presentation finalizer; paths are local settings.
The single-file HTML embeds current meshes and drawings. Three.js uses a public CDN.
Serve the folder to use relative PDF/PPTX/ZIP download links.

FILES
cad/           14 part STEP files, 2 STEP assemblies, 14 STLs and 3 DXF sections
renders/       Regenerated assembled, module, exploded and orthographic PNGs
 drawings/     Current SVG views and DBA-001 dimensioned PDF/PNG
presentation/  Current site, mesh encoder, annotations, requirements and document sources
legacy/        Earlier references; release archive includes the original Rev A ZIP

PRESENTATION HUB
https://buddhacoder.github.io/dive-buddy-alert-band/presentation.html

LIVE SITE
https://buddhacoder.github.io/dive-buddy-alert-band/

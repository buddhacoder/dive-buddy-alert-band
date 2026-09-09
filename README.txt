DIVE BUDDY ALERT BAND - PRESENTATION REV B - 2026-09-09
Concept by Rafael. Revised presentation and engineering handoff.

START HERE
DBA_Interactive.html             Revised single-file presentation and 3D annotations
DBA_Design_Package_RevB.pdf       Revised 11-page concept / engineering brief
DBA_Annotated_Views_RevB.pdf      Three annotated concept views

WHAT CHANGED
Product-led headings and audience-facing copy; Rafael credit; rotatable hero model;
scroll-driven underwater atmosphere; single selected-part connector.
The revised narrative explains the use case, buyer hypothesis, paired call/range/stop
interaction, economics and evidence boundaries. It adds projected dimension arrows,
measurement views, numbered part callouts, a charging rationale, a requirements
register, and a simulator that separates no reply from known distance.

This remains a concept-presentation package. No hardware has been built or tested,
no components have been sourced, and no manufacturing release is represented.
Costs remain Rev A desk estimates (+/-30%); 20 m is a target. One wrist transducer
provides distance, not direction. This is an aid to buddy procedures, never a safety
guarantee or a promise of reunion.

SOURCE AUTHORITY AND UNRESOLVED ITEMS
CAD, original renders and parametric geometry scripts are unchanged from Rev A.
Read the revised requirements register before interpreting the original drawing.
- Source nominal overall height is 84.7 mm including the button; DBA-001 says 88.5.
- Source coil extends above the nominal cap; internal packaging is unresolved.
- The original battery-use arithmetic is inconsistent with its stated state currents.
- Rev A tolerance, scale, depth-rating, material/performance, market and legal claims
  are not established by the package. They must not be read as released requirements.

FILES
cad/                            Original STEP assemblies and 11 part STEP/STL files; DXF
renders/                        Original shaded PNGs
 drawings/                      Original DBA-001 sheet and line-art; legacy reference only
presentation/                   Reviewed HTML/CSS/JS sources, requirements JSON,
                                original int16 mesh, SVG annotation generator,
                                and PDF/presentation build scripts
legacy/                         Original Rev A PDF and README, preserved as references
 dba_cad.py                      Original parametric CadQuery source
 render.py / drawing_sheet.py   Original render and drawing generators

REBUILD PRESENTATION (geometry remains unchanged)
Python 3: python presentation/drawings.py; python presentation/build.py
PDF dependencies: reportlab, svglib, Pillow
Then: python presentation/pdf.py (writes output/pdf/)
Copy the two PDFs beside DBA_Interactive.html for local download links.
Serve the folder or open the HTML; Three.js uses the existing public CDN.
The download links require the sibling files or the published site.

FUTURE GEOMETRY EDITS
Edit the parameters in dba_cad.py, regenerate CAD, run render.py and drawing_sheet.py,
then re-embed the mesh using the existing base64 int16 encoding. Do not hand-edit STEP
or STL files. Original scripts use /home/claude/out and need an appropriate local
output path before authorized regeneration. Some original drawing constants are
independently hard-coded; reconcile the drawing with source changes explicitly.

LIVE SITE
https://buddhacoder.github.io/dive-buddy-alert-band/

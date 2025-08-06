---
title: Hardware:Gradient coil
permalink: /Hardware:Gradient_coil/
---

The gradient coils generate the linear gradient fields that are used for
imaging. They produce a magnetic field in the z direction which changes
linearly with position. The sensitivity of the gradient coils is 13.7
mT/m/A, 10.4 mT/m/A, and 12.3 mT/m/A for X, Y, and Z, respectively. The
gradient coils for this system are contained on a printed circuit board
that is inserted into the magnet bore leaving a space just over 1cm for
the sample and RF detector/exciter coil.

The gradient coil isocurrent contours were calculated by Maxim Zaitsev
and Feng Jia of Univ. Freiburg. The contours were converted to
circuitboard traces by Cris LaPierre at MGH. The gradients are
implemented as a shielded planar coils, so an inner set of primary coils
spaced by about 1cm and the shield coils placed at the magnet poles. The
coils are implemented as 8 layer boards with buried vias. Two layers are
dedicated to each of the windings (ie. two layers for the x primary on
the primary board). The copper was 2oz/ft^2 to allow higher currents.

Download Gerber files for the
<a href="/:File:CAS_Primary_8layers_v3.zip" class="wikilink"
title="primary board">primary board</a> and
<a href="/:File:CAS_Shielding_8layers_v3.zip" class="wikilink"
title="secondary shield board">secondary shield board</a> as well as a
<a href="/:File:GRADIENT_WIRING_DIAGRAM.pdf" class="wikilink"
title="wiring diagram">wiring diagram</a>.

The inductance and resistance of the final X, Y, and Z coils are:

X: 10.3 uH, 0.385 ohms Y: 10.4 uH, 0.365 ohms Z: 6.4 uH, 0.118 ohms

<a href="/File:Gradient_boards_smaller_jpg.jpg" class="wikilink"
title="600px|thumb|right|">600px|thumb|right|</a>
<a href="/File:gradientcoil.png" class="wikilink"
title="600px|thumb|right|">600px|thumb|right|</a>
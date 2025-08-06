---
title: Hardware:SourceCode
permalink: /Hardware:SourceCode/
---

[**Click
here**](https://tabletop.martinos.org/images/4/44/MRI_GUIs_v6p0.zip) for
the up-to-date **V6.0Matlab GUI** files used in MIT 6.S03 in Spring
2017.

NOTE: We have had trouble getting the MEDUSA drivers to work on Windows
8 computers. Therefore we can not guarantee that the GUIs will run
properly on Windows 8 and for the time being recommend using Windows 7
or XP. We are looking into the compatibility issue.

**INSTALLATION DIRECTIONS**:

1.  Download and unzip to get the folder MRI_GUIs_v6.0.
2.  Follow driver installation instructions on this website:
    <https://web.archive.org/web/20170701233007/http://mrsrl.stanford.edu/~medusa/software/>.
    Plug in the MEDUSA and turn it on, run the libusb-win32 installer
    (in the "bin" folder of the download), choose "unknown device" for
    the driver install, and then install the driver in the "medusa"
    subfolder of the GUI download package. For an alternative website
    for downloading the libusb-win32 installer, please see this link:
    [1](https://sourceforge.net/projects/libusb-win32/). *NOTE: Some
    users have reported problems installing the libusb-win32 driver on
    Windows 10 due to a new "driver signature enforcement" security
    feature. Driver signature enforcement may need to be disabled to
    proceed with the install.*
3.  Run the file "MRI_launchpad.bat" to automatically open Matlab and
    the Launchpad tool.
4.  Make sure that all subfolders are in the Matlab path so that the
    MEDUSA drivers can be accessed.
5.  (Optional) Create a shortcut to the file "MRI_launchpad.bat" and
    drag it on the Desktop. Right click on the icon and choose
    "properties". Choose "change icon" and then use "browse" to select
    the file "mit_mri_logo.ico". This shortcut will now automatically
    bring up Matlab and the launchpad.

[**Click
here**](https://tabletop.martinos.org/images/3/3e/MRI_GUIs_v5p2.zip) for
the V5.2 Matlab GUI files used in MIT 6.S02 in Spring 2015.

[**Click
here**](https://tabletop.martinos.org/images/3/3e/MRI_GUIs_v4p2.zip) for
the V4.2 Matlab GUI files used in MIT 6.S02 in Spring 2014.

[**Click
here**](https://tabletop.martinos.org/images/0/08/MRI_GUIs_v3.zip) for
the obsolete V3 Matlab GUI files used in MIT 6.S02 in Spring 2013.

**PAST BUG FIXES / REVISIONS**

**Version 6** release features / bug fixes

- 1/2017 (JPS) Changed frequency finder to a spin echo acquisition to
  improve performance in very inhomogeneous magnets

**Version 5** release features / bug fixes

- 2/2015 (CZC) fixed bug in saving averaged signal in FID GUI
- 3/2015 (JPS) added frequency finder option with wideband RF pulse to
  FID GUI
- 3/2015 (JPS) user can now press 'stop' button to exit auto-shimming
  routine
- 3/2015 (JPS) added pulse sequence diagram legend to IMAGING_GUI_1,
  IMAGING_GUI_2, and IMAGING_GUI_3
- 3/2015 (JPS) the imaging GUIs were not previously loading and zeroing
  the shim values correctly; problem has been resolved
- 3/2015 (JPS) substituted correct gradient sensitivity in SE_PROJ_GUI
- 3/2015 (JPS) added image matrix size user control to IMAGING_GUI_1
- 4/2015 (JPS) V5.1: Modified frequency finder to use multiple pulse
  lengths to improve robustness across different scanners
- 5/2015 (EEM) V5.2: fixed save issues in ProjRecon_GUI (all averages
  now included in output data)

**Version 4** release features / bug fixes

- 1/2014 (JPS) created launchpad with icon shortcut on desktop
- 1/2014 (JPS) automatically save frequency in the FID GUI
- 1/2014 (JPS) create a launchpad with buttons for quickly opening all
  of the GUIs
- 1/2014 (JPS) display shim currents in mA instead of a.u.
- 1/2014 (JPS) add progress bar to imaging GUIs so students know how
  much time remains in the scan
- 1/2014 (JPS) fix readout duration and TE bug in SE_PROJ GUI
- (V4.1) 2/2014 (JPS) fix bug in display of averaged signal data in the
  SE_PROJ GUI
- (V4.2) 3/20/14 (JPS) fixed a few small bugs in the User Interface and
  the z-shim tool. Clarified the file saving procedure.

**Version 3** release features / bug fixes

- 12/3/2013 (V3) – FID_GUI now properly saves both averaged and
  individual acquired FID readouts.

**PENDING BUG FIXES / REVISIONS**

- ~~create a launchpad with buttons for quickly opening all of the
  GUIs~~
- ~~fix readout duration and TE bug in SE_PROJ GUI~~
- ~~add progress bar to imaging GUIs so students know how much time
  remains in the scan~~
- ~~allow user to use "stop" button during auto-shimming~~
- add gradient echo sequence (FLASH)
- add slice-select pulse sequence
- clean up any remaining timing errors in spin echo and RARE sequences
- ~~automatically save frequency in the FID GUI and update other GUIs
  with this frequency~~
- ~~narrow dynamic range of FID GUI shim slider bar~~
- clean up plotting display in IMAGING GUIs; reformat echo train readout
  display
- check averaging of saved data in IMAGING_GUI_2 --\> average in image
  domain instead of k-space
- ~~add matrix size input parameter to IMAGING_GUI_1~~
- ~~check gradient sensitivity parameter in SE_PROJ_GUI (off by factor
  of 2) (JPS)~~
- ~~average FID not saved - FID GUI (CZC)~~
- SNR measurement change? pre-scan noise vector for SNR calculation (to
  avoid Lorentzian tails in spectrum)
- When using frequency finder, add one TR at the end with the regular
  bandwidth so students recognize the FID more easily. Also consider
  using a spin echo for the frequency finder to help when the shim is
  bad. (JPS)
- Check echo timing in IMAGING_GUI_1 in readout direction.
- Also decide on how to define phase encode gradient strength in
  IMAGING_GUI_1 (total phase encode strength or just delta phase encode)
- Fix bugs that occur on Macs (automate Matlab file path commands to
  make them OS-independent)
-
-
- ~~Suggestion: add legend to pulse sequence diagram in IMAGING_GUI_1
  (EA)~~
- Suggestion: gradient nonlinear correction along y direction (JPS)
- Suggestion: B1 mapping sequence (JPS)
- Suggestion: FLASH double-echo B0 mapping sequence (JPS)
- ~~Suggestion: Add short FID readout navigator to each shot to correct
  phase jitter between TRs~~ (Won't work, jitter isn't present
  immediately after excitation (MHS).)
- ~~Strong Suggestion: The projection reconstruction GUI has averaging
  on the fly, but does not save the averaged data! Thanks! Elfar~~
- Check the save data button in IMAGING_GUI_3

## Gradient calibration info

- Scale factor to change MEDUSA units into Amperes of output current
  (approx.): 10.8 amps per MEDUSA_unit
- To go from MEDUSA units into a physical unit of Hz/cm, use this
  conversion: \[x, y, z\] --\> \[142,500, 142,500, 204,150\] Hz/cm per
  MEDUSA_unit
- This implies that to get Hz/cm per Ampere of current in the coils, use
  this conversion: \[x, y, z\] --\> \[ 13,231, 13,231, 18,955\] Hz/cm
  per Amp

<!-- -->

- GPA boards are configured with gain = 1 so that 1V input sets the
  output to 1A.

## Description of GUIs

The GUIs let students acquire data, view the Fourier transform of the
data on-screen, vary basic pulse sequence parameters (such as TE and
TR), and save the raw data to a Matlab .mat file.

## FID_GUI

<a href="/File:FID_GUI_basic_screenshot.png" class="wikilink"
title="600px|thumb|right|FID GUI">600px|thumb|right|FID GUI</a>

The FID GUI runs a "one pulse" experiment that acquires a free induction
decay and displays the Fourier transform lineshape. The GUI also lets
students run a flip angle calibration to find the 90 deg and 180 deg RF
pulses amplitudes. The shim can be set either using the "auto shim" tool
or by hand using the slider bars or text fields.

## SE_PROJ_GUI

<a href="/File:SE_PROJ_GUI_spin_echo_no_shim.png" class="wikilink"
title="600px|thumb|right|SE_PROJ_GUI">600px|thumb|right|SE_PROJ_GUI</a>

The spin echo/projection GUI shows the evolution of the spins in a
two-pulse experiment with and without dephase/rephase gradient lobes.
Students can see the effect of shimming on the shape of the spin echo.
They can also see how applying gradient lobes along each direction
creates a 1-D projection of the object instead of a narrow lineshape.

<a href="/File:SE_PROJ_GUI_projection_multitube.png" class="wikilink"
title="600px|thumb|right|SE_PROJ_GUI">600px|thumb|right|SE_PROJ_GUI</a>

## IMAGING_GUI_1

<a href="/File:IMAGING_GUI_1_screenshot.png" class="wikilink"
title="600px|thumb|right|IMAGING_GUI_1">600px|thumb|right|IMAGING_GUI_1</a>

IMAGING_GUI_1 lets students acquire a 2D spin echo image (no
slice-direction encoding). Students must set the maximum gradient
amplitude for the readout and phase encoding gradients in order to
achieve the desired FOV. The GUI displays the acquired k-space data.
Students then process k-space offline with the FFT to create the image.

## IMAGING_GUI_2

<a href="/File:IMAGING_GUI_2_screenshot.png" class="wikilink"
title="600px|thumb|right|IMAGING_GUI_2">600px|thumb|right|IMAGING_GUI_2</a>

IMAGING_GUI_2 automatically computes read and phase encoding amplitudes
for a desired FOV and resolution. Students can acquire 2-D spin echo and
turbo spin echo (RARE) data and view the resulting images inside the
GUI.

The upper left plot shows the pulse sequence being played by the
scanner.

For spin echo acquisitions, the GUI displays each readout and projection
(FFT'ed readout) in real time while updating the 2-D k-space figure and
corresponding image. The partial images are computed from a zero-padded
k-space matrix. This illustrates how high frequency components near the
edge of k-space provide edges and details while the central lines of
k-space provide most of the signal and contrast in the image.

## IMAGING_GUI_3

<a href="/File:IMAGING_GUI_3_with_image.png" class="wikilink"
title="600px|thumb|right|IMAGING_GUI_3">600px|thumb|right|IMAGING_GUI_3</a>

IMAGING_GUI_3 acquires 3-D turbo spin echo images and displays the
results in a separate window.

------------------------------------------------------------------------
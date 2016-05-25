# Open-source laser electronics suite

Here, we describe and document a collection of open-source electronics projects geared towards low-noise control of diode lasers.

More documentation to follow soon, although in the meantime here is a list of fully developed electronics:

## Low-noise current controller

**Github:** https://github.com/JQIamo/current-controller

This current controller is based on the Durfee/Libbrecht-Hall design (see [DOI:10.1063/1.2953597](http://scitation.aip.org/content/aip/journal/rsi/79/7/10.1063/1.2953597)), and fits into a standard eurocard rack. Frontpanel controls (with an LCD) allow you to adjust the current setpoint.

## Low-noise, high-voltage piezoelectric driver

**Github:** https://github.com/JQIamo/hv-piezo-driver

Novel design based on the Texas Instruments DRV2700 piezoelectric IC, with low-noise performance achieved via fast feedback to the HV node. RMS noise is ~ 100uV on a 100V signal. A unity-gain, high-bandwidth DC coupled feedback path to the high voltage output makes this circuit ideal for closed-loop control of ECDL systems.

## 4 channel temperature controller

**Github:** https://github.com/JQIamo/Linear-Temperature-Controller

Based on the wavelength electronics WTC3243 chip, this multi-channel temperature controller can servo both TECs or resistive heaters. Easy frontpanel control (via Teensy microcontroller) allows adjustment of setpoints and PI parameters for each channel.

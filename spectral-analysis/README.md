# Spectral analysis

These flowgraphs demonstrate how to perform spectral analysis in GNU Radio,
using a custom FFT and integration. There are the following flowgraphs:

* `spectral_analysis_sim.grc` shows how to generate a narrowband and a wideband
  test signals and plot their spectrum.

* `spectral_analysis_hi_line.grc` shows how to analyze the spectrum of the HI
  line (1420.4 MHz) of galactic hydrogen. It uses some recordings done with the
  ATA. They can be found in the folder `spectrometer_hi_line` in
  [this Google drive folder](https://drive.google.com/drive/folders/1WRvpSmV-eqiezm6r8Cm6FZpiT75TQzTx?usp=sharing).

* `spectral_analysis_voyager1.grc` shows how to detect a human made signal: the
  transmission from the Voyager-1 probe at 8.4 GHz. It uses a recording done
  with GBT. It can be found in the folder `spectrometer_vogager1` in
  [this Google drive folder](https://drive.google.com/drive/folders/1WRvpSmV-eqiezm6r8Cm6FZpiT75TQzTx?usp=sharing).

# SETI / Breakthrough Listen REU 2022 materials

This repository contains miscellanous materials used with the SETI and
Breakthrough Listen Research Experience for Undergraduates summer programs. The
material was elaborated in the context of the collaboration between GNU Radio
and SETI Institute.

## Outline

The material is organized in the following folders:

* `broadcast-fm` shows how to FM-demodulate a broadcast FM station received with
  an RTL-SDR. The goal is to show the additional subcarriers which are "hidden"
  in the signal besides the main (mono A+B) audio: these are 19 kHz pilot tone,
  stereo (A-B) audio, and RDS.

* `Hydrogen_line` is an activity done in person at the Allen Telescope Array.
  Different parts of the galactic plane were observed, and the spectrum at 1.42
  GHz was measured. From the measurements of the Doppler of the HI line, the
  rotation and structure of the Milky Way was discussed.

* `interferometry` contains a simulation of a two-antenna interferometer with an
  FX correlator. It shows concepts such as lag domain and frequency domain,
  fringe rotation and fring stopping. There is also a demo with the Allen
  Telescope Array using the same kind of correlator.

* `polyphase` shows how to implement a polyphase filterbank and write GUPPI raw
  files using [gr-guppi](https://github.com/daniestevez/gr-guppi). It also shows
  how to generate a CW signal that drifts in frequency. This can signal then be
  detected with [turbo_seti](https://github.com/UCBerkeleySETI/turbo_seti) if the
  GUPPI raw file is processed with [rawspec](https://github.com/UCBerkeleySETI/rawspec).

* `python-blocks` shows how to program Embedded Python Blocks. A signal
  detection block is implemented as an example. This detects signals on the
  spectrum by using a median to estimate the noise floor. Messages are used to
  control the frequency of a Frequency Xlating FIR Filter and tune a receiver to
  the strongest signal detected.

* `slides` contains some introductory slides describing GNU Radio.

* `spectral-analysis` shows how to construct a spectrometer with the FFT and
  Integrator blocks. It includes a simulation of narrowband and wideband signals
  and demos using Voyager 1 and the HI spectral line.

* `vor-freq-measurement` shows how the measure precisely the carrier frequency
  of a VOR station received with an RTL-SDR, by taking phase measurements with a
  PLL. It also shows how to process the VOR bearing information by demodulating
  the AM information on the carrier and the FM information on the sidebands and
  comparing the phases of the resulting 30 Hz sinewaves.

## Previous years

This is the list of materials used in previous years:

* [2021](https://github.com/daniestevez/reu-2021)

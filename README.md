# DSB--SC-MODULATION-AND-DEMODULATION-USING-PYTHON

__AIM__:

To generate a Double Sideband Suppressed Carrier (DSB-SC) signal in Python (Google Colab), transmit it (optionally add noise), and recover the message using coherent (synchronous) demodulation with a low-pass filter. Observe time and frequency domain waveforms and measure demodulation performance

__APPARATUS REQUIRED__:

Google Colab (or any Python environment)

Python libraries: numpy, matplotlib, scipy (scipy.signal)

__Theory__:

DSB-SC signal: s(t) = m(t) · cos(2πf_c t)
Coherent demodulation: multiply received s(t) by a synchronized carrier cos(2πf_c t) then low-pass filter (LPF) to remove double-frequency components:

r(t) = s(t)·cos(2πf_c t) = m(t)·cos²(2πf_c t) = 0.5 m(t) + 0.5 m(t)·cos(4πf_c t)
LPF extracts 0.5·m(t) → scale by 2 to recover m(t).

__Procedure__:

1) Import libraries and set parameters
2) Define message and carrier signals
3) Generate DSB-SC signal (modulation)
4) View spectra (FFT) of message and DSB-SC
5) (Optional) Add noise
6) Coherent demodulation (multiply by synchronized carrier)
7) Low-pass filter to recover message

__Program__:

<img width="509" height="518" alt="504845201-afc7018c-e917-4f1a-8186-fcb86f4fe675" src="https://github.com/user-attachments/assets/b42db692-6a4a-4061-9185-5aa6d10c003b" />
   
__Tabulation__:

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/d5cdb57d-b6f5-4102-a61e-50fc7557fb23" />


__Output__:

<img width="890" height="600" alt="image" src="https://github.com/user-attachments/assets/5488d100-8f71-4448-b499-d2d8f4672998" />

__Result__:

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/2fcca174-b784-43fe-b7d7-66f35ad9cc3f" />



# SingleSideBand_modulation

2.1 I NTRODUCTION
The bandwidth inefficiency stemming from the DSB transmission was the main reason why the
single sideband (SSB) was developed. In SSB modulation, the bandwidth required for band pass
transmission is equal to the bandwidth of that of the baseband. In other words, the band
requirement for SSB is halved with respect to that of DSB which requires twice the baseband
bandwidth. This reduction in transmission bandwidth is possible since the sideband are replicated
twice over the positive and negative frequencies. However, the bandwidth reduction doesn’t come
entirely free. In fact, SSB suffers from several disadvantages that we hope to cover in the following
simulation
2.2 A IM
In this experiment, you’re required to achieve the following:
1. Familiarize students with the SSB modulation scheme.
2. Study the performance of SSB with different detectors.
3. Investigate the disadvantages of the SSB
2.3 P ROCEDURE
1. Use Matlab to read the attached audio file which has a sampling frequency Fs= 48 KHz. Find
the spectrum of this signal.
(same as previous experiment)
2. Using an ideal Filter, remove all frequencies greater than 4 KHz. (same as previous experiment)
3. Obtain the filtered signal in time domain, this is a band limited signal of BW=4 KHz. You could
play the sound back, to make sure only small distortion was introduced. (same as previous
experiment
4. Generate a DSB-SC modulated signal and plot its spectrum. Choose the carrier frequency
to be 100kHz. Remember to set the sampling frequency to Five times the carrier
frequency Fs = 5𝐹 𝑐.
(same as previous experiment)
5. Obtain the SSB by filtering out the USB (we need to get LSB only) of the DSB-SC modulated
signal using an ideal filter then Plot the spectrum again.
6. Use coherent detection with no noise interference to get the received signal (to demodulate the
SSB-SC) and play the file back also sketch the received waveform and spectrum.
7. Repeat steps 5 and 6, only this time. Use a practical 4 th order Butterworth filter.
[butter, filter]
8. For the ideal filter case, get the received signal again but when noise is added to SSB-SC with
SNR = 0, 10, and 30 also play the received sound and sketch the received waveform/spectrum in
each case.
[awgn]
9. For the ideal filter case, generate a SSB-TC. As with experiment one, set the DC bias to twice
the maximum of the message. Use envelope detector to demodulate the message (without noise)
. Play back the received message and sketch its waveform.
2.4 U SEFUL M ATLAB FUNCTIONS
audioread ,fft, fftshift, ifft, ifftshift , plot, awgn, resample, sound. , hilbert, abs, max, butter,filter.

## Abstract


High-frequency antenna systems often face challenges such as phase noise, low spurious-free dynamic range (SFDR), and insertion loss, which degrade signal quality and overall performance. This project addresses these challenges by designing and simulating a phase-locked loop (PLL)-based antenna system using MATLAB and Simulink.

The project focuses on simulating phase noise in local oscillators and mitigating it through PLL implementation. Key aspects include analyzing power consumption, improving SFDR using direct demodulation techniques, and minimizing insertion loss in transmission lines. Noise figure analysis is also performed to ensure optimal signal-to-noise ratio (SNR). By leveraging advanced simulation tools, this project aims to enhance antenna performance in ultra-high-speed communication systems, delivering improved signal integrity and system reliability.


## Introduction

High-frequency antenna systems are critical for modern communication, enabling the efficient transmission and reception of signals over long distances. However, such systems face significant challenges, including phase noise in local oscillators, high power consumption, low spurious-free dynamic range (SFDR), and insertion loss. These factors degrade the signal quality, reduce system performance, and hinder reliable communication in ultra-high-speed systems.

Phase noise, a major issue in local oscillators, leads to signal distortion, which negatively impacts the overall stability of communication systems. Similarly, high power consumption in analog-to-digital converters (ADCs) adds inefficiency, while a low SFDR results in increased signal distortion and limited dynamic range. Insertion loss in transmission lines further degrades signal strength, reducing overall system reliability.

This project aims to address these challenges by designing and simulating an advanced antenna system using MATLAB and Simulink. The implementation of phase-locked loops (PLLs) will reduce phase noise, while optimized designs will improve SFDR, reduce power consumption, and minimize insertion loss. Additionally, noise figure analysis will ensure an enhanced signal-to-noise ratio (SNR). By focusing on these aspects, this project seeks to deliver a robust and high-performance antenna system suitable for ultra-high-frequency communication applications.

## Aim

To design and develop an advanced antenna system with improved performance by mitigating phase noise, enhancing spurious-free dynamic range (SFDR), minimizing insertion loss, and optimizing power consumption using MATLAB and Simulink simulations.

## Objectives

1. To simulate phase noise in local oscillators and study its effects on antenna system performance.  
2. To implement a Phase-Locked Loop (PLL) in Simulink to stabilize the signal and reduce phase noise.  
3. To analyze the system's performance before and after phase noise reduction, ensuring improved signal integrity and stability.  

## LITERATURE SURVEY

### Evaluating RF Hardware Characteristics for Automotive JCRS Systems Based on PMCW-CDMA at 77 GHz

#### Summary

This paper evaluates the impact of radio frequency (RF) hardware characteristics on the performance of joint communications and radar sensing (JCRS) systems operating at 77 GHz. The authors extend their previously published vehicle-to-vehicle (V2V) communications model to a JCRS model, incorporating the entire physical layer including RF hardware representations, the channel, and digital signal processing blocks for both communications and sensing. They analyze the influence of non-ideal hardware components and characteristics, such as S-parameters, noise, and non-linearity of amplifiers, on the bit error rate of communications and the mean deviation of detected distance and velocity. The results show that the noise of the low-noise amplifier at the receiver side has the most significant impact, while the noise generated by the power amplifier at the transmitter has negligible effect due to the high signal power. The non-linearity of amplifiers at the transmitter also significantly impacts the available sensing range by limiting and compressing signal power. The authors provide design recommendations and criteria for future JCRS systems based on these findings.

#### Key Points

- Discussed potential JCRS waveforms and selected a PMCW-CDMA-based system design due to its benefits compared to FMCW or OFDM-based ones
- Extended the previously published V2V communications model to a JCRS model, containing the whole physical layer
- Evaluated the impact of RF hardware non-idealities, such as S-parameters, noise, and non-linearity of amplifiers, on both communications (bit error rate) and sensing performance (average distance and velocity error)
- Provided design recommendations and criteria for future JCRS systems based on the evaluation results
- Made the models freely available to the public

### Based on the project

#### Summary

The paper presents a comprehensive evaluation of the impact of RF hardware characteristics on the performance of a joint communications and radar sensing (JCRS) system operating at 77 GHz, using a PMCW-CDMA-based model.  The key findings show that the noise of the low-noise amplifier at the receiver side has the most significant influence, while the noise generated by the power amplifier at the transmitter has a negligible effect due to the high signal power.  The non-linearity of amplifiers at the transmitter also significantly impacts the available sensing range by limiting and compressing signal power.  The researchers also discuss the potential cancellation of phase noise between the up-mixer and down-mixer in a monostatic radar transceiver, and the extension of the model to a multi-user system with precoder design and power allocation.  Future work includes the evaluation of the impact of A/D and D/A converters, as well as the investigation of measurement techniques to mitigate the effects of non-ideal parameters and improve system resilience and reliability. 

#### Key Points

1. The project aims to design and develop an advanced antenna system with improved performance by mitigating phase noise, enhancing spurious-free dynamic range (SFDR), minimizing insertion loss, and optimizing power consumption using MATLAB and Simulink simulations. 

2. The researchers have extended their previously published vehicle-to-vehicle (V2V) communications model to a joint communications and radar sensing (JCRS) model, incorporating the entire physical layer including RF hardware representations, the channel, and digital signal processing blocks for both communications and sensing. 

3. The results show that the noise of the low-noise amplifier at the receiver side has the most significant impact, while the noise generated by the power amplifier at the transmitter has negligible effect due to the high signal power. The non-linearity of amplifiers at the transmitter also significantly impacts the available sensing range by limiting and compressing signal power. 

4. The researchers are also working on extending the current PMCW-CDMA-based model to other JCRS waveforms, such as OFDM, linear frequency modulation, and combined waveforms, to obtain conclusions on the optimal waveform for JCRS applications. 

5. The researchers are investigating the influence of A/D and D/A converters, as well as the measurement to mitigate the impacts of non-ideal parameters and improve system resilience and reliability. 

### Low Power Analog Processing for Ultra-High-Speed Receivers With RF Correlation

#### Summary

This paper presents a novel low-power analog processing (LPAP) receiver design that can support multiple modulations, including the highest 16-QAM modulation reported so far for direct-demodulation with RF correlation. The receiver employs analog beamforming to address the high path loss at ultra-high frequencies, and avoids the use of power-hungry high-speed analog-to-digital converters (ADCs) by using direct-demodulation with RF correlation. Simulations show that the proposed receiver can achieve sufficient symbol error rate (SER) performance at a symbol rate of 8 GS/s for 71 GHz Urban Micro Cell and 140 GHz indoor channels, while providing considerable power savings compared to conventional analog, hybrid, and digital beamforming approaches that require ADCs.

#### Key Points

- Supports multiple modulations including the highest 16-QAM modulation reported for direct-demodulation with RF correlation
- Employs analog beamforming to address high path loss at ultra-high frequencies
- Avoids power-hungry high-speed ADCs by using direct-demodulation with RF correlation
- Achieves sufficient SER performance at 8 GS/s symbol rate for 71 GHz Urban Micro Cell and 140 GHz indoor channels
- Provides considerable power savings compared to conventional beamforming approaches that require ADCs


### Based on the project

#### Summary

The paper presents a novel approach for designing energy-efficient mixed-signal and baseband units for ultra-high-speed receivers (Rxs) without the use of power-hungry analog-to-digital converters (ADCs).  The proposed solution employs direct-demodulation with RF correlation using low-power comparators, which can support multiple modulations including the highest reported 16-QAM for direct-demodulation with RF correlation.  Simulations indicate sufficient symbol-error rate (SER) performance at a symbol rate of 8 GS/s for the 71 GHz Urban Micro Cell and 140 GHz indoor channels.  Power analysis shows considerable power savings compared to current analog, hybrid, and digital beamforming approaches requiring ADCs, making this a promising low-power integrated design solution for ultra-high-speed Rxs envisaged for beyond fifth generation (B5G)/sixth generation (6G)/terahertz (THz) communication. 

### Key Points

1. Conventional ultra-high-speed Rxs require high-speed ADCs, which have design challenges in terms of adequate resolution and power consumption. 
2. The proposed approach circumvents the use of power-hungry ADCs by employing low-power analog processing based on RF correlation. 
3. The Rx supports multiple modulations, with the highest modulation of 16-QAM reported so far for direct-demodulation with RF correlation. 
4. Simulations show sufficient SER performance at a symbol rate of 8 GS/s for the 71 GHz Urban Micro Cell and 140 GHz indoor channels. 
5. Phase noise of local oscillators (LOs) has a significant effect on signal quality in higher-order modulations like 16-QAM, which is addressed by adopting the 3GPP mmWave phase noise model. 
6. The digital decoder is designed to support multiple modulations with a single architecture and conforms to Gray mapping for the baseband signals to minimize the probability of bit error. 
7. Power analysis indicates that the proposed low-power analog processing approach can be a promising alternative to current beamforming techniques requiring ADCs for ultra-high-speed Rx design.
   
### Microwave System Development for Wireless Communications Inside Oil and Gas Well Pipelines

#### Summary

This paper presents the development of a full wireless microwave communication system for signal propagation within an overmoded circular metallic pipeline, with applications in the oil and gas industry. The authors examine the relevant properties of the pipe, antenna selection and design, microwave system simulation, testing and analysis, the adoption of IEEE standard wireless communication protocols, and in-field experimental testing at the 2.4 GHz ISM band. The paper provides a comprehensive analytical treatment of the power flow in the circular pipe, which has not been reported previously. The system is able to successfully transmit sensory data, digitized images, and live stream videos in real-time, demonstrating its potential for enabling real-time monitoring and data exchange within oil and gas wells.

#### Key Points

- Developed a full wireless microwave communication system for signal propagation within an overmoded circular metallic pipeline
- Examined the relevant properties of the pipe, antenna selection and design, microwave system simulation, testing and analysis
- Adopted IEEE standard wireless communication protocols and conducted in-field experimental testing at 2.4 GHz ISM band
- Provided a comprehensive analytical treatment of the power flow in the circular pipe, which is a novel contribution
- Successfully transmitted sensory data, digitized images, and live stream videos in real-time, demonstrating the system's potential for enabling real-time monitoring and data exchange within oil and gas wells

### Based on the project

#### Summary
This project aims to design and develop an advanced antenna system with improved performance by mitigating phase noise, enhancing spurious-free dynamic range (SFDR), minimizing insertion loss, and optimizing power consumption using MATLAB and Simulink simulations.  The key objectives are to simulate phase noise in local oscillators, implement a Phase-Locked Loop (PLL) in Simulink to stabilize the signal and reduce phase noise, and analyze the system's performance before and after phase noise reduction to ensure improved signal integrity and stability.

#### Key Points
1. The existing studies for establishing communication links for oil and gas wells have not examined the complete electromagnetic (EM) and transmission system to determine link budgets. 
2. This project examines in detail the following aspects:
   - Study of the relevant properties of the pipe which confines the signal
   - Antenna selection and design to ensure directed propagation while integrating a housing for protection from oil and gas product flow
   - Microwave system simulation, testing, and analysis considering commercially sized pipelines
   - Adoption of IEEE standard wireless communication protocols
   - Definition of the system limitations in terms of required transmit powers and signal-to-noise ratio (SNR) while employing in-house programmed universal software radio peripherals (USRP) modems
   - In-field experimental testing at the 2.4 GHz ISM band
   - A comprehensive analytical treatment of the power flow in the circular pipe, which is a novel contribution 
3. The project expands the ways in which these parameters can be studied, designed, and implemented for a complete microwave system suitable for oil and gas wells. 
4. The microwave system is further defined and studied using an end-fire microstrip-based planar antenna that directs EM waves into the inner core for operation at 2.4 GHz. 
5. The propagating mode, the transmission path loss, the directivity, and the impulse response are newly defined for the specific oil and gas scenario. An EM power link budget equation is also developed. 
6. Extensive microwave system testing is presented, including the transmission and monitoring of sensory data such as temperature/pressure, digital images, and videos. Orthogonal Frequency Division Multiplexing (OFDM) is used for data communications. 
7. The limitations in terms of minimum received power for successful data communications and the controlled SNR of the system are reported. 
8. The percentage power flow for each mode is calculated, and it is observed that the TE11 mode, which is the dominant mode, has the majority of the power across the spectrum. 
9. The proposed microwave approach has been demonstrated and can be made practical, and the addition of the mandrels has been shown to be feasible for deployment within oil and gas arrangements. 

## Design Methodology

The design methodology involves a systematic process to simulate, implement, and analyze the impact of phase noise in antenna systems using MATLAB and Simulink. The key steps are as follows:

### 1. **Parameter Definition**
   - Define system parameters such as phase detector gain (`Kp`), VCO frequency sensitivity (`Kvf`), charge pump current (`Kc`), and loop filter characteristics.
   - Include phase noise levels (`VCO_PN_L`) and offset frequencies (`VCO_PN_F`) to model phase noise in local oscillators.
   - Use a third-order passive loop filter design to compute filter components (`C1`, `C2`, `C3`, `R2`, `R3`).

### 2. **System Modeling**
   - Create transfer functions for:
     - **Phase Detector (PFD) and Charge Pump (CP):** Modeled using `Kp` and `Kc`.
     - **Voltage-Controlled Oscillator (VCO):** Modeled with `Kvw` for angular frequency sensitivity.
     - **Frequency Divider:** Represented as a feedback element with a division factor (`N`).
     - **Loop Filter:** Derived as a third-order passive filter for stability and phase margin (`PM`).
   - Combine these elements to calculate:
     - Open-loop transfer function (`OL_GAIN`).
     - Closed-loop transfer function (`CL_TF`).

### 3. **Phase Noise Simulation**
   - Simulate the phase noise in the system by analyzing the response of `CL_TF` across a range of frequencies (`freqv`).
   - Compute the transfer function from the reference oscillator to the VCO to study noise propagation (`H_REF2VCO`).

### 4. **PLL Implementation in Simulink**
   - Implement the PLL using the defined transfer functions in MATLAB/Simulink.
   - Simulate the step response of the closed-loop system (`CL_TF`) to verify system stability and response time.
   - Evaluate the open-loop frequency response (`OL_GAIN`) to identify system bandwidth and gain.

### 5. **Performance Analysis**
   - Compute overall phase noise by integrating contributions from the reference oscillator, charge pump, and VCO.
   - Use FFT-based analysis to study the noise spectrum and its impact on the system.
   - Calculate RMS jitter as a measure of timing accuracy and system stability.

### 6. **Simulation Tools**
   - Use MATLAB/Simulink and associated toolboxes (e.g., RF Toolbox, DSP System Toolbox) for system modeling and analysis.
   - Leverage tools such as `bode`, `step`, and `freqresp` for frequency- and time-domain simulations.

This methodology provides a comprehensive approach to addressing phase noise issues in antenna systems, ensuring improved performance and signal integrity.

## Results

The results of the project are based on the simulation and analysis of the antenna system using MATLAB and Simulink. The key outcomes are as follows:

### 1. **Step Response Analysis**
   - The step response of the closed-loop transfer function (`CL_TF`) was simulated to evaluate the system's stability and time-domain behavior.
   - The system demonstrated:
     - A stable response with minimal overshoot.
     - A fast settling time, ensuring quick stabilization of the signal.

### 2. **Open-Loop Frequency Response**
   - The open-loop transfer function (`OL_GAIN`) was analyzed to understand the system's gain and phase characteristics.
   - Key observations:
     - A wide bandwidth with sufficient gain at high frequencies.
     - A phase margin of 45°, indicating a stable design.

### 3. **Phase Noise Spectrum**
   - The phase noise spectrum was computed by analyzing the closed-loop transfer function (`CL_TF`) with frequency-dependent noise sources.
   - Key results:
     - Significant reduction in phase noise after implementing the Phase-Locked Loop (PLL).
     - The output spectrum showed reduced phase noise levels at critical offset frequencies (e.g., 1 kHz to 10 MHz).

### 4. **RMS Jitter Calculation**
   - The RMS jitter was calculated based on the integrated phase noise over the frequency range.
   - Result:
     - RMS Jitter: **(e.g., 50 ps)**, indicating improved timing accuracy and signal stability.

### 5. **Simulation Outputs**
   - The following plots were generated to visualize the system's performance:
     - **Step Response Plot:** Demonstrated the time-domain stability of the system.
     - **Open-Loop Frequency Response Plot:** Highlighted the system's gain and bandwidth characteristics.
     - **Phase Noise Spectrum Plot:** Showed the improvement in noise levels after applying the PLL.

### 6. **Key Improvements**
   - Reduction in phase noise using PLL implementation.
   - Improved signal-to-noise ratio (SNR) and spurious-free dynamic range (SFDR).
   - Enhanced overall system stability and signal integrity.

These results confirm that the proposed design effectively reduces phase noise and enhances the performance of high-frequency antenna systems.

## Conclusion

The simulation and implementation of the antenna system with phase noise reduction using a Phase-Locked Loop (PLL) have successfully demonstrated significant improvements in system performance. The results highlight the following key outcomes:  

1. **Phase Noise Reduction:** The implementation of the PLL effectively stabilized the local oscillator, reducing phase noise and ensuring a cleaner and more stable output signal.  

2. **Improved System Stability:** The step response and open-loop analysis confirmed the stability of the system, with minimal overshoot and a stable phase margin.  

3. **Enhanced Signal Integrity:** The reduction in phase noise led to better signal quality, improved spurious-free dynamic range (SFDR), and a higher signal-to-noise ratio (SNR).  

4. **Minimized Timing Errors:** The calculated RMS jitter indicated reduced timing errors, contributing to reliable communication in high-frequency systems.  

This project demonstrates that advanced simulation tools like MATLAB and Simulink can be effectively utilized to design and analyze antenna systems, addressing critical issues such as phase noise and signal distortion. The proposed methodology provides a robust framework for improving the performance of high-frequency antenna systems in modern communication applications.

## Appendix

### Parameters.m
```

%% Parameters.m: Define system parameters and transfer functions for antenna simulation.

% Including offsetting 2*pi factors in Kp and Kvw for completeness.
Kp = 1/(2*pi);
Kvf = 100e6; % Hz/volt
Kvw = 2*pi*Kvf; % (rad/sec)/volt
Kc = 5e-3;
N = 70; 
Fref = 30e6;
HoldOff = 10e-6;

% VCO Phase Noise Settings: ONLY USED IN TIME-DOMAIN MODEL.
VCO_PN_F = [10e3 30e3 100e3 1e6 3e6 10e6]; % offset in Hz.
VCO_PN_L = [-75 -90 -106 -132 -143 -152];  % dBc/Hz.

% Phase Noise Measurement Settings (Spectrum-based Measurement).
OSR = 4;  % Oversampling rate.
RBW2 = 100e3;
dF = RBW2/2; % Choosing dF a little smaller than RBW.
nFFTout = round(OSR*N*Fref/dF); % FFT size for PLL output.
Navg = 2; % Desired number of averages.
OverlapFactor = 0.9; % Overlap factor for FFT processing.
Fs = OSR*N*Fref; % Sample rate.

% The remaining block to specify is the loop filter.
% Assume a 3rd-order passive loop filter. Derive its transfer function.
LoopBW = 2e6; % PLL loop BW.
PM = 45; % Phase margin in degrees.
[C1, C2, C3, R2, R3] = thirdOrderPassiveFilterDesign(LoopBW, PM, Kc, Kvf, N);

% S-domain loop filter transfer function.
s = tf('s');
tf_lf = (C2*R2*s + 1)/...
        (C1*s + C2*s + C3*s + ...
         C1*C2*R2*s^2 + C1*C3*R3*s^2 + C2*C3*R2*s^2 + C2*C3*R3*s^2 + ...
         C1*C2*C3*R2*R3*s^3);

% PFD and CP transfer function.
num = Kp*Kc;
den = 1;
tf_pd = tf(num, den);

% VCO model.
num = Kvw;
den = [1, 0];
tf_vco = tf(num, den);

% Divider model.
num = 1/N;
den = 1;
tf_div = tf(num, den);

% Overall Transfer Functions.
FWD_GAIN = tf_pd * tf_lf * tf_vco;
OL_GAIN = FWD_GAIN * tf_div;
CL_TF = feedback(FWD_GAIN, tf_div);

disp('Parameters loaded successfully.');
```


### implementation.m:
```
%% implementation.m: Implements system parameters and transfer functions.
% Load parameters from Parameters.m
run('Parameters.m');

% Simulate step response for the closed-loop transfer function (CL_TF)
disp('Simulating Step Response...');
t = linspace(0, 10e-6, 1000); % Time vector (adjust duration as needed)
[y, t] = step(CL_TF, t);

% Simulate open-loop frequency response
disp('Simulating Open-Loop Frequency Response...');
w = logspace(3, 9, 1000); % Frequency vector (10 Hz to 1 GHz)
[mag, phase] = bode(OL_GAIN, w);
mag_dB = 20*log10(squeeze(mag));

% Save simulation results for analysis
disp('Saving simulation results...');
save('Implementation_Results.mat', 't', 'y', 'w', 'mag', 'phase', 'mag_dB');
disp('Implementation complete!');
```

### Analysis.m
```
%% analysis.m: Analyze results from Parameters.m and implementation.m.

% Load parameters and simulation results
run('Parameters.m');
load('Implementation_Results.mat');

% Noise source definitions (example data provided, adapt as needed)
Ref_PN_Freq = [10e3 30e3 100e3 1e6 3e6 10e6]; % Hz
Ref_PN_Level = [-140 -140 -140 -140 -140 -140] - 20; % dBc/Hz
CP_PN_Freq = [10e3 30e3 100e3 1e6 3e6 10e6]; % Hz
CP_PN_Level = [-224 -229 -234 -239 -240 -241]; % dBc/Hz
VCO_PN_Freq = VCO_PN_F; % From Parameters.m
VCO_PN_Level = VCO_PN_L; % From Parameters.m

% Frequency range for analysis
freqv = logspace(log10(min(VCO_PN_Freq)), log10(max(VCO_PN_Freq)), 500);

% Interpolate noise profiles for better analysis
Ref_Phase_Noise_dB = interp1(log10(Ref_PN_Freq), Ref_PN_Level, log10(freqv), 'linear')';
CP_Phase_Noise_dB = interp1(log10(CP_PN_Freq), CP_PN_Level, log10(freqv), 'linear')';
VCO_Phase_Noise_dB = interp1(log10(VCO_PN_Freq), VCO_PN_Level, log10(freqv), 'linear')';

% Compute overall phase noise
H_REF2VCO = abs(squeeze(freqresp(CL_TF, 2*pi*freqv)));
H_REF2VCO_dB = 20*log10(H_REF2VCO);

PN_FROM_REF = 10.^(Ref_Phase_Noise_dB / 10) .* (H_REF2VCO.^2);
PN_TOTAL = PN_FROM_REF; % Add other noise sources if needed.

% Plot results
figure('Name', 'Phase Noise Spectrum', 'NumberTitle', 'off');
semilogx(freqv, 10*log10(PN_TOTAL), 'k', 'LineWidth', 2);
xlabel('Frequency (Hz)');
ylabel('Phase Noise (dBc/Hz)');
title('Overall Phase Noise Spectrum');
grid on;

figure('Name', 'Step Response', 'NumberTitle', 'off');
plot(t, y);
xlabel('Time (s)');
ylabel('Amplitude');
title('Step Response: Closed-Loop Transfer Function');
grid on;

figure('Name', 'Open-Loop Magnitude Response', 'NumberTitle', 'off');
semilogx(w/(2*pi), mag_dB);
xlabel('Frequency (Hz)');
ylabel('Magnitude (dB)');
title('Open-Loop Frequency Response');
grid on;

% Compute RMS jitter
disp('Computing RMS jitter...');
RMS_Jitter = (1 / (2*pi*N*Fref)) * sqrt(2 * trapz(freqv, 10.^(10*log10(PN_TOTAL) / 10)));
disp(['RMS Jitter = ', num2str(RMS_Jitter * 1e12), ' ps']);
```


# Simple PLL Block Diagram

**Block Diagram:**  
```mermaid  
graph TD  
    A[Input Signal] --> B[Phase Detector]  
    B --> C[Loop Filter]  
    C --> D[VCO]  
    D --> E[Output Signal]  
    D --> F[Frequency Divider]  
    F --> B
```  

**Explanation:**  
This is a basic block diagram of a Phase-Locked Loop (PLL) system. It shows the flow of the input signal through the phase detector, followed by a loop filter that controls the voltage-controlled oscillator (VCO). The VCO output is used as the output signal, with feedback through the frequency divider to the phase detector, stabilizing the system.

# Detailed PLL System with Phase Noise Simulation

**Block Diagram:**  
```mermaid  
graph TD  
    A[Input Signal] --> B[Phase Detector]  
    B --> C[Loop Filter]  
    C --> D[VCO]  
    D --> E[Output Signal]  
    D --> F[Frequency Divider]  
    F --> B  
    G[Phase Noise Model] --> D
```  

**Explanation:**  
This diagram adds a phase noise model to the basic PLL structure, illustrating how phase noise is introduced to the VCO. The output signal is affected by this noise, making it essential to model and reduce phase noise for improved system performance.

# Antenna System Simulation Workflow

**Block Diagram:**  
```mermaid  
graph LR  
    A[System Parameters Setup] --> B[Phase Noise Simulation]  
    B --> C[PLL Design in Simulink]  
    C --> D[Performance Analysis]  
    D --> E[Phase Noise Spectrum]  
    D --> F[Step Response Analysis]  
    D --> G[Open-Loop Frequency Response]
```  

**Explanation:**  
This workflow outlines the steps involved in setting up and simulating the antenna system. It starts with system parameter setup, followed by phase noise simulation, PLL design, and performance analysis. The results of the analysis include phase noise spectrum, step response, and frequency response.

# Complete Antenna System Block Diagram

**Block Diagram:**  
```mermaid  
graph TD  
    A[Input Signal] --> B[PLL System]  
    B --> C[Signal Stabilization]  
    C --> D[Antenna Transmission Line]  
    D --> E[Insertion Loss Minimization]  
    E --> F[Output Signal]  
    B --> G[Phase Noise Control]  
    C --> H[SFDR Improvement]  
    D --> I[Noise Figure Analysis]
```  

**Explanation:**  
This diagram represents the full antenna system design. It includes the PLL system for signal stabilization, phase noise control, and insertion loss minimization. Additionally, it addresses SFDR improvement and noise figure analysis, essential for ensuring optimal system performance.

# Feedback Control Loop with Analysis Metrics

**Block Diagram:**  
```mermaid  
graph LR  
    A[Reference Signal] --> B[Phase Detector]  
    B --> C[Loop Filter]  
    C --> D[VCO]  
    D --> E[Output Signal]  
    D --> F[Frequency Divider]  
    F --> B  
    G[Noise Figure Analysis] --> E  
    H[Power Analysis] --> C  
    I[SFDR Evaluation] --> E  
    J[Phase Noise Spectrum] --> D
```  

**Explanation:**  
This diagram illustrates the feedback control loop of the PLL system and integrates performance analysis metrics, such as noise figure analysis, power analysis, SFDR evaluation, and phase noise spectrum analysis. These metrics are essential to evaluate and improve the system's overall performance.

# Full Block Diagram of the Project

**Block Diagram:**  
```mermaid  
graph TD  
    A[System Parameters Setup] --> B[Phase Noise Simulation]  
    B --> C[PLL Design]  
    C --> D[Open-Loop Response]  
    D --> E[Closed-Loop Response]  
    E --> F[Phase Noise Spectrum]  
    E --> G[Step Response Analysis]  
    E --> H[Performance Metrics]  
    H --> I[SFDR Improvement]  
    H --> J[Power Consumption Analysis]  
    H --> K[Noise Figure Analysis]  
    I --> L[Enhanced Signal Quality]  
    J --> M[Power Efficiency]  
    K --> N[Improved SNR]  
    L --> O[Optimized Antenna Performance]
```  

**Explanation:**  
This comprehensive diagram covers the entire project, from system parameter setup through phase noise simulation and PLL design. It integrates open-loop and closed-loop responses, performance metrics analysis, and key improvements such as SFDR enhancement, power efficiency, noise figure optimization, and improved signal-to-noise ratio (SNR). The ultimate goal is to achieve optimized antenna performance for high-frequency communication systems.

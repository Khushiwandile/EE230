# EE230

\documentclass[12pt]{article}
\usepackage{graphicx}
  
%
% Title[Enter title of the experiment here]
\title{EE230: Analog Circuits Lab\\ Lab No.}
% Author[Enter details of author here]
\author{Khushi Wandile, 22b1285}

% begin the document.
\begin{document}

% make a title page.[this creates title page]
\maketitle

%\textbf{ ** All experiment reports may not contain all fields in this format,This document is just for your reference**} 

\section{Time response of the RC circuits}
%**For each experiment a new section has to be created**
\subsection{Aim of the Expermiment}

Aim: To analyze the time response characteristics of an RC low-pass filter circuit. The specific objectives are as follows:\\
(a)Transient Response Analysis\\
(b)Bandwidth Determination\\
(c)Rise and Fall Time Analysis

\subsection{Design}

{Part(a):\\
Design a simple RC low-pass filter circuit and Used a square wave signal (V_{in1}) \ with:\\
5 Vpp,\ 2 ms period,\ 2.5 V \ DC \ offset\\

\begin{equation}
     \tau = R_{1} \times C_{1}
 \end{equation} \\
 Part(b):\\
Calculate the bandwidth as the reciprocal of the time constant and measured the bandwidth on the oscilloscope.\\

\begin{equation}
\text{Bandwidth (BW)} = \frac{1}{2\pi\tau} \label{eq:bandwidth}
\end{equation}
Part(c):\\
Used the 'Cursor' and 'Measure' function on the oscilloscope to measure rise and fall times.\\

}

 
     



%\textbf{this command prints text inside it in bold style}


\subsection{Simulation results}%[One more section] 

\subsubsection{Circuit Schematics}
\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{RC.jpg}
\end{figure}




\subsection{Experimental results}

Values used for the components: $R_1 = 1 \, \text{k}\Omega$ and $C_1 = 100 \, \mu\text{F}$.
\begin{table}[!hbt]
		% Center the table
		\begin{center}
		\caption{Time Constant}
		\begin{tabular}{|c|c|}
			% To create a horizontal line, type \hline
			\hline
			% To end a column type &
			% For a linebreak type \\
		     Calculated value & Measured value\\
			\hline
			100 us & 79.6 us\\
			\hline
            
		\end{tabular}
		\end{center}
\end{table}

\begin{table}[!hbt]
		% Center the table
		\begin{center}
		\caption{Bandwidth\\}
		\begin{tabular}{|c|c|}
			% To create a horizontal line, type \hline
			\hline
			% To end a column type &
			% For a linebreak type \\
		     Calculated value & Measured value\\
			\hline
			0.01 MHz & 0.0125 MHz\\
			\hline
            
		\end{tabular}
		\end{center}
\end{table}
\newpage
\begin{table}[!hbt]
		% Center the table
		\begin{center}
		\caption{Rise time and Fall time}
		\begin{tabular}{|c|c|c|}
			% To create a horizontal line, type \hline
			\hline
			% To end a column type &
			% For a linebreak type \\
			& Rise time & Fall time \\
			\hline
			using cursor & 171 us & 173 us \\
			\hline
			using measure & 162.5 us & 168.9 us  \\
			\hline
            
		\end{tabular}
		\end{center}
\end{table}
 \subsection{Conclusion and Inference}
The experiment demonstrated the transient response, bandwidth characteristics, and rise/fall times. The comparison between theoretical and measured values revealed insights into the circuit's behavior, highlighting the importance of accounting for practical considerations in circuit design and analysis.

\subsection{Experiment completion status}
I successfully completed the above sections of the lab

\newpage

\section{Frequency response of the RC circuits}

\subsection{Aim of the experiment}
{The aim of this experiment is to characterize the amplitude-frequency response (magnitude Bode plot) of an RC Low Pass Filter circuit by applying a sinusoidal input with varying frequencies.}
\subsection{Design}
Design a simple RC low-pass filter circuit and use a sine wave signal (\(V_{\text{in1}}\)):

\[ R_{1} = 1 \, \text{k}\Omega, \ C_{1} = 100 \, \text{nF}, \ (V_{\text{in1}} = \sin(\omega t)) \]

Steps involved:\\
1. Measure \(V_{\text{Outpp}}\) at different frequencies. Start measurements from 5 Hz, take more readings until 3 kHz, and then go to 1 MHz in a step of decades for \(V_{\text{outpp}}\) at different input frequencies\\
2. Plot the collected data in a rough amplitude-frequency response plot in notebook\\
3. Identify the frequency range where the output reaches 1/sqrt{2}
  times the amplitude of the input signal ie, the bandwidth of the circuit\\
  4. From the amplitude-frequency response plot, determine the measured bandwidth

\subsection{Simulation results}


\subsubsection{Circuit Schematics}


\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{RC.jpg}
\end{figure}

\subsubsection{Simulation results}
\begin{figure}[h!]
\centering
\includegraphics[scale = 0.6]{Bode_magnitude.jpg}
\end{figure}
This plot illustrates the designed RC low-pass filter's behavior. It shows how the output amplitude changes across a range of input frequencies from 5 Hz to 1 MHz. As expected, higher frequencies are attenuated, confirming the filter's low-pass nature. The -3 dB cutoff point indicates the frequency where the output starts to decrease significantly.


\subsection{Experimental results}
{Bandwidth measured from the Bode plot = 1.59 KHz}
\subsection{Conclusion and Inference}
{Simulation validates the efficacy of the designed RC low-pass filter, demonstrating effective attenuation of higher frequencies. The observed -3 dB cutoff frequency signifies the onset of this attenuation}
\subsection{Experiment completion status}{I successfully completed the above sections of the lab}

\newpage

\section{Basics of probing the circuit}

\subsection{Aim of the experiment}
{Demonstrate proper probing techniques for a potential divider circuit using a Digital Storage Oscilloscope (DSO)}
\subsection{Design}
Design a simple potential divider circuit with :

\[ R_{1} = 1 \text{k}\Omega \,R_{2} = 1 \text{k}\Omega\,R_{3} = 1 \text{k}\Omega

\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{pd.jpg}
\end{figure}

Design: Use Vdd = +15V, Vss = -15V, and 1KΩ resistors\\\\
Steps involved:\\
1. Measure voltage across R3 using DSO Channel 1, compare with expected value.\\
2.Measure voltage across R2 using DSO Channel 2 with Channel 1 across R3.\\
3. To avoid error in measurement we use Multimeter to measure voltage across R2 and R3\\
  4. Apply 5 Vpp sinusoidal input (4.7 KHz), Measure R2 voltage waveform using DSO

\subsection{Simulation results}
\newpage


\subsubsection{Circuit Schematics}
A simple potential divider circuit with :

\[ R_{1} = 1 \text{k}\Omega \,R_{2} = 1 \text{k}\Omega\,R_{3} = 1 \text{k}\Omega

\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{pd.jpg}
\end{figure}

Design: Use Vdd = +15V, Vss = -15V, and 1KΩ resistors


\subsubsection{Simulation results}

This plot illustrates the designed RC low-pass filter's behavior. It shows how the output amplitude changes across a range of input frequencies from 5 Hz to 1 MHz. As expected, higher frequencies are attenuated, confirming the filter's low-pass nature. The -3 dB cutoff point indicates the frequency where the output starts to decrease significantly.


\subsection{Experimental results}
{Expected and Measure values for voltages across R2 and R3\\
\begin{table}[!hbt]
		% Center the table
		\begin{center}
		\caption{Voltages measured using DSO channels\\}
		\begin{tabular}{|c|c|c|}
			% To create a horizontal line, type \hline
			\hline
			% To end a column type &
			% For a linebreak type \\
		     & Measured value & expected value\\
			\hline
			V_{R2} & 10.2V & 5V\\
                \hline
			V_{R3} & 0.001V & -5V\\
			\hline
            
		\end{tabular}
		\end{center}
  \end{table}\\
   After measuring Voltages using Multimeter, the measured values:\\\\
 [ V_{R2}= 5V, \ V_{R3}= -5V ]\\
 \newline
 Part(d):\\
  For Input Voltage : Sinusoidal voltage with 5 Vpp\, 4.7 KHz\\
  Expected output: Sinusoldal with 1.67 Vpp \, 4.7 KHz\\
  Obtained output: Sinusoidal with 1.68 Vpp \, 4.68 KHz

\subsection{Conclusion and Inference}
{Correct probing techniques with a Digital Storage Oscilloscope (DSO) yielded accurate measurements across R3. However, discrepancies in R2 measurements prompted use of instruments like a high-precision multimeter. \\\\Sinusoidal input analysis revealed variations, possible sourses of error are:\\
1. Electronic noise affecting signal integrity during measurements\\
2. Impedance mismatch between the circuit and measurement instruments causing loading effects\\
3. Variations in resistor values from their specified tolerances}
\subsection{Experiment completion status}{I successfully completed the above sections of the lab}

\newpage

\section{Half wave Rectifier}

\subsection{Aim of the experiment}
{Investigate the behavior of a half-wave rectifier circuit with a sinusoidal input by plotting input and output waveforms and observe the impact of changing diode polarity on rectification.}
\subsection{Design}
Half-wave rectifier circuit with a resistor R = 22 

\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{pd.jpg}
\end{figure}

Design: Use Vdd = +15V, Vss = -15V, and 1KΩ resistors\\\\
Steps involved:\\
1. Measure voltage across R3 using DSO Channel 1, compare with expected value.\\
2.Measure voltage across R2 using DSO Channel 2 with Channel 1 across R3.\\
3. To avoid error in measurement we use Multimeter to measure voltage across R2 and R3\\
  4. Apply 5 Vpp sinusoidal input (4.7 KHz), Measure R2 voltage waveform using DSO

\subsection{Simulation results}
\newpage


\subsubsection{Circuit Schematics}
A simple potential divider circuit with :

\[ R_{1} = 1 \text{k}\Omega \,R_{2} = 1 \text{k}\Omega\,R_{3} = 1 \text{k}\Omega

\begin{figure}[h!]
\centering
\includegraphics[scale = 0.4]{pd.jpg}
\end{figure}

Design: Use Vdd = +15V, Vss = -15V, and 1KΩ resistors


\subsubsection{Simulation results}

This plot illustrates the designed RC low-pass filter's behavior. It shows how the output amplitude changes across a range of input frequencies from 5 Hz to 1 MHz. As expected, higher frequencies are attenuated, confirming the filter's low-pass nature. The -3 dB cutoff point indicates the frequency where the output starts to decrease significantly.


\subsection{Experimental results}
{Expected and Measure values for voltages across R2 and R3\\
\begin{table}[!hbt]
		% Center the table
		\begin{center}
		\caption{Voltages measured using DSO channels\\}
		\begin{tabular}{|c|c|c|}
			% To create a horizontal line, type \hline
			\hline
			% To end a column type &
			% For a linebreak type \\
		     & Measured value & expected value\\
			\hline
			V_{R2} & 10.2V & 5V\\
                \hline
			V_{R3} & 0.001V & -5V\\
			\hline
            
		\end{tabular}
		\end{center}
  \end{table}\\
   After measuring Voltages using Multimeter, the measured values:\\\\
 [ V_{R2}= 5V, \ V_{R3}= -5V ]\\
 \newline
 Part(d):\\
  For Input Voltage : Sinusoidal voltage with 5 Vpp\, 4.7 KHz\\
  Expected output: Sinusoldal with 1.67 Vpp \, 4.7 KHz\\
  Obtained output: Sinusoidal with 1.68 Vpp \, 4.68 KHz

\subsection{Conclusion and Inference}
{Correct probing techniques with a Digital Storage Oscilloscope (DSO) yielded accurate measurements across R3. However, discrepancies in R2 measurements prompted use of instruments like a high-precision multimeter. \\\\Sinusoidal input analysis revealed variations, possible sourses of error are:\\
1. Electronic noise affecting signal integrity during measurements\\
2. Impedance mismatch between the circuit and measurement instruments causing loading effects\\
3. Variations in resistor values from their specified tolerances}
\subsection{Experiment completion status}{I successfully completed the above sections of the lab}

** Add more experiments section (on new page) if applicable**

\end{document}


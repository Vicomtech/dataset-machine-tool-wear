This dataset contains the data captured in a machine tool process (turning process) and includes data from the control system, sensors and tool flank wear.
Data corresponding to 13 diferent tools was acquired and segmented into N segments of 1 s. The total number of considered segments is equal to the number of rows in the dataset, i.e. 2054.	
Different features were extracted from each of the segments and the flank wear, i.e. Vb, of each tool was calculated.	
"A schematic representation of the turning process, location of sensors and signal processing is reported in ""Tool remaining useful life prediction using bidirectional recurrent neural networks (brnn)"". The International Journal of Advanced Manufacturing Technology, 125(9-10):4027–4045, 2023"	
	
Signal	Description
AE	Acoustic emissions
Ax1, Ay1, Az1	Triaxial accelerometer 1
Ax2, Ay2, Az2	Triaxial accelerometer 2
F_f	Feed force
F_c	Cutting force
F_p	Radial force
Iu_s, Iv_s	Currents of spindle motor
Iu_x, Iv_x	Motor currents in x-axis
Vu_s, Vv_s, Vw_s	Voltage of spindle motor
Vu_x, Vv_x, Vw_x	Motor voltage in x-axis
Micro	Microphone
TV50.S	Mechanical power of spindle motor
TV51.S	Electrical power of spindle motor
TV2.S	Torque of spindle motor
TV2.X, TV2.Z	Motor torque
CV3.S	Electrical current of spindle motor
CV3.X, CV3.Z	Electrical current in x-axis and z-axis
CON.SV2.S	Spindle speed (encoder)
CON.SV2.X, CON.SV2.Z	Speed in x-axis and z-axis (encoder)
CON.G.FREAL	Programmed feed (CNC)
CON.A.SREAL.S	Programmed spindle speed (CNC)
Tool	Tool ID
Vb	Flank wear
	
For each signal, the following five values were extracted:	
Feature	Description
MEAN	The sum of a group of numbers divided by the amount of numbers of that collection
RMS	The square root of the mean square (the arithmetic mean of the squares of a set of numbers)
MAX	The maximum value of a group of numbers
SK	Skewness is a measure of symmetry in a distribution
KURT	Kurtosis is a measure of the “tailedness” of the probability distribution of a variable
	
Regarding the acoustic emission signal, however, the following features were extracted:	
RMS	The square root of the mean square (the arithmetic mean of the squares of a set of numbers)
MAX	The maximum value of a group of numbers
KURT	Kurtosis is a measure of the “tailedness” of the probability distribution of a variable
VAR	Variance is the sum of squared differences from the mean divided by number of elements
C_0.1	Number of times that the amplitude of the signal exceeds a predefined threshold - 0.1 V
C_0.15	Number of times that the amplitude of the signal exceeds a predefined threshold - 0.15 V
CF	Crest Factor is the peak amplitude of the waveform divided by the RMS value of the waveform

We extend our gratitude to Mondragon Universitatea for generously providing the facilities and the raw data of which this dataset is derived.
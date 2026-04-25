# Higher-Rates
paper code

1. HF_Q.zip corresponds to the original erroneous version, in which the coning angle was not converted to radians under the dynamic coning environment.
2. HF_final.zip is the final revised version, where the coning angle is correctly converted into radians in the dynamic coning environment.


Since the coning data contains multiple coning angles and covers a duration of one hour, the overall file size is large. The data is split into four compressed packages for upload: coin_data1.zip, coin_data2.zip, coin_data3.zip, and coin_data4.zip.
Please decompress all four archives and place the extracted files into the directory:`HF_final\Q_Coin\coin_data`

First, we introduce the common components of the two algorithms:
The Algorithm folder contains attitude algorithms, namely:
Ser_exp (TS)
Sec_order4 (SO4)
Sec_order (SO2)
HR_RK (Runge-Kutta algorithm, not included in this paper)
Hig_Rate (HR)
Fun_iter (FI)

The utils folder stores auxiliary functions for multiple algorithms, including auxiliary functions for attitude computation and error analysis functions.

The config.m script serves as a common parameter configuration file, which defines the simulation duration, error parameters, and plotting parameters.Note that MATLAB plotting is only for demonstration purposes; all simulation results are exported to Excel format and subsequently plotted using OriginPro.

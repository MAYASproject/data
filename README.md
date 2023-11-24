# data
PCG, BCG raw data. 
The files contain the signals of phonocardiogram, ballistocardiogram, in numpy format.

Use the file called BCG_PCG.zip please search for this file in the repository
unzip in your system.

For example for the files called 1_Act_134.0_S1.npy and 1_Act_134.0_S1.npy 
 1_Act_134.0_S1.npy contains the PCG
1_Act_134.0_S2.npy contains the BCG
134 is the pressure

this is the code to see the signals:

import numpy as np
import matplotlib.pyplot as plt
PCC=np.load('1_Act_134.0_S1.npy')
print(PCC.shape)
plt.subplot(2,1,1)
plt.plot(PCC[0:1500])

BCC=np.load('1_Act_134.0_S2.npy')
print(BCC.shape)
plt.subplot(2,1,2)
plt.plot(BCC[0:1500])

plt.show()


If you want to use the data, please cite

RafaelGonzalez‑Landaeta, Brenda Ramirez & Jose Mejia. Estimation of systolic blood pressure by Random Forest using heart sounds and a ballistocardiogram. Scientifc Reports, (2022) 

Rafael Gonzalez‑Landaeta & Jose Mejia, "M.A.Y.A.S Project: Creation of a database of physiological signals. Estimation of changes in blood pressure.", UACJ Institutional Repository, 2022


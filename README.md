# DESIGN OF DIFFERENTIAL INPUT SINGLE ENDED OUTPUT SINGLE STAGE AMPLIFER
Design and implementation of a differntial input single ended output single stage amplifier using tsmc 180nm semiconductor technology. Achieved required gain, bandwidth through simulations. 
### 1.Design specification:
To design a differential-input single-ended output Single-Stage amplifier, using CMOS 180nm technology. The amplifier is powered from a 1.8V power supply. The amplifier to have one current source with a capacitive load as 10pF.
| Design Parameter| Specification Value| 
| :---:  | :-: |
| Slew rate| =5V/us|
| Unity Gain Bandwidth| >=5MHz|
| Gain (Av)| >=40db|
| Load capacitance (CL)|=10Pf|
| Power dissipiation |<=0.3mw|
|ICMR+|=1.6V|
|ICMR-|=0.8v|

### 2.ltspice circuit:

<img width="626" alt="differential amplifier circuit" src="https://github.com/user-attachments/assets/00baabdd-6011-44a2-b255-37279971a9d1" />

### 3. Design Process:

* W/L ratio of M3 and M4 is found using ICMR+.
* W/L ratio of M1 and M2 is found using GBW.
* Iref current is found using slew rate.
* W/L ratio of M5 is found using ICMR-.
* W/L ratio of M6 will be same as M5.

### 3. Simulations:
The input is applied differentailly. Following is the simulation of input and ouput voltage
<img width="719" alt="differntai amplifier input and utput voltage" src="https://github.com/user-attachments/assets/19df4372-a7c5-4b46-8a4c-850f88283829" />

The freqency response is shown below:
<img width="787" alt="frequency response" src="https://github.com/user-attachments/assets/c8cab667-14b2-45c9-9807-b9ca8c22b041" />

### 3. Simulations:

From the Simulation we can observe that the gain of the circuit is approximately 36db and gain bandwidth product is approximately 4.44KHz, which are very near to our design specifications.









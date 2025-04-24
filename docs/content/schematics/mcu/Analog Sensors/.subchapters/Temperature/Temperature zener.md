
# LMx35

Datasheets from [STMicroelectronics](https://www.st.com/resource/en/datasheet/lm135.pdf) and [Texas Instruments](https://www.ti.com/lit/ds/symlink/lm335.pdf)

![](images/render/kicad/LMx35.svg)

This sensor is powered with current, not voltage and `R1` should be chosen to limit current through the sensor within 0.4 ... 5 mA range.

The measures temperature is converted into voltage with scale factor of 10 mV/°K, which also requires extra conversion into Celsius.

And, of course, the current depends on supply voltage and measured temperature. 

The expected output voltages at operating ranges are:

| Sensor                              |               | LM135        | LM235        | LM335        |
| ----------------------------------- | ------------- | ------------ | ------------ | ------------ |
| Temperature range, [°C]             |               | -55 ... +150 | -40 ... +125 | -40 ... +100 |
| Voltage at lowers temperature, [V]  | $V_{T_{min}}$ | 2.1815       | 2.3315       | 2.3315       |
| Voltage at highest temperature, [V] | $V_{T_{max}}$ | 4.2315       | 3.9815       | 3.7315       |

It exceeds  the highest limit of STM32 ADC, and limit the measurement down to 56.85°C if powered from 5V and also requires to add safety 3.6V zener to protect the ADC.


Estimation of `R1` can be done:

$$
R1_{max}= \frac{\Delta V_{min}}{I_{min}}=\frac{V_{supply}-V_{T_{max}}}{I_{min}}
$$

$$
R1_{min}= \frac{\Delta V_{max}}{I_{max}}=\frac{V_{supply}-V_{T_{min}}}{I_{max}}
$$

Thus, for 5V supply and limited 3.3V ADC output, 1K resistor would suffice.
# ADC

Thus, to read and calculate voltage at sensor output pin:

$$
V_{input}=\frac{ADC_{input}}{ADC_{resolution}} \times V_{ref}
$$

where: 

- $ADC_{input}$– voltage level at analog input pin
- $ADC_{resolution}$ – resolution range of certain microcontroller or ADC converter. Can be calculated as: $$ADC_{resolution}=2^{bits}-1$$
- $bits$ – ADC resolution digits of certain microcontroller. For many STM32 equals to 12.
- $V_{ref}$ – reference voltage level. 

So, the measured is roughly equal to:

$$
V_{input}=\frac{ADC_{input}}{2^{12}-1} \times 3.3 = ADC_{input} \times 0.000806 [V]=ADC_{input} \times 0.806 [mV]
$$

Which also mean that we can read the voltage with resolution of 0.806 mV.
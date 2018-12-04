# Vaja1-ADC-single-conversion-STM32F0
single conversion
-------------------------------------------------
ODGOVORI:
2.)
B. PC0
C. 1 ADC pretvornik
D. Da je določeni pin že zaseden;
Odpravimo napako tako da obkljukamo željeni pin v ADC zavihku… npr. IN10=PC0
e.)16 ADC + 2 Druga
f.)ADC_IN10
H) 
1. 12-Bit, 0-4095
2. 6-Bit, 0-63
3. 10-Bit, 0-1023
----------------------------------------------
Komentar:
v Serial code begin 1 sem moral dodati GPIO_PinState potenciometer;. V user code begin 3 pa sem še dodal potenciometer=HAL_GPIO_ReadPin(GPIOC, GPIO_PIN_10); da mi je lahko sploh bralo vrednosti iz potenciometra. Potem je program deloval.

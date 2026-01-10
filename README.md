# Cross-Chip_MixPincer

## Dataset

We established the  Cross-Chip dataset covering architectures from the 8-bit AVR-based Atmel XMEGA to the 32-bit ARM Cortex-M family, including the STM32F0 (Cortex-M0), STM32F1 (Cortex-M3), and STM32F3 (Cortex-M4). Utilizing the ChipWhisperer capture platform, we acquire power traces from each target device executing an AES-128 algorithm implementation called tiny-AES-c, where each device operates under a different fixed encryption key. The dataset for each platform consists of 60,000 traces, partitioned into 50,000 for profiling and 10,000 for test. Each trace comprises 1,000 sample points, corresponding to the power consumption segment covering the S-box substitution in the first round of AES-128. We use the HW of the S-box output as the label.


## Framework

we provide test codes of our framework in 'MixPincer_test.py' and a model instance in the folder 'model'.

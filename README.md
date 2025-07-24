# Ring_Oscillator

**Under the guidance of Professor Nagendra Krishnapura, IIT Madras**

## Software and PDK used : Cadence Virtuoso and TSMC 65nm PDK

Used 11 Inverters to design the Oscillator.

The CMOS inverters used : https://github.com/arkaprabhapal/CMOS-inverter

**Tested for both L and 5L channel length mosfets (L = 150um)**

## 1. Schematic
<img width="941" height="243" alt="image" src="https://github.com/user-attachments/assets/9d4fda8a-c3fb-4585-a9c0-c6e777114bc4" />

## Input, Output Waveforms :
<img width="965" height="737" alt="image" src="https://github.com/user-attachments/assets/bbe3cef1-4818-4209-a0dc-e6a8686383ea" />

<img width="943" height="508" alt="image" src="https://github.com/user-attachments/assets/48a0ecb9-9804-4486-aae4-02e669b9b551" />

## PSS Analyses Table :

|                      | Length = L   | Length = 5L   |
|----------------------|--------------|---------------|
| Oscillation Frequency| 1.725557 GHz | 137.1709 MHz  |
| Average Power        | 12.904 mW    | 12.8625 mW    |
| Average Current      | 41.6077 µA   | 11.191 µA     |

**PSS Waveforms for L :-**

<img width="1046" height="447" alt="image" src="https://github.com/user-attachments/assets/dc3aa87e-7acd-4d71-b2dd-d621aa4768bc" />
<img width="1132" height="427" alt="image" src="https://github.com/user-attachments/assets/db9bf1bc-0c2a-49d5-a902-7b98566ce50e" />
<img width="235" height="126" alt="image" src="https://github.com/user-attachments/assets/04c5c121-add3-4c9f-9383-77caec61e2c7" />

**PSS Waveforms for 5L :-**
<img width="1367" height="471" alt="image" src="https://github.com/user-attachments/assets/82bb3bb3-df93-4e16-a0d5-c5554b8ed3fc" />


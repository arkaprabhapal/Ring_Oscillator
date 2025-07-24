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

## 2. Corner Analysis (For Schematic and Layout)
_The Layout results are obtained by selecting the view as extracted results instead of the schematic view in the config file._

# 📊 Performance Metrics Comparison

This section documents a comparison of performance metrics observed from both schematic and layout simulations across different PVT corners.

## 🧪 Schematic Results

| MOS | VDD (V) | Temp (°C) | Oscillation Frequency | Avg Current (µA) | Avg Power (mW) |
|-----|---------|-----------|------------------------|------------------|----------------|
| tt  | 1.2     | 50        | 1.694 GHz              | 40.2345          | 12.89          |
| ff  | 1.3     | 0         | 2.393 GHz              | 65.1074          | 15.07          |
| ss  | 1.1     | 100       | 1.172 GHz              | 24.0606          | 10.87          |

## 🧱 Layout Results

| MOS | VDD (V) | Temp (°C) | Oscillation Frequency | Avg Current (µA) | Avg Power (mW) |
|-----|---------|-----------|------------------------|------------------|----------------|
| tt  | 1.2     | 50        | 995.4 MHz              | 33.9183          | 12.8536        |
| ff  | 1.3     | 0         | 1.458 GHz              | 55.82            | 15.023         |
| ss  | 1.1     | 100       | 661.4 MHz              | 19.88            | 10.84          |

---

## 3. After simulating the Ring Oscillator with extraction of one single CMOS Inverter, I made the entire layout of CMOS inverter and simulated and compared the results. 

<img width="1567" height="438" alt="image" src="https://github.com/user-attachments/assets/448ad975-35ac-413b-9f83-6a172512c9c4" />

<img width="1168" height="406" alt="image" src="https://github.com/user-attachments/assets/f97c79a1-d0d5-4a6e-8e4f-2813bb6429f9" />

<img width="967" height="731" alt="image" src="https://github.com/user-attachments/assets/1af00740-0497-471f-9778-36cd05bfc954" />

**Results obtained :-**
<img width="1166" height="230" alt="image" src="https://github.com/user-attachments/assets/e5bcc633-a5d1-4080-9611-ccb98a8f92a6" />

## 🧱 Layout Simulation Data

| mos        | VDD | T   | Layout                                                                 |
|------------|-----|-----|------------------------------------------------------------------------|
|            |     |     | oscillation frequency | average current (µA) | average power (mW)      |
| Nominal    | 1.2 | 27  | 1.00617 GHz           | 36.51               | 12.613                  |
| 1 (tt)     | 1.2 | 50  | 970.4 MHz             | 35.34               | 12.59                   |
| 2 (ff)     | 1.3 | 0   | 1.416 GHz             | 57.896              | 14.69                   |
| 3 (ss)     | 1.1 | 100 | 648 MHz               | 20.857              | 10.63                   |

---


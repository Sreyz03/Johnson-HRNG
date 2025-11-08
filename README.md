# Johnson-Nyquist Noise-Based Hardware Random Number Generator (HRNG)

This repository contains the implementation, analysis, and documentation for a **Johnson–Nyquist Noise-Based Hardware Random Number Generator (HRNG)** designed for **secure server load balancing** and **entropy generation**.  
The project focuses on using naturally occurring thermal noise as a high-entropy source to achieve true randomness for cryptographic and distributed computing systems.

---

## 📁 Repository Structure

Johnson-HRNG/
│
├── Entropy As A Service/
│ └── EaaS.pdf
│
├── Server Load Balancer/
│ └── Server.py
│
├── .gitignore
├── Abstract.pdf
├── Arduino -v2.ino
├── Final_with_histogram.ipynb
├── UART_Transmission.ino
├── final_ppt.pptx
└── main.py


---

## ⚙️ File Descriptions

### 🧩 Hardware and Firmware
- **Arduino -v2.ino** — Main Arduino sketch for reading analog noise signals and transmitting digitized random data.  
- **UART_Transmission.ino** — Handles serial (UART) communication between the Arduino/microcontroller and the PC for random data transfer.  

### 💻 Software and Processing
- **main.py** — Python script for receiving and analyzing the random data stream. Can also be extended for TRNG-based simulations.  
- **Final_with_histogram.ipynb** — Jupyter Notebook for data visualization, randomness histogram generation, and post-processing (e.g., whitening).  
- **Server Load Balancer/Server.py** — Implements a TRNG-based load balancing algorithm to distribute server requests using true random sequences.

### 📄 Documentation
- **Abstract.pdf** — Concise project summary and problem statement.  
- **final_ppt.pptx** — Final presentation slides detailing the design, methodology, and results.  
- **Entropy As A Service/EaaS.pdf** — Reference or concept document discussing randomness distribution over networks.

### ⚙️ Configuration
- **.gitignore** — Specifies files and directories to be ignored by Git (e.g., build files, temporary logs, IDE configs).

---

## 🧪 Project Overview

This project generates **true random numbers** by capturing **Johnson–Nyquist noise** — the natural thermal noise across resistors — using analog circuitry.  
The analog noise signal is:
1. Amplified via an instrumentation amplifier  
2. Filtered using a band-pass network  
3. Digitized using an ADC  
4. Transmitted to a computer for analysis or random-based decision making  

The Python and Jupyter scripts process and validate the randomness statistically and demonstrate a **TRNG-based server load balancer** for improved security and fairness.

---

## 🧰 Applications

- Cryptographic key generation  
- Secure server load balancing  
- OTP and CAPTCHA generation  
- Entropy-as-a-Service (EaaS) systems  
- Randomized scheduling in distributed systems  

---

## 👥 Authors

- Sreyas Kishore T  
- Muhammed Midlaj M P  
- Mohammed Suhail K M  
- Vaishnav U  

---

## 🧾 License

This project is released under the **MIT License**.  
You are free to use, modify, and distribute the code with proper attribution.

---



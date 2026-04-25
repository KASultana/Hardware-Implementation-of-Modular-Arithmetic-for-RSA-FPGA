# Hardware Implementation of Modular Arithmetic for RSA-FPGA

VHDL-based RSA modular arithmetic and 16-bit RSA core implemented on a **Basys-3 FPGA**.

## 📝 Description
This project implements the core modular arithmetic blocks required for the RSA cryptosystem in hardware. Developed as part of the **SE520 Laboratory** at **Grenoble INP – Esisar**, the project includes modular addition, modular multiplication, and MSB-first modular exponentiation, all designed in VHDL and verified using self-checking testbenches.

The arithmetic blocks are integrated into a complete 16-bit RSA encryption/decryption core deployed on the Basys-3 FPGA. The project also demonstrates a hardware brute-force attack on a small RSA key space, highlighting the importance of large key sizes in public-key cryptography.

## 📂 Repository Structure
The project is organized into sequential tasks reflecting the lab progression:
- **Task 1:** Behavioral and RTL descriptions of the **Modulo $m$ Adder**.
- **Task 2:** Implementation of the **Modulo $m$ Multiplier** using an MSB-based algorithm.
- **Task 3:** Development of the **Modulo $m$ Exponentiation** block.
- **Task 4.1:** Integration of the **RSA Core** with Basys-3 peripherals (Switches, Buttons, and 7-segment display).
- **Task 4.2:** Implementation of a **Brute-force attack** block to find 16-bit RSA private keys.

## 🛠️ Technologies & Tools
- **Language:** VHDL
- **Hardware:** Basys-3 Board (Xilinx Artix-7 FPGA)
- **Software:** Vivado / ModelSim

## 🚀 How to Use
1. **Simulation:** Verify the correctness of each arithmetic block using the provided testbenches (e.g., `tb_modm_adder.vhd`).
2. **Implementation:** Synthesize the design and flash the bitstream onto the Basys-3 board using Vivado.
3. **Hardware Testing:** - Use **Switches** to toggle between Cleartext/Cryptotext and Encryption/Decryption modes.
   - The result is displayed in hexadecimal on the **4-digit 7-segment display**.

## 👥 Contributors
- **Kazi Aklima Sultana** — [@KASultana](https://github.com/KASultana)
- **Thomas Ibrahim** — [@tomehabb](https://github.com/tomehabb)

**Supervised by:** Prof. Yann Kieffer, Grenoble INP – Esisar.

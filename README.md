# SPI Communication (MOSI Only) - 12 Bits Data Transfer (Verilog)

This project demonstrates SPI communication between a master and a slave, using only the **MOSI (Master Out Slave In)** line for the transfer of 12 bits of data. The communication is written in **Verilog** and simulated using **Xilinx Vivado**. Synchronization is handled through **SCLK (Serial Clock)**, and a **Done** signal is generated to indicate the completion of the data transfer.

## Project Overview

- **Master** sends 12-bit data to the **Slave** over the MOSI line.
- Data synchronization between Master and Slave is achieved using the **sclk** clock signal.
- A **done** signal is generated after the transmission of the 12 bits is complete to indicate successful communication.

## Features

- **mosi-only communication**: Only the MOSI line is used for data transfer.
- **12-bit data transfer**: The master transmits 12 bits of data at a time.
- **Synchronization via SCLK**: Data is synchronized using the SCLK (Serial Clock) signal.
- **Done Signal**: A signal that indicates when the transmission is complete.

## Simulation Details

- **Xilinx Vivado**: The project is implemented using Xilinx Vivado, and all testing is done via simulation.
- **Verilog**: The SPI communication logic is written in Verilog.
- **Testbench**: A testbench is used to simulate and verify the communication with different test cases to ensure reliable data transfer.
  
## How It Works

1. The Master initiates the communication by sending 12 bits of data to the Slave via the **mosi** line.
2. The **sclk** signal ensures that the Slave is synchronized with the Master during data transmission.
3. Once the 12 bits are successfully transmitted, a **done** signal is asserted to indicate the completion of the transmission.

## Simulation

This project has been verified through simulation in Xilinx Vivado. Different test cases were created in the testbench to validate the communication under various scenarios, ensuring that the 12-bit transfer is correctly handled and synchronized between the Master and Slave.

## Waveform

![SPI_Simulations](https://github.com/user-attachments/assets/42daa783-b95c-4f40-8b9f-7632d53a4023)

# Glossary – DAQ & Trigger Units 
(From CAEN website https://www.caen.it/support-services/daq-trigger-units/)

---

## A

- **ADC Conversion Time**  
  The time required, after the sample command, to digitize the analog signal.

- **ADC Dead Time**  
  The minimum amount of time required after the end of a GATE to have the ADC ready for a new acquisition.

- **ADC Resolution**  
  The number of bits in which the ADC full-scale range is divided.

- **Address Modifier**  
  Code that carries information about the size and type of VME data transfer.

- **Analog Adder**  
  A linear Fan-In.

- **AND**  
  Logical designation or circuit function meaning that all inputs must be in the TRUE state for a TRUE output.

- **Anti-Coincidence**  
  An input signal which suppresses the normal functioning of the unit for the duration of its application.

---

## B

- **Backplane**  
  A monolithic, multilayer printed circuit board at the rear of a crate providing bus dataway, power lines, and modules' connectors.

- **Bandwidth**  
  The frequency range over which the gain of an amplifier or other circuit does not vary by more than 3 dB.

- **Baseline Restorer**  
  A circuit that maintains the amplifier DC output (baseline) at a fixed potential independently from the counting rate.

- **Baseline Shift**  
  Drift of the amplifier DC level (baseline) that may impair peak amplitude stability.

- **Block Transfer (BLT32)**  
  A 32-bit VME data transfer from/to a series of adjacent locations of a module.

- **Bridged Outputs**  
  Parallel output connections that share the same driver.

---

## C

- **CAMAC**  
  Computer Automated Measurement And Control; an international standard of modular instrumentation defined by the ESONE Committee of the JNRC.

- **CANbus**  
  Controlled Area Network; a network consisting of multiple microcontrollers that need to communicate with each other.

- **Chained Block Transfer (CBLT)**  
  Sequential readout of multiple VME slave modules selected by a single address cycle.

- **Charge ADC**  
  An ADC which measures the input charge integrated during the GATE period.

- **Charge Sensitive Preamplifier**  
  A preamplifier whose peak output amplitude is directly proportional to the input integrated charge.

- **Coincidence Unit**  
  A device that performs the AND logic function of two or more inputs.

- **Common Mode Range**  
  The maximum range (usually voltage) within which differential inputs can operate without a loss of accuracy.

- **Common Mode Rejection Ratio (CMRR)**  
  The ratio between the common mode input noise and the output voltage, expressed in dB. It indicates the ability to reject common mode noise.

- **Common Start**  
  A signal common to all input channels marking the beginning of a time interval measurement in a TDC.

- **Common Stop**  
  A signal common to all input channels marking the end of a time interval measurement in a TDC.

---

## D

- **Daisy Chain**  
  Connection of control signals on several boards in a chain.

- **DC Level Shift**  
  A programmable DC Offset.

- **Differential Input**  
  A circuit that is sensitive to the algebraic difference between the IN+ and IN- input signals.

- **Differential Non-Linearity**  
  The maximum deviation of the ADC bin widths from a flat distribution, expressed as a percentage.

- **Dual Port Memory**  
  A memory module with two interfaces for data transfer.

- **Dwell Time**  
  The trigger generation period of the internal programmable timer of a MultiChannel Scaler.

---

## E

- **ECL**  
  Emitter-Coupled Logic, a non-saturated logic performed by emitter-coupled transistors.  

  - LOGICAL 0 = LOW = -1.75 V  
  - LOGICAL 1 = HIGH = -0.9 V  

- **Event Counter**  
  A counter indicating the number of trigger signals processed by a DAQ module.

---

## F

- **Fall Time**  
  The time required for a pulse to decrease from 90% to 10% of its full amplitude.

- **Fan-In**  
  Mixing of more than one input to obtain outputs:
  - **Linear**: The algebraic sum of the inputs.
  - **Logic**: The logical OR of the inputs.

- **Fan-Out**  
  Reproduction of an input signal on multiple outputs.

- **FWHM**  
  Full Width at Half Maximum: the width of a pulse or waveform at 50% amplitude.

---

## G

- **GATE**  
  An input control signal used to enable the passage of other signals.

- **Geographical Addressing**  
  Addressing a module based on its physical location (slot number) in a crate.

- **Ground Loop**  
  A low impedance path along which voltage drops occur due to external pickup.

---

## H

- **High Speed CAENET**  
  A CAEN proprietary 1 Megabit/second serial transmission protocol.

---

## I

- **Inhibit**  
  A signal or switch preventing a unit from operating or responding to inputs.

- **Integral Non-Linearity**  
  Maximum deviation (expressed as a fraction of full scale) of ADC response from a straight line fit.

---

## J

- **JAUX**  
  A 3-row, 30-pin connector in a VME V430 compliant backplane for various power lines and geographical address connections.

---

## L

- **Latch**  
  Memory register.

- **Leading Edge Discriminator**  
  Delivers a logic pulse for each input signal larger than a programmable threshold.

- **Live Insertion**  
  The possibility of inserting (or removing) a board into the crate without switching it off.
  
- **Low Threshold Discriminator**  
  A Leading Edge Discriminator with high sensitivity on small signals.

- **LSB**  
  Least Significant Bit.

- **LVDS**  
  Low Voltage Differential Signaling (specified in the IEEE 1596.3 standard), it’s a way to communicate data using a very low voltage swing (about 350 mV) over balanced connections.

--- 

## M

- **Majority Logic**  
  Generates a TRUE output when the number of coincident inputs is equal to or greater than a specified threshold.

- **Master**  
  A device capable of controlling the data transfer operation according to some protocol.

- **MBLT64**  
  Multiplexed Block Transfer; similar to BLT but transfers 64-bit words instead of 32-bit ones.

- **Multicast Mode (MCST)**  
  Allows commands to be sent to a chosen set of VME slave modules in a single data transfer bus transaction.

- **Multichannel Scaler**  
  A scaler with independent channels and a periodic programmable trigger to record counting rates as a function of time.

- **Multievent Buffer**  
  A FIFO-like buffer for storing/reading data from multiple triggers.

- **Multihit TDC**  
  A TDC that can accept multiple hits per channel.

---

## N

- **NAND**  
  A complementary output AND circuit.

- **NIM (Nuclear Instrumentation Module)**  
  International standard of modular instrumentation defined by the U.S. NIM Committee.  
  - Modules have a minimum standard width of 1.35 inches, height of 8.75 inches, and depth of 10 inches.  
  - Can be built in double-width, triple-width, etc.

- **NIM Logic Levels**  
  - **Inputs**:  
    LOGICAL 1 = -12 to -32 mA, or 600 mV to 1.6 V into 50 Ohm.  
    LOGICAL 0 = < +2 mA or <100 mV into 50 Ohm.  
  - **Outputs**:  
    LOGICAL 1 = -14 to -32 mA, or 700 mV to 1.6 V into 50 Ohm.  
    LOGICAL 0 = < +2 mA or <100 mV into 50 Ohm.

- **Non-Updating Discriminator**  
  A discriminator whose output must return to zero before retriggering can occur.

- **NOR**  
  A complementary output OR circuit.

---

## O

- **OR**  
  A logic circuit where the output is TRUE if at least one input is TRUE.

- **Overflow Suppression**  
  A digital technique to skip "out of range" values from memory.

---

## P

- **PAUX**  
  A 3-row, 30-pin connector in VME V430 compliant boards that mates with the JAUX connector.

- **Peak Sensing ADC**  
  An ADC that measures the peak amplitude of waveforms within the GATE period.

- **Pedestal**  
  The ADC value readout when no input signal is present.

- **Pile-Up**  
  Overlapping of amplifier output signals due to excessive count rate.

- **Pole Zero Cancellation**  
  A circuit eliminating the undershoot of semi-Gaussian shaped output pulses.

- **Power Supply Rejection**  
  Ability of a device to reject the effects of power supply variations.

- **Programmable Logic Unit**  
  A module that accepts inputs and generates logic combinations of the inputs based on programmed operations.

---

## Q

- **QDC**  
  Charge ADC.

---

## R

- **Reflection Coefficient**  
  The amount of signal amplitude reflected by an input due to impedance mismatch.

- **Rise Time**  
  Time required for a pulse to grow from 10% to 90% of its full amplitude.

- **RMS**  
  The square root of ⟨(X - ⟨X⟩)²⟩, where X is a random variable and ⟨⟩ denotes the average.

---

## S

- **Sample and Hold**  
  A circuit that samples and holds the instantaneous amplitude of an input signal on command.

- **Sampling ADC**  
  A device that samples an input waveform at specified time intervals, digitizes the analog values, and stores the results in digital memory.

- **Scaler**  
  Counter.

- **Semi-Gaussian Shaping**  
  A pulse shape resembling a Gaussian curve obtained using CR-(RC)ⁿ filters with equal time constants.

- **Shaping Amplifier**  
  Shapes output pulses from a charge-sensitive preamplifier to improve S/N ratio and minimize pile-up risks (commonly used in energy spectroscopy).

- **Shaping Time**  
  Time constant of a shaping amplifier filter.

- **Single-Ended Signal**  
  A ground-referenced signal.

- **Sliding Scale Technique**  
  A technique to reduce ADC differential non-linearity.

---

## T

- **TAC**  
  Time-to-Amplitude Converter.

- **TDC**  
  Time-to-Digital Converter.

- **Translator**  
  A device that converts logical signals from one standard to another (e.g., TTL to ECL).

- **TTL**  
  Transistor-Transistor Logic.  
  - Logical 0: 0 to 0.8 V.  
  - Logical 1: 2.0 to 5.0 V.

---

## U

- **Updating Discriminator**  
  A discriminator that can be retriggered before the output returns to zero.

---

## V

- **V430**  
  A VMEbus compatible crate type with extra JAUX connectors for power and geographical addressing.

- **Veto**  
  Inhibit.

- **VME (Versa Module Eurocard)**  
  A modular asynchronous computer architecture for data transfer, storage, and processing (defined by IEEE-1014-1987 specifications).  

  - Three card heights are allowed: 3U, 6U, or 9U (1U = 43.60mm).  
  - A single-slot card is 6T wide (1T = 5.08mm).  
  - Length: 160mm or 340mm.

- **VME64**  
  An extension of VME specifications offering a larger 64-bit data path and addressing range.

- **VME64x**  
  A further extension of VME64, providing geographical addressing capability and larger bandwidth for data transfer.

- **VME64xP**  
  VME64x extension for Physics, adding features useful for physics experiments, such as additional user-defined I/O pins.

- **VSWR (Voltage Standing Wave Ratio)**  
  \( \text{VSWR} = \frac{E_i + E_r}{E_i - E_r} \), where \( E_i \) is the incident wave amplitude and \( E_r \) the reflected wave amplitude.

---

## Z

- **Zero Suppression**  
  A digital technique that skips values below a programmable threshold from memory.

# Embedded Systems Roadmap  

This roadmap is for students and early engineers who want to become **actually employable** in embedded systems.

**Reality check:**  
If you start seriously in mid-college and stay consistent, **2–3 years** is a realistic timeline for good embedded product roles.

There are shortcuts to interviews.  
There are **no shortcuts to competence**.

---

## 🔲 Phase 0 — Foundations (0–3 Months)

> **Goal:** Make C programming and basic electronics bulletproof.

### What to focus on
- C memory model (stack, heap, BSS, data)
- Pointers, structs, bit-fields
- `volatile`, `const`, `static`
- Bitwise operations & masks
- Compiler warnings & basic build systems (Make/CMake)
- Digital electronics: pull-ups, pull-downs, debouncing
- Power basics: LDO vs SMPS, decoupling
- OS basics: process vs thread, interrupts, real-time meaning

### Mandatory mini-projects
- Circular buffer in pure C
- Command parser in C
- Simple cooperative scheduler
- Timer-based LED blink (no delays)
- Button debouncing
- UART echo

### Exit criteria
✔ Can explain *why* bugs happen  
✔ Comfortable reading datasheets  
✔ C syntax no longer slows thinking

---

## 🔲 Phase 1 — Microcontroller Depth (3–9 Months)

> **Goal:** Move from Arduino-level to real firmware engineering.

### Choose ONE MCU family
- **STM32** → industrial / control / automotive  
- **ESP32** → IoT / wireless products  

*(Depth > breadth)*

### Core topics
- MCU architecture & startup sequence
- Clock tree configuration
- Register-level programming
- GPIO, Timers, PWM
- ADC fundamentals
- UART, SPI, I2C
- Watchdog timers
- Low-power modes

### Tooling habits
- GCC toolchain basics
- Debugging with breakpoints & registers
- Git (clean commits, branches, README discipline)
- Linux CLI (build, flash, serial tools)

### Projects that matter
- Sensor node (multiple sensors + filtering)
- Motor control with PWM + encoder
- Custom GPIO/UART drivers from reference manual

### Exit criteria
✔ Can write drivers without copy-paste  
✔ Debugs peripherals logically  
✔ Understands timing constraints

---

## 🔲 Phase 2 — RTOS & Product Thinking (9–18 Months)

> **Goal:** Write firmware that behaves like a real product.

### RTOS (FreeRTOS)
- Tasks & priorities
- Queues, semaphores, mutexes
- Software timers
- ISR-safe APIs
- Deadlocks & priority inversion
- When NOT to use RTOS

### Communication & connectivity
- UART, SPI, I2C (deep understanding)
- CAN (strong plus)
- Wi-Fi / BLE fundamentals
- MQTT / HTTP basics

### Embedded Linux (optional but powerful)
- Cross-compilation basics
- Device tree concepts
- Userspace vs kernel drivers
- Buildroot / Yocto awareness

### Product-level projects
- RTOS-based IoT node (sensor + comm + logging tasks)
- Data logger (SD card + RTC + power-fail safety)
- MCU ↔ Linux board communication (SPI/I2C)

### Exit criteria
✔ Designs task architecture before coding  
✔ Can explain latency & timing  
✔ Thinks in failure modes

---

## 🔲 Phase 3 — Specialization & Senior Mindset (18–36 Months)

> **Goal:** Become valuable in a specific embedded domain.

### Pick 1–2 tracks only

#### 🚗 Automotive / Safety
- CAN, LIN basics
- AUTOSAR concepts
- MISRA-C discipline
- Functional safety mindset

**Practice:**  
Two MCUs exchanging CAN messages with error handling.

---

#### 🌱 Industrial IoT / Low Power
- Sleep strategies
- Power profiling
- Watchdog strategy
- Secure boot concepts
- OTA update design

---

#### 🐧 Embedded Linux / Edge
- Embedded Linux app development
- Cross-compiling workflows
- Remote update mechanisms
- TinyML concepts (optional)

---

## 🔲 Senior-Level Habits (What Companies Pay For)

- Design before coding
- State machines & layering
- Hardware-agnostic abstractions
- Error handling & timeouts
- Logging & diagnostics
- Clear documentation

Your GitHub **must show**:
- Clean folder structure
- Meaningful commit history
- READMEs explaining **why**, not just **what**

---

## 🔲 Final Reality Check

- Certifications rarely decide hiring
- Projects + debugging do
- 2–3 deep courses > 10 shallow ones
- Embedded rewards patience, depth, and calm thinking

If you enjoy **debugging more than shortcuts**, you’re in the right field.

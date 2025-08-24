## 📦 COTS-STM32F1

A structured, layered repository for STM32F1 development using bare-metal techniques. Built to reinforce low-level understanding and modular design principles in embedded systems.

---


### 🧱 Architecture Overview

```
COTS-STM32F1/
├── LIB/         # Platform-independent utilities (e.g., ring buffers, math libs)
├── MCAL/        # Microcontroller Abstraction Layer (register-level drivers)
├── HAL/         # Hardware Abstraction Layer (peripheral interfaces)
├── APP/         # Example applications or test cases
├── docs/        # Schematics, datasheets, pinouts, design notes.
└── README.md    # This file
```

---


### 🎯 Project Scope

This repository explores embedded systems development on STM32F1 using a layered architecture. It emphasizes clarity, modularity, and low-level control through direct register access. The structure is intentionally manual and granular, designed to reinforce foundational understanding rather than optimize for speed or abstraction.

While the layered methodology introduces separation of concerns (LIB, MCAL, HAL, APP), it remains tightly coupled to the hardware and avoids high-level frameworks or auto-generated code. Each layer serves as a stepping stone to deeper insight into how embedded systems operate beneath the surface.

---

### 📚 Layer Breakdown

| Layer     | Description                                                 |
|-----------|-------------------------------------------------------------|
| **LIB**   | Generic C utilities not tied to STM32 (e.g., math, buffers) |
| **MCAL**  | Low-level drivers using direct register access (e.g., GPIO,ADC)              |
| **HAL**   | Abstracted interfaces with different deviced used in embedded systems built on MCAL (e.g., sensor wrappers, motor interface) |
| **APP**   | Simple test cases and usage examples                        |


---

### 📄 License

Licensed under the **MIT License** to allow free use and modification. See [LICENSE](LICENSE) for details.



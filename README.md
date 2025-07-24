
# 📦 Automated Warehouse Simulation with TIA Portal and Factory I/O

A complete simulation of an automated warehouse system using Siemens TIA Portal and Factory I/O. The project integrates ladder logic with a 3D warehouse model to demonstrate the storage, retrieval, and transport of boxes via conveyor belts and a stacker crane.

---

## 📚 Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies & Requirements](#technologies--requirements)
- [Installation Guide](#installation-guide)
- [Usage Instructions](#usage-instructions)
- [Demo Preview](#demo-preview)


---

## ✅ Features

- 🔄 Full automation cycle: box input, storage, retrieval, and output.
- 🤖 Control of conveyors, sensors, emitter/remover, and stacker crane using Ladder Logic.
- 🖥️ Real-time simulation using **Factory I/O** with 3D visualization.
- 🧠 Modular and flexible PLC logic, easily expandable.
- 🧪 Includes emergency stop, start/reset buttons, and selector for manual/auto control.
- 🛠️ TIA Portal-compatible project structure using **S7-1200 V15**.

---

## 📁 Project Structure

```

badredenyx-plc\_tiaportal\_autowarehouse/
├── README.md
├── Automated Warehouse.factoryio         # 3D simulation scene file for Factory I/O
└── FactoryIO\_Template\_S7-1200\_V15\_V15.1/ # TIA Portal PLC project
├── \*.ap15\_1                           # Main project archive
├── project\_structure.txt             # Project content overview
├── IA\_hw\_FIO\_TIA/                    # Core simulation setup
│   ├── \*.sim15\_1                     # Simulation project
│   └── System/, XRef/, AdditionalFiles/
└── Logs/                             # Conversion logs between TIA versions

````

---

## 🛠️ Technologies & Requirements

- **TIA Portal** V15.1 or newer (for PLC programming)
- **Factory I/O** v2.2.2 or compatible (for simulation)
- **Siemens S7-1200** controller support
- Basic understanding of Ladder Logic and industrial control systems

---

## 📦 Installation Guide

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/badredenyx-plc_tiaportal_autowarehouse.git
   ````

2. **Open the TIA Portal project**

   * Launch Siemens TIA Portal V15.1+
   * Open `FactoryIO_Template_S7-1200_V15_V15.1.ap15_1` from the `FactoryIO_Template_S7-1200_V15_V15.1` folder

3. **Open the Factory I/O scene**

   * Start Factory I/O
   * Load `Automated Warehouse.factoryio` from the root folder
   * Ensure the I/O driver is set to **S7-1200 (ISO on TCP)**

4. **Connect and Simulate**

   * Use PLCSIM to simulate the PLC if no hardware is connected
   * Connect Factory I/O to the virtual PLC via TIA Portal’s IP configuration

---

## 🚀 Usage Instructions

1. **Start Simulation**

   * Run the PLC logic in TIA Portal (via online or PLCSIM)
   * Play the scene in Factory I/O

2. **Interact with the System**

   * Use the **Start**, **Stop**, and **Reset** buttons to control the system
   * Use the selector switch to toggle **Manual/Auto** mode

3. **Observe Operations**

   * Boxes are emitted, transported via conveyors, stored in racks by a stacker crane, then retrieved

4. **Modify Logic**

   * Adjust the ladder logic in TIA Portal to customize automation flow
   * Expand the project to include barcode readers, SCADA integration, etc.

---

## 🎥 Demo Preview

> *(You can replace this with your own GIF or video)*
> ![Simulation Demo](https://github.com/Badredenyx/PLC_TiaPortal_AutoWarehouse/main/Simulation.gif)

---

## 🤝 Contributing

Want to improve the automation logic or add new features?

1. Fork the repository
2. Create a feature branch (`git checkout -b new-feature`)
3. Commit your changes (`git commit -am 'Add feature'`)
4. Push to your fork (`git push origin new-feature`)
5. Submit a Pull Request

---

## Credits
This project was created by me as part of the Industrial Automation course.

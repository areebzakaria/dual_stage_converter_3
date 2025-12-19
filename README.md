# Dual-Stage Buck Converter (44V to 12V & 5V)

This project features a high-efficiency dual-stage DC-DC buck converter designed using the **Texas Instruments LMR36506 synchronous regulator**.  
The board is optimized for a compact **40mm x 40mm footprint**, focusing on robust thermal management and EMI shielding.

---

## Technical Specifications
- **Input Voltage:** 44V DC (Nominal)  
- **Stage 1 Output:** 12V DC @ 600mA  
- **Stage 2 Output:** 5V DC @ 600mA (cascaded from 12V rail)  
- **Regulator IC:** LMR36506 (RPE Package - 9-Pin VQFN)  
- **Switching Frequency:** High frequency for reduced inductor size  

---

## Hardware Features

### 1. Thermal Management
Since the Stage 1 regulator drops a significant voltage (44V → 12V), heat dissipation is critical.
- **Thermal Vias:** An array of 0.25mm vias is placed directly on the IC's center thermal pad (Pin 9) to conduct heat to the bottom layer.  
- **Ground Plane:** A solid copper pour on the bottom layer acts as a primary heat sink and EMI shield.  

### 2. PCB Layout Optimization
- **Compact Footprint:** Entire design fits within a 40mm × 40mm area.  
- **High-Voltage Safety:** Optimized trace clearances (0.2mm) to handle the 44V input safely.  
- **Power Flow:** Linear layout from left (Input) to right (Output) with thick 0.8mm–1.0mm power traces.  
- **Connectors:** Standard 2.54mm pitch headers for easy lab probing and integration.  

---

## Project Goals
- Deliver a compact, efficient dual-stage buck converter for high-voltage input applications.  
- Ensure robust thermal management and EMI shielding for reliable operation.  
- Provide a lab-friendly design with standard connectors and safe clearances.  

---

## License
This project is released under the MIT License. See [LICENSE](LICENSE) for details.

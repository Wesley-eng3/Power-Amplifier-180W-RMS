# Power-Amplifier-180W-RMS

This is a 180W RMS power amplifier project featuring a preamplifier stage, 3-band tone control (bass, middle, treble), and a symmetrical power supply. Ideal for high-power audio applications such as active speaker systems, DIY audio projects, and electronic experimentation.

📐 Specifications
Output Power: up to 180W RMS @ 4Ω

Amplifier Topology: Class AB

Output Transistors:

2SC5200 (NPN)

2SA1943 (PNP)

Preamplifier: TL072 with 3-band tone control

Power Supply:

Symmetrical power supply with rectification and filtering

Dual AC input

Recommended voltage: ±45VDC

Protections:

Flyback diodes for current return protection

2.5A fuses on power rails

Controls:

Volume

Bass

Middle

Treble

3-position gain switch (20dB / 10dB / 30dB)

🧩 Circuit Sections
🔌 Power Supply
Full-wave rectifier using 1N4001 diodes

1000µF and 100nF filter capacitors

Symmetrical outputs: +DC / -DC

🎛️ Preamp
TL072 operating with symmetrical power

3-band active tone control (P1, P2, P3)

Volume control (P4)

Gain selector switch with R2, R3, and R4

🔉 Power Amplifier (AMP 90W - 180W)
Differential input stage with Q1 (BC556) and Q2 (BC556)

Driver stage with Q3 (BC546), Q4 (BC546)

Output stage with Q6 (BD139), Q5 (BD140), Q8 (2SC5200), Q9 (2SA1943)

Emitter resistors for thermal stabilization

Protection diodes (D5–D9)

📁 Included Files
amplifier_schematic.png: Complete circuit schematic

Schematic

<img width="1241" height="823" alt="Schematic" src="https://github.com/user-attachments/assets/fc22f6bc-fc34-47dc-b27d-925f47f7dc81" />

Altium Tool View

<img width="1473" height="816" alt="PCB Altium" src="https://github.com/user-attachments/assets/d935e22d-6ecb-44c4-a7ff-4a2197f79d99" />

3D View

<img width="7413" height="3598" alt="PCB1" src="https://github.com/user-attachments/assets/7f1742a1-d08c-4fed-b315-8154a2a42b59" />

<img width="1266" height="817" alt="PCB2" src="https://github.com/user-attachments/assets/f8415547-8df5-4f33-8faa-d0757647107a" />

Top Layer

<img width="1562" height="672" alt="Top" src="https://github.com/user-attachments/assets/943e195c-ee20-4bcb-a833-a62602e84ff6" />

Bottom

<img width="1472" height="632" alt="Bottom" src="https://github.com/user-attachments/assets/c821a09a-0979-4d76-b191-10bd5b8e272f" />

🛠️ Requirements
Symmetrical power supply around ±45VDC (not included)

Heatsinks for power transistors

Printed circuit board (PCB) or perfboard/protoboard

Advanced electronics knowledge

📦 BOM – Power Amplifier 180W RMS (AMP + Power Supply)
Ref.	Component	Value / Part Number	Notes
Q1	PNP Transistor	BC556	Differential input stage
Q2	PNP Transistor	BC556	
Q3	NPN Transistor	BC546	Driver stage
Q4	NPN Transistor	BC546	VAS stage
Q5	PNP Power Transistor	BD140	Driver for Q9
Q6	NPN Power Transistor	BD139	Driver for Q8
Q8	NPN Output Power Transistor	2SC5200	Output stage
Q9	PNP Output Power Transistor	2SA1943	Output stage
D1–D4	Diode	1N4001	Bridge rectifier (AC1)
D10–D13	Diode	1N4001	Bridge rectifier (AC2)
D5–D9	Diode	1N4148 / 1N4007	Protection diodes
C1–C4	Electrolytic Capacitor	1000µF / 63V	Power supply filtering
C5	Polyester Capacitor	100nF	High-frequency decoupling
C6	Electrolytic Capacitor	220nF	Input coupling
C7	Electrolytic Capacitor	100µF	Supply decoupling
C8	Ceramic Capacitor	4.7µF	Coupling
C9	Electrolytic Capacitor	22µF	Feedback loop
C10	Ceramic Capacitor	120pF	Compensation capacitor
C11	Electrolytic Capacitor	47µF	Bootstrap
R1	Resistor	150k	Input bias
R2	Resistor	680R	Feedback
R3	Resistor	20k	
R4	Resistor	100R	
R5	Resistor	1k	
R6	Resistor	22k	
R7	Resistor	7.5k	
R8	Resistor	7.5k	
R9, R10	Resistor	2.2k	
R11, R12	Power Resistor	0.1Ω / 5W	Emitter resistor (output)
F1, F2	Fuse	2.5A	Line protection
AC1, AC2	AC Connectors	2-pin screw terminal	
OUT (AMP)	Output Connector	2-pin screw terminal	To speaker
Switch	SP3T Toggle Switch	3-Position (On-Off-On)	Gain selection

🎚️ BOM – Preamp Section
Ref.	Component	Value / Part Number	Notes
U1	Dual Op-Amp	TL072	Main preamp IC
P1	Potentiometer	100k Linear	Bass control
P2	Potentiometer	100k Linear	Middle control
P3	Potentiometer	500k Linear	Treble control
P4	Potentiometer	10k Linear	Volume control
R1	Resistor	150k	Input bias
R2	Resistor	220k	Gain path
R3	Resistor	56k	Gain path
R4	Resistor	470k	Gain path
R5, R6	Resistor	12k	Tone control
R7, R9	Resistor	3.9k	Tone control
R8	Resistor	22k	Tone control
R10	Resistor	1.8k	Tone control
R11	Resistor	100k	Tone output
R12, R13	Resistor	22k	Pull-down
C1	Capacitor	220nF	Input coupling
C2, C3, C4, C5, C6	Capacitor	4.7µF	Tone path
C7	Electrolytic Capacitor	100µF	VCC decoupling
C8	Capacitor	4.7µF	Output coupling
CX	Capacitor	100µF	VCC filtering
IN, IN AMP	3-pin/2-pin Connector	Screw terminal	Audio input/output

⚠️ Warning
Caution: This circuit operates with high voltages. Handle with care and make sure components are correctly rated to avoid damage or safety risks.

👨‍💻 Author
Project developed by Wesley Freitas


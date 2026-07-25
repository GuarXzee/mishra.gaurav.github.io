## Antenna Fundamentals

>CST: Computer Simulation Technology

### RF Parameters
#### S-Parameters
- Describe how RF energy travels between ports in a network.
- Used to model input-output behavior in multiport systems.
- Common parameters: S11, S12, S21, S22.
- Reflection parameters: S11 and S22.
- Transmission parameters: S12 and S21.
- S-parameters help calculate return loss, impedance, admittance, VSWR, gain/loss, phase, and group delay.

#### S11 Parameter
- Input-port reflection coefficient.
- Measures power reflected back from port 1.
- Used to check antenna matching.
- Good match: S11 < -10 dB (≈ 90% power accepted).
- At -3 dB, transmitted and reflected power are equal.

#### S22 Parameter
- Output-port reflection coefficient.
- Measures power reflected back from port 2.
- Works like S11 for the second port.
- Together with S11, it gives return loss, impedance, admittance, and VSWR for both ports.

#### S12 Parameter
- Reverse transmission coefficient.
- Measures power from port 2 delivered back to port 1.
- Useful for evaluating reverse coupling.

#### S21 Parameter
- Forward transmission coefficient.
- Measures power from port 1 delivered to port 2.
- Used to evaluate insertion loss or gain.
- Important for EBG/FSS structures to assess how much signal passes through or is absorbed.
- Also gives phase and group delay information.

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 300" width="640" height="300" font-family="Cambria, Georgia, serif">
  <defs>
    <marker id="arr" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="8" markerHeight="8" orient="auto-start-reverse">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="#7f9fc4"/>
    </marker>
  </defs>
  <rect x="230" y="55" width="180" height="180" rx="28" fill="none" stroke="#8fa8c8" stroke-width="1.5"/>
  <text x="320" y="152" font-size="22" text-anchor="middle" fill="#ffffff">Component</text>
  <line x1="40" y1="100" x2="222" y2="100" stroke="#7f9fc4" stroke-width="2.5" marker-end="url(#arr)"/>
  <line x1="410" y1="150" x2="600" y2="150" stroke="#7f9fc4" stroke-width="2.5" marker-end="url(#arr)"/>
  <line x1="230" y1="195" x2="48" y2="195" stroke="#7f9fc4" stroke-width="2.5" marker-end="url(#arr)"/>
  <text x="42" y="45" font-size="22" fill="#ffffff">Incident</text>
  <text x="42" y="75" font-size="22" fill="#ffffff">Power</text>
  <text x="425" y="105" font-size="22" fill="#ffffff">Transmitted</text>
  <text x="425" y="135" font-size="22" fill="#ffffff">Power</text>
  <text x="45" y="235" font-size="22" fill="#ffffff">Reflected</text>
  <text x="45" y="265" font-size="22" fill="#ffffff">Power</text>
</svg>

#### Insertion Loss
- Insertion Loss = Transmitted power / Incident power.

#### Return Loss
- Return Loss = Reflected power / Incident power.

#### VSWR
- Voltage Standing Wave Ratio.
- Measures mismatch between antenna and feed line.
- Indicates reflected standing waves along the feeder.
- Range: 1 to infinity.
- VSWR < 2 is generally acceptable.
- VSWR > 2 means poor matching at that frequency.

#### Gain
- Ratio of power radiated in a direction to power from an isotropic antenna.
- 3 dB gain means twice the power in that direction compared to isotropic.

#### RCS
- Radar Cross Section.
- Describes how detectable an object is by radar.
- Large RCS means easier detection.

#### Bandwidth
- Frequency range over which the antenna works effectively.
- Wider bandwidth covers more radio frequencies.
## S-Parameters for Patch antenna
### Antenna Description
- Patch size: 28 x 36 mm.
- Feed size: 14 x 2 mm.
- Substrate size: 56 x 50 mm.
- Ground plane size: 56 x 50 mm.

### Simulation Process
- Create discrete edge port from the edge of the ground plane to the feed.
- Go to Simulation -> Global Properties -> Tetrahedral -> Cells per Wavelength and reduce mesh count if required.
- Go to Home -> Setup Solver -> Specials -> Max Number of Passes and reduce max mesh assignments for the free version.
- Run simulation.
- Open 1D Results -> S-Parameters.

## Microstrip Patch Antenna Gain Analysis
### Setup
- Go to Simulation -> Field Monitor.
- Set monitor frequency to 2.4 GHz.
- Enable Far Field.
- Enable E-field.
- Enable Surface Current.
- Enable Current Density.
- Enable Power Loss Density.
- Click Apply.
- Click OK.

### Simulation
- Go to Home -> Start Simulation.
- Wait for the solver to complete.
- Open Results section.

### Gain results
- Locate Gain result in far field results.
- Gain = 2.944 dB.
- Realized gain = 2.594 dB.
- Note radiation efficiency result.
- Note total efficiency result.

### Visualization
- In Results, open Far Field cut at 2.4 GHz.
- Use color palette to inspect gain magnitude.
- Right-click -> Structure Transparency -> Far Field Transparency.
- Verify antenna structure in the far field display.
- Confirm radiation pattern direction toward +Z axis.
- Open 2D plot for realized gain.
- Open Cartesian plot: main lobe at 0°, magnitude 2.59 dB.
- Open Polar plot: main lobe at 0°, magnitude 2.59 dB.

### Field and current results
- Open E-field result and animate field lines.
- Open H-field result and animate magnetic field.
- Open surface current density result.
- Verify current density from feed across the patch.
- Change display mode to streamlines.
- Change display mode to bubbles.
- Change display mode to arrows.
- Observe non-uniform current distribution.
- Note that slots may improve current uniformity.

### Additional results
- Open VSWR result.
- Open Z-matrix result.
- Open Y-matrix result.
- Open Balance result.
- Confirm all selected monitor results are available.
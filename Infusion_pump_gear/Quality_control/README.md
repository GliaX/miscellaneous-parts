# Design Intent & Quality Control - Infusion Pump Gear

## 1. Primary Function & Purpose
- **Application:** Precise torque and rotational motion transfer within the infusion pump mechanism.
- **Critical Requirement:** Smooth engagement with zero tooth slipping to maintain accurate, controlled liquid delivery.

## 2. Material Selection & Rationale
- **Approved Materials:** ABS or PETG.
- **Rationale:** Selected for high mechanical strength, fatigue tolerance, and low friction wear resistance required for continuous pump operation.

## 3. Manufacturing Specifications (FDM / 3D Printing)
- **Print Orientation:** Flat on the print bed (aligns layer orientation perpendicular to tooth shear force vectors for maximum strength).
- **Infill:** 100% Solid (Ensures maximum core density and prevents internal structural collapse under torque).
- **Wall Thickness / Shells:** 5 Perimeters (Horizontal Shells) to ensure the gear teeth consist of solid extruded lines rather than infill pattern gaps.
- **Layer Height:** 0.2 mm (Optimal balance between dimensional resolution of tooth profiles and inter-layer adhesion strength).

## 4. Quality Control & Inspection Checklist

### Phase 1: Bench & Mechanical Verification
- [ ] **Dimensional Tolerance:** Verify pitch and outer diameter within ±0.1 mm accuracy using calipers.
- [ ] **Tooth Surface Finish:** Inspect gear teeth faces for zero stringing, blobs, or under-extrusion artifacts.
- [ ] **Shaft Alignment Test:** Mount on the motor/pump shaft to confirm a secure, precise fit without mechanical play or slippage.
- [ ] **Manual Mesh Test:** Manually rotate in mesh with the mating gear inside the pump housing to verify smooth, continuous rotation without binding.

### Phase 2: Dynamic Functional Testing (Validation Stage)
- [ ] **Fluid Dispensing Accuracy Test:** Run an active pumping cycle to discharge **500 mL of water** over a targeted timeframe. Verify that the output volume and flow rate match calibration specs with zero mechanical slippage or timing errors under continuous load.

For more detailes about tests, see the [Testing Protocol](testing-protocol.md).

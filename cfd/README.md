# CFD Analysis — ANSYS Fluent 2021 R2

## Files

| File | Description |
|------|-------------|
| `cfd_results.png` | Pressure contour and pressure-velocity graph |

## Simulation Setup

| Parameter | Value |
|-----------|-------|
| Software | ANSYS Fluent 2021 R2 |
| Mesh type | Unstructured mesh with adaptive sizing |
| Solver | Pressure-based, density-coupled |
| Turbulence model | k-ω (also tested k-ε) |
| Iterations | 1500 |
| Geometry | 2D axisymmetric CD nozzle |

## Boundary Conditions

| Boundary | Condition |
|----------|-----------|
| Inlet | Pressure inlet (chamber pressure) |
| Outlet | Pressure outlet (1 atm atmospheric) |
| Wall | No-slip, adiabatic |
| Axis | Symmetry |

## Results

- **Supersonic flow** achieved in divergent section (Mach > 1 downstream of throat)
- **Pressure drops** continuously from inlet to exit as expected in isentropic expansion
- **Velocity increases** through convergent section to sonic at throat, then supersonic in divergent
- At **~70% nozzle length**, turbulence near divergent wall was observed
- Reducing nozzle length below 50% would improve wall boundary layer but reduce efficiency

## CFD Workflow

```
Geometry Import (SolidWorks → ANSYS Workbench)
        ↓
Meshing (ANSYS Meshing — unstructured, refined at throat)
        ↓
Physics Setup (Fluent — compressible, turbulence model, BCs)
        ↓
Solving (1500 iterations, residual convergence)
        ↓
Post-Processing (pressure contour, velocity contour, P-V graph)
```

## Key Findings

The CD nozzle effectively accelerates the combustion gases to supersonic speeds. The pressure and velocity contours confirm design intent and validate the nozzle geometry for the KNSU propellant operating conditions.
